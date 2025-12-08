---
title: "Worklog Tuần 12"
weight: 2
chapter: false
pre: " <b> 1.12 </b> "
---

### Mục tiêu tuần 12:

* Hệ thống lại toàn bộ kiến thức về Serverless và AI.
* Thiết kế chi tiết cơ sở dữ liệu DynamoDB phục vụ cho dự án và hệ thống API.
* Rà soát lại toàn bộ luồng kết nối giữa các dịch vụ trong hệ thống.

---

### Các công việc triển khai trong tuần:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
|-----|-----------|---------------|------------------|----------------|
| 2 | - Ôn tập kiến thức và thiết kế cơ sở dữ liệu DynamoDB <br>&emsp; + Rà soát lại Partition Key (PK) và Sort Key (SK) <br> - **Thực hành:** <br>&emsp; + Thiết kế Schema cho các bảng dữ liệu của dự án <br>&emsp; + Xác định các Access Pattern (cách truy vấn dữ liệu) | 24/11/2025 | 24/11/2025 | https://cloudjourney.awsstudygroup.com/ |
| 3 | - Ôn tập và thiết kế hệ thống API (API Gateway + Lambda): <br>&emsp; + Rà soát cách triển khai REST API và Lambda Proxy Integration <br>&emsp; + Liệt kê danh sách các API endpoint cần thiết như POST, GET | 25/11/2025 | 25/11/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | - Ôn tập lại quy trình tích hợp AI với Amazon Bedrock <br>&emsp; + Rà soát các phương thức gọi API của Bedrock <br>&emsp; + Ôn tập các kỹ thuật Prompt Engineering cơ bản | 26/11/2025 | 26/11/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | - Ôn tập về bảo mật và xác thực (Cognito + IAM): <br>&emsp; + Rà soát luồng xác thực: Người dùng đăng nhập → Nhận Token → Gửi Token lên API Gateway <br>&emsp; + Ôn lại cách xây dựng IAM Policy theo nguyên tắc cấp quyền tối thiểu | 27/11/2025 | 27/11/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | - Ôn tập công tác giám sát và vận hành hệ thống <br>&emsp; + Rà soát CloudWatch để lên phương án giám sát khi triển khai dự án <br>&emsp; + Ôn tập cách sử dụng thư viện Boto3 <br>&emsp; + Lập kế hoạch chi tiết các bước triển khai dự án | 28/11/2025 | 28/11/2025 | https://cloudjourney.awsstudygroup.com/ |

---

### Kết quả đạt được trong tuần 12:

* Hoàn thiện thiết kế Schema cho DynamoDB:
  * Xây dựng cấu trúc bảng dữ liệu rõ ràng, tối ưu cho các nhu cầu truy vấn của hệ thống.

* Xác định đầy đủ giao diện kết nối giữa các thành phần:
  * Định nghĩa rõ ràng input và output cho các hàm Lambda.
  * Nắm vững cách sử dụng thư viện Boto3 để liên kết các dịch vụ AWS trong hệ thống.

* Xây dựng sẵn chiến lược Prompt (Prompt Strategy) nhằm phục vụ việc kiểm thử và triển khai AI với Bedrock đúng theo yêu cầu.

* Hiểu rõ luồng xử lý Identity (danh tính người dùng) từ Cognito qua API Gateway và xuống Lambda.
