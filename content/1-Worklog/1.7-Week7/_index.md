---
title: "Worklog – Week 7"
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

## Learning Objectives for Week 7

- Get familiar with the Serverless architecture using AWS Lambda and Amazon API Gateway.
- Understand the working principles of Event-Driven systems on the AWS platform.
- Learn how to build asynchronous processing systems using Amazon SQS and SNS.
- Practice building APIs that connect Lambda with DynamoDB and S3 for data processing.

---

## Weekly Implementation Details

| Day | Main Activities | Start Date | End Date | References |
|-----|------------------|------------|----------|------------|
| 2 | Study AWS Lambda: function concepts and permission management using IAM Roles; learn Amazon API Gateway including HTTP methods and CORS mechanism; practice creating IAM Roles for Lambda, building Lambda functions for file upload processing, configuring API Gateway to trigger Lambda, and storing data in DynamoDB | 11/08/2025 | 11/08/2025 | |
| 3 | Practice integrating Lambda with S3 and DynamoDB: building image processing Lambda functions, creating S3 Buckets, configuring IAM Policies for Lambda, creating and managing DynamoDB tables, building data-write Lambda functions, and cleaning up resources | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Practice deploying a static website with S3: creating buckets, enabling static hosting, attaching bucket policies, and uploading frontend files; building a CRUD system with DynamoDB and Lambda, configuring API Gateway, testing APIs using Postman and frontend, and cleaning up resources | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Learn Event-Driven architecture with Amazon SQS and SNS: publish/subscribe model and message queue principles; practice creating SQS Queues and SNS Topics, building Lambda and APIs to interact with SQS and SNS, and testing system operations | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | Learn AWS Step Functions and their role in orchestrating microservices in Serverless systems | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

## Summary of Achievements in Week 7

During the seventh week, I focused on studying and practicing Serverless and Event-Driven architecture models on the AWS platform. First, I explored how AWS Lambda works, gaining an understanding of how serverless functions are deployed without the need to manage servers, as well as the role of IAM Roles in granting resource access to Lambda functions based on the principle of least privilege.

At the same time, I learned about Amazon API Gateway, including how to build RESTful APIs, use HTTP methods, and configure CORS to allow secure access from frontend applications. Through hands-on practice, I successfully built a system where API Gateway acted as the entry point, triggering Lambda functions to process requests and store data in DynamoDB.

Next, I practiced integrating Lambda with Amazon S3 and DynamoDB. I built Lambda functions to handle file uploads to S3 while storing metadata in DynamoDB. Through this workflow, I gained a clearer understanding of how to build a complete serverless backend system with three core components: API Gateway – Lambda – DynamoDB.

In addition, I successfully deployed a static website using Amazon S3, where the frontend interacted with backend APIs via API Gateway to perform create, read, update, and delete (CRUD) operations on data. Testing through Postman and directly on the web interface helped me better understand real-world request processing flows.

Alongside Serverless architecture, I continued learning the Event-Driven model using Amazon SQS and SNS. I created SQS Queues and SNS Topics, built Lambda functions to process messages from queues, and practiced publish/subscribe mechanisms to simulate asynchronous processing systems. This helped me understand the role of message queues in decoupling system components, improving reliability, and enhancing scalability.

Toward the end of the week, I gained an overview of AWS Step Functions and their capability to orchestrate Lambda functions within microservices systems according to logical execution flows. Through this week’s learning activities, I established a solid foundation in Serverless and Event-Driven architectures, as well as modern backend system development on AWS with scalability, cost efficiency, and maintainability.
