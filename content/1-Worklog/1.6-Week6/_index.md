---
title: "Worklog – Week 6"
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

## Learning Objectives for Week 6

- Understand relational (SQL) and non-relational (NoSQL) database services on AWS.
- Learn how to deploy, operate, and back up databases securely in the cloud environment.
- Get familiar with query acceleration mechanisms using in-memory caching with Amazon ElastiCache.
- Practice interacting with AWS databases programmatically using the Python SDK.

---

## Weekly Implementation Details

| Day | Main Activities | Start Date | End Date | References |
|-----|------------------|------------|----------|------------|
| 2 | Study the overview of Amazon RDS and Amazon Aurora; database engines such as MySQL and PostgreSQL; Multi-AZ architecture; Read Replicas mechanism; automated backup and recovery | 11/08/2025 | 11/08/2025 | |
| 3 | Hands-on practice with RDS deployment: preparing infrastructure including VPC, EC2, Security Group, and DB Subnet Group; deploying EC2 and RDS in Private Subnets; connecting EC2 to RDS; deploying applications; configuring automated backup and cleaning up resources | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Learn about Amazon DynamoDB (NoSQL): table structure, Primary Key, Sort Key, Read/Write Capacity models (On-demand, Provisioned); hands-on practice with table creation, data write/read/update/query operations; creating Global Secondary Index and querying through indexes | 13/08/2025 | 13/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Learn AWS SDK for Python including Botocore and Boto3; configure AWS CLI; use Python to interact with DynamoDB: create tables, insert, read, update, delete data, scan tables, load sample data, and remove all resources | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | Learn Amazon ElastiCache for Redis: cluster, node, shard concepts; create Access Keys and configure AWS CLI; create ElastiCache Cluster via Console and CLI; use AWS SDK to perform read/write operations with string, hash, publish/subscribe, and stream | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

## Summary of Achievements in Week 6

During the sixth week, I focused on studying and practicing with database systems and data storage services on the AWS platform. First, I researched Amazon RDS and Amazon Aurora, gaining a solid understanding of popular database engines such as MySQL and PostgreSQL, as well as how AWS ensures high availability through the Multi-AZ architecture. In addition, I learned about the Read Replicas mechanism used to improve read performance and system scalability, along with automated backup and recovery mechanisms to ensure data safety.

In the RDS hands-on session, I successfully deployed a complete system consisting of EC2 and RDS in a Private Subnet environment. I configured Security Groups and DB Subnet Groups appropriately to ensure secure communication between the application and the database. I also performed automated backups and tested data recovery procedures, helping me better understand real-world cloud database operations.

Next, I studied Amazon DynamoDB – the NoSQL database service provided by AWS. I learned about table structures, the roles of Partition Key and Sort Key, and the principles of capacity allocation under both On-demand and Provisioned modes. Through hands-on practice, I created database tables, performed write, read, update, and query operations, and built Global Secondary Indexes to optimize queries on alternative attributes.

At the same time, I became familiar with the AWS SDK for Python ecosystem, including Botocore and Boto3. I configured AWS CLI for account access and used Python scripts to interact directly with DynamoDB, such as creating tables, inserting data, querying, scanning entire tables, and deleting resources. This programming-based interaction helped me better understand how real-world applications communicate with AWS services through APIs.

In addition, I explored and practiced with Amazon ElastiCache for Redis – AWS’s distributed in-memory caching service. I created an ElastiCache Cluster, connected to it via the AWS SDK, and performed read/write operations such as setting and getting strings, working with hashes, publish/subscribe messaging, and streams. Through this process, I clearly understood the important role of caching in accelerating data access and reducing the load on primary databases.

By the end of Week 6, I had gained a comprehensive understanding of AWS database models, including relational databases, NoSQL systems, and caching services. Moreover, I developed practical skills in deployment, programming, backup, and performance optimization, which form a critical foundation for building and operating cloud-based application systems.
