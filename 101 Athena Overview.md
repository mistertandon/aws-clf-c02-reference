
---

## 196. 
![alt text](https://github.com/mistertandon/aws-clf-co2-slides-by-stephane-maarek/blob/main/s9/196.png)

Amazon Athena is a serverless, interactive query service that enables SQL-based analytics on data stored in Amazon S3. Built on the Presto engine, Athena supports various file formats, including CSV, JSON, ORC, Avro, and Parquet, allowing users to analyze data without the need for ETL processes or additional infrastructure.

Users can query data directly from S3, leveraging Athena’s integration with AWS services like Amazon QuickSight for advanced visualization and reporting. Athena's pay-per-query model charges approximately $5 per terabyte of data scanned, with significant cost savings when data is compressed or stored in columnar formats such as Parquet or ORC, as these reduce the volume of data scanned.

Athena excels in diverse use cases, including business intelligence, ad hoc querying, and log analysis. It is particularly effective for analyzing logs from AWS services such as VPC Flow Logs, ELB Logs, and CloudTrail, providing actionable insights for operational and security audits. By eliminating the need for infrastructure management, Athena streamlines data analytics, enabling rapid, scalable insights.

---
