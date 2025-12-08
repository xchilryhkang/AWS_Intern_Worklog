---
title: "APT Magic – Đề xuất dự án"
date: "2025-10-28"
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

# APT Magic  
## Nền tảng AI Serverless cho tạo ảnh cá nhân hóa và tương tác xã hội

---

### 1. Tóm tắt điều hành (Executive Summary)
**APT Magic** là một ứng dụng web AI chạy trên kiến trúc serverless, cho phép người dùng tạo, cá nhân hóa và chia sẻ nội dung nghệ thuật như hình ảnh do AI sinh ra. Nền tảng tích hợp các mô hình AI nền tảng thông qua **Amazon Bedrock** và cung cấp trải nghiệm web mượt mà với **Next.js (SSR)** được triển khai trên **AWS Amplify**.

Phiên bản **MVP** tập trung vào khả năng tạo ảnh và chia sẻ theo thời gian thực, trong khi **Thiết kế tương lai (Future Design)** hướng tới việc mở rộng với **SageMaker Inference**, **Step Functions**, và **AWS MLOps Pipelines** để điều phối mô hình và tự động hóa nâng cao.

APT Magic hiện đang được phát triển như một kiến trúc AWS-native hiện đại, tiết kiệm chi phí và bảo mật cao cho nhóm người dùng nhỏ đến trung bình, với định hướng mở rộng lên quy mô doanh nghiệp trong tương lai.

---

### 2. Vấn đề đặt ra (Problem Statement)
#### Vấn đề
Phần lớn các nền tảng tạo ảnh AI hiện nay có chi phí cao, phụ thuộc vào các API bên thứ ba thiếu minh bạch và cung cấp khả năng cá nhân hóa hạn chế.  
Các nhà phát triển và nhà sáng tạo thường gặp phải độ trễ cao, thiếu tính minh bạch trong quản lý mô hình, và hạn chế quyền kiểm soát đối với dữ liệu người dùng.

#### Giải pháp
APT Magic tận dụng **kiến trúc AWS Serverless** để cung cấp:
- Tạo ảnh AI theo thời gian thực thông qua **Amazon Bedrock (Stability AI)**.  
- Xác thực người dùng và quản lý nội dung an toàn với **Amazon Cognito** và **DynamoDB**.  
- Xử lý API linh hoạt, mở rộng với **AWS Lambda** và **API Gateway**.  
- Phân phối toàn cầu, độ trễ thấp nhờ **CloudFront CDN** và **WAF bảo mật**.  

Trong tương lai, hệ thống sẽ được nâng cấp với **Step Functions orchestration**, **SQS/SNS decoupling**, **SageMaker Inference Pipelines**, và CI/CD tiết kiệm chi phí thông qua **CodeBuild**, **CodePipeline**, và **CloudFormation**, đưa APT Magic trở thành một nền tảng **MLOps tự động hóa hoàn chỉnh**.

---

### 3. Kiến trúc giải pháp (Solution Architecture)

#### **Kiến trúc MVP**
MVP được xây dựng theo kiến trúc **serverless hoàn toàn**, tập trung vào khả năng mở rộng, dễ bảo trì và tối ưu chi phí.

**Các dịch vụ AWS cốt lõi:**
- **Route53 + CloudFront + WAF** — Truy cập toàn cầu an toàn và lưu cache.
- **Amplify (Next.js SSR)** — Lưu trữ frontend và server-side rendering.
- **API Gateway + Lambda Functions** — Xử lý backend (tạo ảnh, subscription, post API).
- **Amazon Cognito** — Xác thực người dùng và kiểm soát truy cập.
- **Amazon S3 + DynamoDB** — Lưu trữ dữ liệu và hình ảnh.
- **Amazon Bedrock** — Tích hợp mô hình AI nền tảng (Stability AI).
- **Secrets Manager, CloudWatch, CloudTrail** — Bảo mật, ghi log và giám sát.

**Bảo mật**
- **PrivateLink** giúp giao tiếp an toàn giữa Lambda và các dịch vụ backend.  
- **WAF + IAM Policies** để lọc traffic và kiểm soát truy cập theo vai trò.

![APT Magic MVP Architecture](/images/system_architecture.png)

---

#### **Thiết kế tương lai (Future Design – Kiến trúc nâng cao)**
Ở giai đoạn tiếp theo, APT Magic sẽ phát triển thành một **nền tảng điều phối AI (AI Orchestration Platform)**, bổ sung các lớp tự động hóa, khả năng chống lỗi và quản lý vòng đời mô hình.

**Các dịch vụ sẽ bổ sung:**
- **AWS Step Functions** — Điều phối các workflow bất đồng bộ như:
  - Tạo ảnh AI nhiều bước (kiểm tra prompt → inference → upload kết quả).
  - Xác nhận thanh toán → xử lý mô hình → gửi thông báo.
