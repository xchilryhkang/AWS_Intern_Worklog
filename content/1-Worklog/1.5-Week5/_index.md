---
title: "Worklog – Week 5"
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

## Study Orientation for Week 5

- Gain an overview of the AWS security model and its core security principles.
- Understand identity management, authorization, and authentication mechanisms on the AWS platform.
- Practice encryption, monitoring, and data protection mechanisms in the cloud environment.

---

## Weekly Activities

| Day | Main Activities | Start Date | End Date | References |
|-----|------------------|------------|-----------|-------------|
| 2 | Study the Shared Responsibility Model and the division of responsibilities between AWS and customers; research an overview of Amazon IAM including Root Account, IAM User, IAM Group, IAM Policy, IAM Role, and Permission Boundary | 11/08/2025 | 11/08/2025 | |
| 3 | Practice creating IAM Groups, IAM Users, IAM Roles, and Assume Roles; configure administrative users for EC2 and RDS; apply role conditions based on IP and access time; create restrictive policies and test access denial scenarios | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Study Tags and AWS Resource Groups; practice tagging EC2 instances via both Console and CLI; create Resource Groups; control EC2 access based on Tags using IAM Policies and test access denial scenarios | 13/08/2025 | 13/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Learn about Amazon Cognito, AWS Organizations, AWS Identity Center (SSO), AWS KMS, and AWS Security Hub; activate Security Hub and evaluate built-in security standards | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | Practice AWS SSO in a multi-account model; create Organizational Units (OU) in AWS Organizations; encrypt data using AWS KMS; upload encrypted data to S3; enable CloudTrail and use Athena to query logs; test encrypted data sharing | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

## Summary of Achievements in Week 5

During the fifth week, I focused on gaining in-depth knowledge of security architecture and identity management on the AWS platform. First, I fully understood the Shared Responsibility Model, in which AWS is responsible for securing the physical infrastructure, hardware, and foundational services, while customers are responsible for securing data, applications, access control, and encryption configurations. This helped me clearly distinguish the boundaries of responsibility when operating systems in the cloud environment.

Next, I conducted a detailed study of Amazon Identity and Access Management (IAM). I gained a strong understanding of core concepts such as Root Account, IAM Users, IAM Groups, IAM Policies, IAM Roles, and Permission Boundaries. Through hands-on practice, I created multiple user groups, configured administrative accounts for services such as EC2 and RDS, and applied the principle of least privilege to minimize security risks. In addition, I configured Assume Roles with restrictions based on IP addresses and access time, and conducted testing on access-denied scenarios when security conditions were not satisfied.

Alongside IAM, I studied and practiced using Tags for both resource management and access control. I attached Tags to EC2 resources using both the AWS Management Console and AWS CLI, created Resource Groups to organize resources by tags, and defined IAM Policies to allow or deny access based on Tag values and Regions. Testing scenarios involving denied access due to incorrect Region, incorrect Tags, or unmet conditions helped me better understand how AWS enforces fine-grained access control at the resource level.

In application user management, I explored Amazon Cognito, including User Pools for account management and authentication, and Identity Pools for granting temporary access to AWS services. At the same time, I studied multi-account operations using AWS Organizations and AWS Identity Center (SSO). I practiced creating Organizational Units (OUs), separating environments, and configuring centralized authentication via SSO, which helped me understand centralized identity management in multi-account architectures.

Regarding data security, I learned how to use AWS Key Management Service (KMS) to create and manage encryption keys. I applied encryption to data stored in Amazon S3, then tested uploading, accessing, and sharing encrypted data through permissions granted by IAM and Roles. In parallel, I enabled AWS CloudTrail to log all account activities and used Amazon Athena to query logs for monitoring and security auditing purposes.

In addition, I activated and used AWS Security Hub to aggregate and evaluate default security standards. Through security reports and alerts, I gained insights into common misconfigurations and learned how to improve the overall security posture of the system.

Through the activities completed in Week 5, I developed a comprehensive understanding of the AWS security ecosystem, from identity management, access control, and resource tagging to data encryption, activity monitoring, and security compliance evaluation. This knowledge forms a critical foundation for deploying secure and production-ready cloud systems in real-world environments.
