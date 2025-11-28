---
title: "Worklog Tuần 10"
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:

- Hiểu và triển khai giám sát hệ thống với **Amazon CloudWatch**.  
- Nắm được cách AWS **CloudTrail** ghi lại hoạt động API và quản lý log theo thời gian thực.  
- Biết cách giám sát ứng dụng serverless và frontend/backend với **AWS Amplify**.  

---

### Các công việc cần triển khai

| Thứ | Hoạt động | Ngày bắt đầu | Ngày kết thúc | Tham khảo |
|-----|-----------|--------------|---------------|------------|
| 2 | Tìm hiểu Amazon CloudWatch: Metrics, Logs, Alarms, Events, Dashboards, AWS X-Ray | 11/08/2025 | 11/08/2025 | |
| 3 | **Thực hành CloudWatch:** tạo IAM Role & Policy, cấu hình EC2, cài đặt CloudWatch Metrics & Logs, tạo Alarm, tạo Dashboard, dọn dẹp tài nguyên | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Tìm hiểu AWS CloudTrail: Trails, Event (Read/Write/All), CloudTrail Insights | 13/08/2025 | 13/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Tìm hiểu AWS Amplify: Frontend, Backend, Storage, Authentication | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | **Thực hành:** Giám sát Lambda với CloudWatch & X-Ray, host source code trên Amplify, tạo custom metric, Alarm, gỡ lỗi logs, giám sát với X-Ray, dọn dẹp tài nguyên | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

### Kết quả đạt được tuần 10

Trong tuần này, em tập trung vào **giám sát hệ thống và quản lý hoạt động trên AWS**, kết hợp thực hành với các dịch vụ CloudWatch, CloudTrail và Amplify:

* **Amazon CloudWatch**  
  - Hiểu và sử dụng **Metrics** để giám sát tài nguyên EC2, Lambda, DynamoDB.  
  - Thiết lập **Logs** để theo dõi chi tiết các hoạt động ứng dụng và hạ tầng.  
  - Tạo **Alarms** để cảnh báo khi có sự cố hoặc vượt ngưỡng định sẵn.  
  - Thiết kế **Dashboard** tổng quan theo dõi các tài nguyên AWS.  
  - Sử dụng **X-Ray** để debug và phân tích hiệu suất của Lambda và API Gateway.

* **AWS CloudTrail**  
  - Tìm hiểu cách ghi lại toàn bộ API call, theo dõi Read/Write events.  
  - Sử dụng CloudTrail Insights để phát hiện hành vi bất thường trong hệ thống.  
  - Kết hợp với CloudWatch để lập alert và tự động hóa phản hồi khi có sự kiện quan trọng.

* **AWS Amplify**  
  - Host frontend/backend ứng dụng nhanh chóng.  
  - Triển khai authentication và storage để tích hợp với Lambda và DynamoDB.  
  - Giám sát hoạt động ứng dụng thông qua CloudWatch Logs và X-Ray.  

* **Kỹ năng bổ sung**  
  - Quản lý IAM Role & Policy để bảo mật và phân quyền đúng mức.  
  - Kết hợp CLI và Console để quản lý đồng thời các tài nguyên AWS.  
  - Lập kế hoạch cleanup tài nguyên sau thực hành để tối ưu chi phí.  

Qua tuần này, em đã có khả năng **giám sát hệ thống AWS theo thời gian thực, debug ứng dụng serverless, tạo cảnh báo và dashboard**, đồng thời quản lý tài nguyên frontend/backend với Amplify một cách hiệu quả.

