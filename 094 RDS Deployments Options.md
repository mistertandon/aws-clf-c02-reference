
---

## 185. RDS deployment: Read Replicas and Multi-AZ
![alt text](https://github.com/mistertandon/aws-clf-co2-slides-by-stephane-maarek/blob/main/s9/185.png)

When deploying Amazon RDS databases, it's essential to select the appropriate architecture for scalability and availability. One effective option is RDS Read Replicas. These replicas distribute read traffic from your primary RDS instance, improving performance by offloading read-heavy workloads. You can create up to 15 Read Replicas, allowing applications to read from multiple instances while write operations are confined to the primary database. This setup scales read operations efficiently but does not affect write performance.

For high availability, RDS Multi-AZ deployments replicate your database across different availability zones (AZs). In this configuration, the primary database handles both read and write requests, while a standby replica in a secondary AZ is maintained for failover purposes. In the event of a failure or an AZ disruption, Amazon RDS automatically triggers a failover, promoting the standby instance to primary. The failover instance remains passive during normal operation and is only activated during an outage. Note that Multi-AZ supports a single failover replica per database.

---

## 186. RDS deployment: Multi-Region
![alt text](https://github.com/mistertandon/aws-clf-co2-slides-by-stephane-maarek/blob/main/s9/186.png)


The Multi-Region deployment option leverages Amazon RDS read replicas across distinct AWS regions to enhance availability and disaster recovery. For instance, an RDS instance in EU-West-1 can have a read replica in US-East-2, allowing applications in US-East-2 to perform read operations locally. However, write operations must be directed to the primary instance in EU-West-1. This same approach applies to other regions, such as AP-Southeast-2 in Australia.

Multi-Region deployments are crucial for business continuity. In the event of a regional failure in EU-West-1, read replicas in US-East-2 or AP-Southeast-2 ensure minimal downtime and data availability. Additionally, this configuration reduces read latency for applications by serving data from geographically closer replicas.

Keep in mind that cross-region replication introduces network data transfer costs, which should be considered during architecture planning.

---
