---
title: "Worklog – Week 4"
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

## Study Orientation for Week 4

- Explore AWS data storage services, with a primary focus on Amazon S3 and hybrid storage solutions.
- Understand backup, recovery, and disaster recovery strategies for system protection.
- Practice deploying highly available, secure, and scalable storage architectures.

---

## Weekly Activities

| Day | Main Activities | Start Date | End Date | References |
|-----|------------------|------------|-----------|-------------|
| 2 | Study Amazon S3 in detail: buckets, objects, access points, storage classes, versioning, CORS, access control, static website hosting, CloudFront integration, replication, and performance optimization; practice creating buckets, uploading data, deploying static websites, and replicating data across regions | 11/08/2025 | 11/08/2025 | |
| 3 | Study the architecture of AWS Backup, design backup plans, configure SNS notifications; practice creating Backup Plans, monitoring backup activities, and testing data recovery | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Study the Snow Family, Storage Gateway (File, Volume, and Tape Gateway), and Disaster Recovery concepts (RTO, RPO); practice creating a File Gateway, sharing data, and connecting with on-premise environments | 13/08/2025 | 13/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Study AWS Import/Export; practice importing virtual machines from VMware to AWS and exporting EC2 instances from AWS to on-premise environments | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | Study Amazon FSx; practice deploying Multi-AZ file server systems with SSD and HDD, performance testing, monitoring, snapshot configuration, capacity scaling, and throughput optimization | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

## Summary of Achievements in Week 4

During the fourth week, I focused on studying AWS storage solutions as well as backup and recovery mechanisms to ensure system safety and reliability.

First, I gained a solid understanding of how Amazon S3 works, including bucket and object structures, access points, and access control mechanisms using ACLs, bucket policies, CORS, and versioning. I successfully practiced creating S3 buckets, uploading data, deploying static websites directly on S3, and integrating CloudFront to accelerate content delivery. In addition, I implemented cross-region replication to enhance data availability and durability.

Alongside S3, I explored hybrid storage solutions through AWS Storage Gateway, including File Gateway, Volume Gateway, and Tape Gateway. Connecting on-premise file shares to AWS helped me better understand real-world hybrid storage architectures. I also studied the Snow Family and common enterprise use cases for large-scale data transfer.

Regarding backup and recovery, I researched the architecture of AWS Backup, the process of building Backup Plans, the role of Backup Vaults, and recovery workflows. I successfully configured automated backup systems, integrated SNS notifications for monitoring, and tested data restoration procedures. At the same time, I gained a clear understanding of Disaster Recovery strategies such as RTO, RPO, Pilot Light, Warm Standby, and Active-Active to ensure continuous system operation during failures.

For file-based storage systems, I practiced deploying Amazon FSx by building Multi-AZ architectures with both SSD and HDD storage. I created file shares, monitored performance, enabled data deduplication and shadow copy mechanisms, and managed user sessions. In addition, I performed storage capacity and throughput scaling to meet increasing usage demands.

Furthermore, I practiced the Import/Export process between on-premise environments and AWS. Specifically, I exported virtual machines from VMware, uploaded them to S3, imported them as AMIs, and launched EC2 instances. Conversely, I also exported EC2 instances back to the local virtualization environment.

Through the activities completed in Week 4, I gained a comprehensive understanding of AWS storage, backup, recovery, and disaster recovery solutions. This knowledge serves as a critical foundation for designing highly available, secure, and scalable real-world cloud systems.
