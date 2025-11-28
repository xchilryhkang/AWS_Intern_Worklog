---
title: "Worklog Tuần 8"
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

- Hiểu và triển khai tự động hóa tạo tài nguyên AWS bằng CloudFormation và AWS CDK.
- Quản lý cấu hình hệ thống và giám sát phiên làm việc với AWS Systems Manager.
- Biết cách kết nối các thành phần hạ tầng (EC2, Lambda, API Gateway, S3) theo mô hình Infrastructure as Code.

---

### Các công việc triển khai trong tuần

| Thứ | Hoạt động | Ngày bắt đầu | Ngày kết thúc | Tham khảo |
|-----|-----------|--------------|---------------|------------|
| 2 | Tìm hiểu AWS CloudFormation và Cloud9: cấu trúc template JSON/YAML, khái niệm Stack, Drift Detection; **Thực hành**: tạo CloudFormation template cơ bản sử dụng Cloud9 | 11/08/2025 | 11/08/2025 | |
| 3 | **Thực hành nâng cao CloudFormation**: triển khai Lambda function, tạo Stack, kết nối EC2, ánh xạ các tài nguyên với StackSets, kiểm tra Drift Detection, dọn dẹp tài nguyên | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Tìm hiểu AWS Systems Manager (SSM): Patch Manager, Run Command, Session Manager; **Thực hành**: tạo EC2 instance, gán IAM Role, cấu hình Patch Manager và Run Command, theo dõi session, dọn dẹp tài nguyên | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Tìm hiểu AWS CDK và triển khai với VS Code: tạo EC2 public, cấu hình môi trường phát triển, tạo ECS cluster, application, API Gateway + Load Balancer, Lambda, S3; triển khai Stack và Nested Stack, dọn dẹp tài nguyên | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | **Thực hành Session Manager**: tạo EC2 private/public, gán IAM Role, kết nối từ máy chủ public đến private, cập nhật IAM Role truy cập S3, tạo S3 bucket và S3 Gateway endpoint, theo dõi session logs, cấu hình Port Forwarding, dọn dẹp tài nguyên | 13/08/2025 | 13/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

### Kết quả đạt được tuần 8

Trong tuần này, em tập trung học và thực hành các giải pháp **Infrastructure as Code** và quản lý cấu hình hệ thống:

* **AWS CloudFormation & CDK**  
  - Hiểu rõ cách tạo, triển khai và quản lý Stack, Nested Stack, StackSets.  
  - Thực hành xây dựng template JSON/YAML để tự động tạo Lambda, EC2, S3, API Gateway.  
  - Áp dụng CloudFormation Drift Detection để phát hiện sự khác biệt giữa template và tài nguyên thực tế.  
  - Sử dụng AWS CDK với VS Code để triển khai hạ tầng linh hoạt, dễ bảo trì và mở rộng.

* **AWS Systems Manager (SSM)**  
  - Quản lý EC2 từ xa thông qua Session Manager, không cần SSH trực tiếp.  
  - Cấu hình Patch Manager và Run Command để tự động cập nhật, vận hành EC2.  
  - Theo dõi logs session và sử dụng Port Forwarding để truy cập EC2 Private.

* **Quản lý hạ tầng tự động**  
  - Kết nối các thành phần hạ tầng (Lambda, API Gateway, EC2, S3) theo kiến trúc IaC.  
  - Hiểu luồng triển khai, cập nhật và xóa tài nguyên một cách an toàn.  
  - Biết dọn dẹp tài nguyên sau thực hành để tối ưu chi phí và tránh dư thừa.

* **Kỹ năng bổ sung**  
  - Làm quen với Cloud9 để phát triển, chỉnh sửa template CloudFormation và CDK.  
  - Hiểu nguyên lý vận hành và giám sát các phiên làm việc EC2 private/public.  
  - Có khả năng triển khai hệ thống backend Serverless và containerized với API Gateway và Load Balancer.

Qua tuần này, em đã nâng cao kỹ năng **tự động hóa hạ tầng AWS**, hiểu cách quản lý và theo dõi hệ thống một cách hiệu quả, sẵn sàng triển khai các môi trường phức tạp hơn trong các tuần tiếp theo.

