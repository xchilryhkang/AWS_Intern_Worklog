---
title: "Week 12 Worklog"
weight: 2
chapter: false
pre: " <b> 1.12 </b> "
---

### Week 12 Objectives:

* Review and consolidate knowledge of Serverless architecture and AI services.
* Design a detailed DynamoDB database schema for the project and its APIs.
* Thoroughly examine and validate the integration flow among system services.

---

### Tasks Implemented During the Week:

| Day | Tasks | Start Date | Completion Date | Reference |
|-----|--------|-------------|------------------|------------|
| 2 | - Review and design the DynamoDB database <br>&emsp; + Revisit Partition Key (PK) and Sort Key (SK) concepts <br> - **Hands-on:** <br>&emsp; + Design schemas for project tables <br>&emsp; + Define access patterns (data query strategies) | 24/11/2025 | 24/11/2025 | https://cloudjourney.awsstudygroup.com/ |
| 3 | - Review and design the API layer (API Gateway + Lambda): <br>&emsp; + Revisit REST API creation and Lambda Proxy Integration <br>&emsp; + List required API endpoints such as POST and GET | 25/11/2025 | 25/11/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | - Review the AI integration workflow with Amazon Bedrock <br>&emsp; + Revisit Bedrock API invocation methods <br>&emsp; + Review fundamental Prompt Engineering techniques | 26/11/2025 | 26/11/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | - Review security and authentication mechanisms (Amazon Cognito + IAM): <br>&emsp; + Revisit the authentication flow: User login → Token issuance → Token submission to API Gateway <br>&emsp; + Review IAM policies based on the principle of least privilege | 27/11/2025 | 27/11/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | - Review system monitoring and operational practices <br>&emsp; + Revisit CloudWatch for planning runtime monitoring <br>&emsp; + Review the use of Boto3 SDK <br>&emsp; + Prepare a detailed project deployment plan | 28/11/2025 | 28/11/2025 | https://cloudjourney.awsstudygroup.com/ |

---

### Week 12 Achievements:

* Finalized the DynamoDB schema design:
  * Built a well-structured data model optimized for efficient data access.

* Clearly defined service interfaces:
  * Specified clear input and output formats for Lambda functions.
  * Gained strong proficiency in using the Boto3 library to interconnect AWS services.

* Prepared a prompt strategy for AI testing and validation with Amazon Bedrock.

* Developed a clear understanding of the identity and authentication flow from Amazon Cognito through API Gateway to AWS Lambda.
