
---

## 205. 
![alt text](https://github.com/mistertandon/aws-clf-co2-slides-by-stephane-maarek/blob/main/s9/205.png)

To excel in the AWS exam, focus on the following key AWS database and analytics services:

- **Relational Databases (OLTP)**: Use **Amazon RDS** and **Amazon Aurora** for relational database management, both of which support SQL. Understand the differences in deployment strategies, such as multi-AZ for high availability, read replicas for scalability, and multi-region setups for disaster recovery and global performance.

- **In-Memory Databases**: Use **Amazon ElastiCache** for caching solutions. For serverless key-value storage, **Amazon DynamoDB** is ideal. Pair **DynamoDB** with **DynamoDB Accelerator (DAX)** for in-memory caching to boost read performance.

- **Data Warehousing (OLAP)**: **Amazon Redshift** is the go-to solution for data warehousing, supporting SQL queries for fast analytics on structured data.

- **Big Data Analytics**: Leverage **Amazon EMR** for Hadoop-based big data processing. For serverless SQL querying on data stored in **Amazon S3**, use **Amazon Athena**.

- **Business Intelligence**: **Amazon QuickSight** provides serverless, scalable dashboards and visualizations, making it an excellent choice for business intelligence solutions.

- **NoSQL Databases**: **Amazon DocumentDB** is a fully managed, MongoDB-compatible database that supports JSON data. It serves as an alternative to **Amazon DynamoDB** for NoSQL applications.

- **Immutable Ledger**: Use **Amazon QLDB** for financial transaction ledgers that require cryptographically verifiable records. Unlike **Amazon Managed Blockchain**, which supports decentralized blockchains, QLDB is designed for central, immutable transaction records.

- **ETL and Data Migration**: **AWS Glue** is a managed ETL service that includes a data catalog for discovering datasets across AWS. For database migrations, **AWS Database Migration Service (DMS)** ensures seamless data transfers between different database platforms.

- **Graph and Time-Series Databases**: For graph database needs, use **Amazon Neptune**. For time-series data, **Amazon Timestream** is optimized for storing and analyzing time-stamped data.

This concise breakdown should provide a clear understanding of AWS database and analytics services, tailored for exam preparation.

---