- **Amazon SQS** — Hàng đợi thông điệp cho các tác vụ Lambda bất đồng bộ.
- **Amazon SNS** — Gửi thông báo sự kiện theo thời gian thực.
- **Amazon ElastiCache (Redis)** — Giới hạn tốc độ và cache yêu cầu inference.
- **Amazon SageMaker Inference** — Triển khai các mô hình fine-tune và quản lý endpoint.
- **AWS CodePipeline + SageMaker Pipelines** — Tự động hóa MLOps: huấn luyện, đánh giá và triển khai.
- **AWS PrivateLink + VPC Endpoints** — Luồng dữ liệu an toàn giữa Lambda, S3 và SageMaker.
- **AWS WAF & Shield Advanced** — Bảo vệ DDoS và lọc bảo mật nâng cao.

- **CI/CD + MLOps**
  - **CodePipeline + CodeBuild + CloudFormation** cho tự động hóa triển khai hạ tầng.

![APT Magic Future Architecture](/images/aptMagic_future.png)

---

### 4. Triển khai kỹ thuật (Technical Implementation)

#### **Các giai đoạn triển khai**
**Giai đoạn 1 – Triển khai MVP (Hoàn thành / Hiện tại)**
- Triển khai Amplify (Next.js SSR) + API Gateway + Lambda.
- Tích hợp Bedrock Stability AI API.
- Triển khai CI/CD với CodePipeline + CloudFormation.
- Kích hoạt xác thực người dùng (Cognito) và lưu trữ dữ liệu (S3 + DynamoDB).

**Giai đoạn 2 – Mở rộng theo Future Design**
- Bổ sung Step Functions + SQS/SNS để quản lý workflow AI bất đồng bộ.
- Thêm ElastiCache để giới hạn request và cache.
- Tích hợp SageMaker Inference cho mô hình fine-tune.
- Triển khai SageMaker Pipelines cho huấn luyện và triển khai tự động.
- Nâng cao bảo mật với Shield Advanced + GuardDuty + PrivateLink.
- Kết nối GitLab Runner với CodeBuild cho hệ thống CI/CD thống nhất.

---

### 5. Lộ trình & Các mốc triển khai (Timeline & Milestones)

---

### 6. Ước tính chi phí (AWS Pricing Estimate)
| Dịch vụ | Chi phí ước tính / tháng | Ghi chú |
|----------|--------------------------|--------|
| Lambda + API Gateway | $0.50 | < 1 triệu lượt gọi |
| Amplify (Next.js SSR) | $0.35 | Hosting web và build |
| S3 + DynamoDB | $0.20 | Lưu trữ ảnh và metadata |
| Bedrock Inference | $3.00 | Dựa trên mức sử dụng (Stability AI) |
| ElastiCache (Tương lai) | $1.00 | Cache giới hạn tốc độ |
| Step Functions + SQS/SNS | $0.60 | Điều phối workflow |
| SageMaker Inference (Tương lai) | $5.00 | Chi phí endpoint |
| CloudWatch + WAF + Shield | $1.00 | Log và bảo mật |
| **Tổng (Ước tính)** | **~$11.65/tháng** | Tăng theo mức sử dụng |

---

### 7. Đánh giá rủi ro (Risk Assessment)
| Rủi ro | Mức độ ảnh hưởng | Xác suất | Biện pháp |
|--------|------------------|----------|-----------|
| Độ trễ khi inference AI | Trung bình | Cao | Dùng ElastiCache + Step Functions |
| Chi phí tăng do gọi mô hình | Cao | Trung bình | Kiểm soát Bedrock, autoscaling SageMaker |
| Lỗi cấu hình CI/CD | Trung bình | Thấp | CloudFormation rollback |
| Lỗ hổng bảo mật | Cao | Trung bình | WAF, GuardDuty, PrivateLink, IAM least privilege |
| Phụ thuộc API bên thứ ba | Trung bình | Trung bình | Fallback Bedrock bằng dữ liệu S3 |

---

### 8. Kết quả kỳ vọng (Expected Outcomes)
#### Kết quả kỹ thuật:
- Hoàn chỉnh quy trình tạo ảnh AI serverless với CI/CD an toàn.
- Điều phối module linh hoạt, sẵn sàng cho mở rộng MLOps.
- Giảm độ trễ và tăng độ ổn định nhờ cache và workflow bất đồng bộ.

#### Giá trị dài hạn:
- Nền tảng cho hệ sinh thái **AI as a Service (AIaaS)**.  
- Khung **MLOps tự động**, sẵn sàng huấn luyện lại mô hình.  
- Hạ tầng cloud dùng chung cho các sản phẩm AI trong tương lai.
