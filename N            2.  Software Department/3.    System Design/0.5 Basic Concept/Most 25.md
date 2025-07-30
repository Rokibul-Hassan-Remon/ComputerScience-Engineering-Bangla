#### ✅ **1. Client-Server Architecture**

The foundation of all web applications. Your device (client) communicates with a server to exchange data.

#### ✅ **2. IP Address & DNS**

DNS translates human-readable domains into IP addresses so clients can find servers.

#### ✅ **3. Proxy & Reverse Proxy**

Proxies mask client identity, while reverse proxies manage traffic, balance loads, and enhance security.

#### ✅ **4. Latency**

The delay in data transmission. Crucial when dealing with global users and performance optimisation.

#### ✅ **5. HTTP vs HTTPS**

Protocols for data exchange. HTTPS adds encryption (SSL/TLS) for secure communication.

#### ✅ **6. APIs & REST**

APIs connect client and server. REST is the most common design style for scalable web APIs.

#### ✅ **7. Concurrency**

Executing multiple tasks simultaneously. Essential for efficient resource utilisation and scalability.

#### ✅ **8. SQL vs NoSQL**

- **SQL**: Structured, reliable, ideal for transactions (e.g. banking).
    
- **NoSQL**: Flexible, scalable, great for big data and real-time apps.
    

#### ✅ **9. Vertical Scaling**

Upgrade a single machine (more CPU, RAM) to boost performance.

#### ✅ **10. Horizontal Scaling**

Add more machines to handle load. More fault-tolerant and scalable.

#### ✅ **11. Load Balancer**

Distributes incoming requests across multiple servers to prevent overload and ensure uptime.

#### ✅ **12. Indexing**

Improves database read performance by reducing lookup time—like a book’s index.

#### ✅ **13. Replication**

Creates copies of data across databases. Helps in failover and handling read-heavy traffic.

#### ✅ **14. Sharding**

Divides database into smaller chunks (shards) based on a key (like user ID) to scale efficiently.

#### ✅ **15. Vertical Partitioning**

Splits large tables by columns to reduce unnecessary data scanning.

#### ✅ **16. Caching**

Stores frequently accessed data in memory (e.g., Redis, Memcached) to speed up responses.

#### ✅ **17. Denormalization**

Combines related tables to avoid JOIN operations in read-heavy systems.

#### ✅ **18. CAP Theorem**

You can only achieve **two out of three** in distributed systems:

- **Consistency**
    
- **Availability**
    
- **Partition Tolerance**
    

#### ✅ **19. Blob Storage (e.g., S3)**

Used to store large files—images, PDFs, videos—separately from the main app logic.

#### ✅ **20. CDN (Content Delivery Network)**

Delivers content from servers closest to the user, reducing latency and speeding up load times.

#### ✅ **21. WebSockets**

Enable real-time, two-way communication. Great for chat apps, gaming, stock tickers.

#### ✅ **22. Webhooks**

Push-based system integration. Triggers instant updates between services (e.g., Stripe payment events).

#### ✅ **23. Microservices**

Architectural style that breaks an app into smaller, independent services. Easier to scale and maintain.

#### ✅ **24. Message Queues (e.g., RabbitMQ, Kafka)**

Allow asynchronous communication between services, improving fault tolerance and scalability.

#### ✅ **25. Rate Limiting & API Gateway**

Protect APIs from being overwhelmed by limiting request rates and managing access control.