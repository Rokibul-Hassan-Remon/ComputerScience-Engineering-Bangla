[Latency -llya Grigorik](https://www.youtube.com/watch?v=g3prXpNjI7U&list=PL7CF533399C1ECDE5)

In 2015, a small team of engineers built Discord in just 60 days.  
  
By 2016, their database was collapsing under the load of 1 billion+ messages per day.  
  
Here’s how they scaled to billions of messages & without downtime  
  
1. Choosing MongoDB for Speed  
Discord started with a MongoDB replica set to move fast and test features.  
  
What Went Wrong:  
- By 100M messages, data and indexes couldn’t fit in RAM.  
- Latency spiked as disk reads replaced fast in-memory operations.  
- MongoDB sharding was complex and lacked stability, so scaling vertically wasn’t an option.  
  
2. The Migration – Moving to Cassandra  
Why Cassandra?  
  
- Linear Scalability – Add nodes as needed.  
- High Availability – Tolerates node failures without downtime.  
- Proven Track Record – Used by Netflix and Apple at massive scales.  
- Community-Driven – Open-source with strong support.  
  
Testing the Migration (Dark Launch):  
- Double Writes: Data written to both MongoDB and Cassandra.  
- Double Reads: Queries ran on both to measure performance.  
- Result: Cassandra handled <5ms reads, proving it could handle the scale.  
  
3. The First Major Problem – Upserts and Data Corruption  
  
Cassandra’s AP Model prioritizes availability over consistency, all writes act as upserts (insert or update).  
  
The Issue:  
- Simultaneous edits and deletes led to incomplete data (missing fields).  
- Cassandra couldn’t detect partial updates due to its eventual consistency.  
  
The Fix:  
- Added data validation to detect and delete corrupt rows.  
- Used tombstones (soft deletes) to handle inconsistencies gracefully.  
  
4. The Second Problem – Tombstone Overload Crashed Cassandra  
6 months later, Cassandra slowed to a crawl  
  
The Cause:  
- A single channel had 1 message but millions of deleted entries (tombstones).  
- Cassandra scans tombstones during reads, leading to high GC pressure and stop-the-world pauses.  
  
The Fix:  
1. Reduced tombstone lifespan from 10 days to 2 days to clean up faster.  
2. Optimized queries to skip empty partitions and avoid scanning useless tombstones.  
  
3. Final Optimizations – Bucketing Data for Scale  
Large Discord channels grow indefinitely, leading to massive partitions that are expensive to read.  
  
The Fix:  
- Bucketing Messages by Time, stored 10 days’ worth of data per bucket.  
- Each bucket created a fixed partition size, preventing performance degradation.  
  
Where Discord Stands Today  
- Runs a 12-node Cassandra cluster with a replication factor of 3.  
- Plans to upgrade to Cassandra 3 for 50% better storage efficiency.  
- Exploring ScyllaDB (C++ rewrite of Cassandra) for faster performance and lower GC pressure.  
  
Reference Blog: [https://lnkd.in/ghD-98-y](https://lnkd.in/ghD-98-y)