
---

## 189. 
![alt text](https://github.com/mistertandon/aws-clf-co2-slides-by-stephane-maarek/blob/main/s9/189.png)

DynamoDB is a fully managed, serverless NoSQL database designed for high availability and durability, with automatic data replication across three Availability Zones. As a key-value and document database, it is optimized for handling massive workloads at scale, making it one of AWS's premier services for modern application development.

Unlike managed services such as Amazon RDS or Amazon ElastiCache, DynamoDB abstracts server provisioning entirely, enabling developers to focus on application logic rather than infrastructure management. While underlying servers power its operation, they remain invisible to users, offering a seamless, serverless experience.

DynamoDB delivers exceptional scalability, supporting millions of requests per second, trillions of rows, and storage scaling into hundreds of terabytes. Its consistent, single-digit millisecond response times ensure low-latency data retrieval, crucial for performance-intensive applications.

Security and governance are seamlessly integrated through AWS Identity and Access Management (IAM), providing robust authorization and administration capabilities. DynamoDB also includes auto-scaling to adapt to dynamic workloads and cost-efficient table classes—*Standard* and *Infrequent Access (IA)*—to optimize storage costs based on data access patterns.

By combining these features with AWS-native tools and integrations, DynamoDB empowers developers to build scalable, high-performance, and cost-effective applications.

---

## 190. 
![alt text](https://github.com/mistertandon/aws-clf-co2-slides-by-stephane-maarek/blob/main/s9/190.png)

DynamoDB stores data in a key-value format and organizes it using a flexible schema structure optimized for high performance and scalability. Each item in a DynamoDB table is uniquely identified by a **primary key**, which can be either: 

- A **partition key** (single attribute) or  
- A **composite primary key** comprising a partition key and a sort key.  

In addition to the primary key, you can define custom attributes to store additional data, effectively functioning as columns in your table. Items are organized into rows, but unlike relational databases, DynamoDB does not enforce a fixed schema, allowing each item to include a unique set of attributes.

This schema-less design, combined with single-digit millisecond latency for data retrieval, makes DynamoDB a powerful NoSQL database solution. It is fully serverless, eliminating infrastructure management while enabling dynamic scaling to handle workloads of any size efficiently.

---

## 191. 
![alt text](https://github.com/mistertandon/aws-clf-co2-slides-by-stephane-maarek/blob/main/s9/191.png)


DynamoDB Accelerator (DAX) is a fully managed in-memory caching service purpose-built for DynamoDB, delivering microsecond latency for read-intensive workloads. By caching frequently accessed data, DAX can improve performance by up to 10 times, significantly enhancing application responsiveness.

DAX is tightly integrated with DynamoDB, eliminating the need for developers to modify their existing application logic for caching. It automatically handles cache invalidation, cluster management, and scaling, enabling seamless acceleration for queries like `GetItem`, `BatchGetItem`, and query operations.

Unlike Amazon ElastiCache, which supports caching for various databases, DAX is exclusive to DynamoDB. This specialization ensures optimized performance and simplicity for DynamoDB workloads. DAX also supports IAM for secure access, and its highly scalable, distributed architecture maintains availability even during peak loads. This makes DAX an essential tool for developers requiring ultra-low latency and efficient data access in DynamoDB-powered applications.

---
