System design is one of the most important areas of backend and full-stack engineering — and it can be intimidating when you’re starting out. But don’t worry, I’ve broken it down into **30 simple concepts**, each with a **tiny definition** to help you understand the building blocks of modern systems.

Whether you’re prepping for interviews or just want to design better systems, this guide is a solid place to begin. Let’s jump in! 👇

# 1. Client-Server Architecture

A model where a client requests resources, and a server responds. This is how browsers interact with web servers.

# 2. IP Address

A unique string of numbers that identifies a device on a network (like your home address, but online).

# 3. Domain Name System (DNS)

It maps human-readable domain names (like `google.com`) to IP addresses.

# 4. Proxy / Reverse Proxy

A proxy forwards requests from a client to the internet, while a reverse proxy forwards requests from the internet to internal servers.

# 5. Latency

The time it takes for a request to go from client to server and back. Lower latency = faster systems.

# 6. HTTP / HTTPS

Protocols for transferring data over the web. HTTPS is the secure, encrypted version.

# 7. APIs

Application Programming Interfaces let systems talk to each other by exposing structured data and functionality.

# 8. REST

A popular way to design APIs using standard HTTP methods like GET, POST, PUT, DELETE.

# 9. GraphQL

A newer alternative to REST that lets clients specify exactly what data they need.

# 10. Database

Stores structured or unstructured data that can be queried and updated.

# 11. SQL vs NoSQL

SQL is relational (tables with schema); NoSQL is non-relational (documents, key-values, etc.).

# 12. Vertical Scaling

Increasing a server’s power (CPU, RAM, etc.) to handle more load.

# 13. Horizontal Scaling

Adding more servers to handle increased traffic in parallel.

# 14. Load Balancer

Distributes incoming requests across multiple servers to ensure no single server is overloaded.

# 15. Indexing

Speeds up data retrieval in databases by creating a quick lookup structure.

# 16. Replication

Copying data across multiple database servers for reliability and availability.

# 17. Sharding

Splitting a database into smaller chunks (shards) so each server only handles part of the data.

# 18. Vertical Partitioning

Breaking a database table into columns and storing them separately to optimize access.

# 19. Caching

Storing frequently accessed data in memory to avoid repeated computation or slow queries.

# 20. Denormalization

Storing duplicated data in a database to speed up read performance (opposite of normalization).

# 21. CAP Theorem

States that in a distributed system, you can only have two out of three: Consistency, Availability, Partition Tolerance.

# 22. Blob Storage

Used to store large files like images, videos, PDFs — binary large objects.

# 23. Content Delivery Network (CDN)

Distributes content to servers globally so users get faster access from their nearest location.

# 24. WebSockets

A protocol that allows two-way, real-time communication between client and server (used in chat apps, etc.).

# 25. Webhooks

User-defined HTTP callbacks triggered by events (e.g., send a message when someone signs up).

# 26. Microservices

An architecture style where systems are split into small, independent services.

# 27. Message Queues

Help systems handle tasks asynchronously by queuing messages for later processing.

# 28. Rate Limiting

Limits how many requests a user can make in a set time to prevent abuse.

# 29. API Gateway

A single entry point for clients to access multiple services, handles routing, auth, etc.

# 30. Idempotency

An idempotent operation produces the same result no matter how many times it’s executed. Crucial for payment and API reliability.