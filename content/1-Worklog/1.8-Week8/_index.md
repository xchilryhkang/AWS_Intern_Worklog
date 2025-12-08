---
title: "Worklog – Week 8"
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

## Objectives of Week 8

- Understand and implement automated AWS resource provisioning using CloudFormation and AWS CDK.
- Manage system configurations and monitor sessions using AWS Systems Manager.
- Learn how to connect infrastructure components (EC2, Lambda, API Gateway, S3) using the Infrastructure as Code (IaC) approach.

---

## Weekly Implementation Details

| Day | Activities | Start Date | End Date | References |
|-----|------------|------------|----------|------------|
| 2 | Learn AWS CloudFormation and Cloud9: template structure in JSON/YAML, Stack concept, and Drift Detection; **Practice**: create a basic CloudFormation template using Cloud9 | 11/08/2025 | 11/08/2025 | |
| 3 | **Advanced CloudFormation Practice**: deploy Lambda functions, create Stacks, connect EC2 resources, map resources using StackSets, perform Drift Detection checks, and clean up resources | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Learn AWS Systems Manager (SSM): Patch Manager, Run Command, Session Manager; **Practice**: create EC2 instances, attach IAM Roles, configure Patch Manager and Run Command, monitor sessions, and clean up resources | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Learn AWS CDK with VS Code: deploy public EC2, configure development environment, create ECS cluster and application, API Gateway + Load Balancer, Lambda, and S3; deploy Stack and Nested Stack, and clean up resources | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | **Session Manager Practice**: create private and public EC2 instances, attach IAM Roles, connect from public to private instances, update IAM Roles for S3 access, create S3 buckets and S3 Gateway Endpoints, monitor session logs, configure Port Forwarding, and clean up resources | 13/08/2025 | 13/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

## Summary of Achievements in Week 8

During this week, I focused on studying and practicing **Infrastructure as Code (IaC)** solutions and system configuration management:

### **AWS CloudFormation & AWS CDK**
- Gained a solid understanding of how to create, deploy, and manage Stacks, Nested Stacks, and StackSets.
- Practiced building JSON/YAML templates to automatically provision Lambda, EC2, S3, and API Gateway resources.
- Applied CloudFormation Drift Detection to identify differences between templates and actual deployed resources.
- Used AWS CDK with VS Code to deploy infrastructure in a more flexible, maintainable, and scalable manner.

### **AWS Systems Manager (SSM)**
- Managed EC2 instances remotely using Session Manager without direct SSH access.
- Configured Patch Manager and Run Command to automate system updates and EC2 operations.
- Monitored session logs and used Port Forwarding to securely access private EC2 instances.

### **Automated Infrastructure Management**
- Connected infrastructure components (Lambda, API Gateway, EC2, S3) using the IaC architecture.
- Understood safe workflows for deploying, updating, and deleting resources.
- Practiced cleaning up resources after labs to optimize costs and avoid unnecessary charges.

### **Additional Skills**
- Became familiar with Cloud9 for developing and editing CloudFormation and CDK templates.
- Understood the principles of monitoring and managing private/public EC2 sessions.
- Gained hands-on experience in deploying Serverless and containerized backend systems using API Gateway and Load Balancer.

Through the activities in Week 8, I significantly strengthened my skills in **automating AWS infrastructure**, system management, and monitoring, providing a strong foundation for deploying more complex cloud environments in subsequent weeks.
