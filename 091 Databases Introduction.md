
---

## 175. Database Introduction


When storing data on AWS, whether using Amazon EBS, EC2 Instance Store, Amazon S3, or Amazon EFS, it’s important to consider the specific capabilities and limitations of each service. These storage solutions are suitable for file operations and unstructured data storage. However, when structured data management is required, databases become essential.

AWS databases like Amazon RDS, Amazon DynamoDB, and Amazon Aurora provide advanced features for structured data storage. They enable efficient indexing, querying, and searching while supporting the definition of relationships between datasets. Modern AWS-managed databases are purpose-built, optimized for specific workloads, and equipped with features such as automated scaling, high availability, and robust security configurations to meet diverse application requirements.

---

## 176. Relational database

Relational databases leverage SQL (Structured Query Language) to perform queries, updates, and lookups, making them ideal for applications requiring strict consistency, well-defined schemas, and advanced querying capabilities. AWS offers managed relational database services like Amazon RDS and Amazon Aurora, which streamline provisioning, scalability, and maintenance for cloud-native applications.

---

## 177. NoSQL database

NoSQL databases, or non-relational databases, are purpose-built for modern applications with specific data models in mind. They provide a flexible, schema-less architecture, enabling developers to adapt data structures as application requirements evolve. This flexibility makes NoSQL databases ideal for dynamic, high-performance workloads.

Key benefits of NoSQL databases include horizontal scalability through distributed servers, unlike relational databases that rely on vertical scaling. Their architecture optimizes performance for specific use cases, such as high-throughput transactions, real-time analytics, or complex relationship querying.

AWS offers several NoSQL database solutions tailored to various data models, including Amazon DynamoDB for key-value and document storage, Amazon ElastiCache for in-memory caching, Amazon Neptune for graph databases, and Amazon OpenSearch Service for search and analytics workloads. These services combine scalability, performance, and seamless integration with other AWS offerings, making them powerful tools for building modern, cloud-native applications.

---

## 178. JSON (JavaScript Object Notation)

NoSQL databases, such as Amazon DynamoDB or Amazon DocumentDB, often store data in JSON (JavaScript Object Notation) format. JSON provides a flexible structure with nested objects, diverse field types, and schema-less design, making it ideal for modeling complex and dynamic datasets. This versatility enables developers to efficiently represent and query hierarchical or semi-structured data in modern NoSQL environments.

---

## 179. Database & shared responsibility on AWS

AWS managed database services, such as Amazon RDS, Amazon DynamoDB, and Amazon Aurora, provide significant advantages over self-managed databases on EC2. These services enable rapid provisioning and are built to ensure high availability with support for vertical and horizontal scaling. AWS automates critical operations, including backups, restores, software patching, and upgrades, freeing you from managing the underlying infrastructure.

Integrated features such as Amazon CloudWatch monitoring and alerting enhance visibility and operational efficiency. In contrast, running databases on EC2 requires you to handle all aspects of resiliency, backup strategies, patching, fault tolerance, and scaling, increasing operational complexity and risk. AWS managed databases simplify these tasks, allowing you to focus on application development rather than infrastructure management.

---
