---
title: "Worklog Tuần 5"
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Định hướng học tập trong tuần 5

- Tìm hiểu tổng quan về mô hình bảo mật của AWS và các nguyên tắc bảo mật cốt lõi.
- Nắm được cách quản lý danh tính, phân quyền và xác thực người dùng trên nền tảng AWS.
- Thực hành các cơ chế mã hóa, giám sát và bảo vệ dữ liệu trong môi trường cloud.

---

### Nội dung triển khai trong tuần

| Thứ | Hoạt động chính | Bắt đầu | Kết thúc | Tham khảo |
|-----|------------------|----------|-----------|------------|
| 2 | Tìm hiểu mô hình Shared Responsibility Model, trách nhiệm giữa AWS và khách hàng; nghiên cứu tổng quan về Amazon IAM gồm Root Account, IAM User, IAM Group, IAM Policy, IAM Role và Permission Boundary | 11/08/2025 | 11/08/2025 | |
| 3 | Thực hành tạo IAM Group, IAM User, IAM Role và Assume Role; cấu hình người dùng quản trị EC2, RDS; thiết lập điều kiện Role theo IP, thời gian; tạo policy giới hạn quyền và kiểm thử tài khoản bị giới hạn | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Tìm hiểu Tag và AWS Resource Groups; thực hành gắn Tag cho EC2 bằng Console và CLI; tạo Resource Group; kiểm soát truy cập EC2 dựa trên Tag thông qua IAM Policy và kiểm thử các trường hợp bị từ chối truy cập | 13/08/2025 | 13/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Tìm hiểu Amazon Cognito, AWS Organizations, AWS Identity Center (SSO), AWS KMS và AWS Security Hub; kích hoạt Security Hub và đánh giá các bộ tiêu chuẩn bảo mật | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | Thực hành AWS SSO với mô hình multi-account; tạo OU trong AWS Organizations; mã hóa dữ liệu với AWS KMS; upload dữ liệu mã hóa lên S3; bật CloudTrail và sử dụng Athena truy vấn log; kiểm thử chia sẻ dữ liệu mã hóa | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

### Tổng hợp kết quả đạt được trong tuần 5

Trong tuần thứ năm, em tập trung tìm hiểu sâu về hệ thống bảo mật và quản lý danh tính trên nền tảng AWS. Trước hết, em đã nắm vững mô hình chia sẻ trách nhiệm (Shared Responsibility Model), trong đó AWS chịu trách nhiệm bảo mật hạ tầng vật lý, phần cứng và các dịch vụ nền tảng, còn khách hàng chịu trách nhiệm cấu hình bảo mật dữ liệu, ứng dụng, phân quyền truy cập và các cơ chế mã hóa. Điều này giúp em hiểu rõ ranh giới trách nhiệm khi vận hành hệ thống trên môi trường cloud.

Tiếp theo, em nghiên cứu chi tiết dịch vụ Amazon Identity and Access Management (IAM). Em đã nắm được các khái niệm cốt lõi như Root Account, IAM User, IAM Group, IAM Policy, IAM Role và Permission Boundary. Thông qua quá trình thực hành, em đã tạo nhiều nhóm người dùng, cấu hình tài khoản quản trị cho từng dịch vụ như EC2, RDS, đồng thời áp dụng nguyên tắc phân quyền tối thiểu (least privilege) để hạn chế rủi ro bảo mật. Ngoài ra, em cũng thực hiện cấu hình Assume Role, giới hạn theo IP và thời gian truy cập, từ đó kiểm thử các kịch bản truy cập bị từ chối khi không thỏa điều kiện bảo mật.

Bên cạnh IAM, em đã tìm hiểu và thực hành sử dụng Tag để quản lý tài nguyên và kiểm soát quyền truy cập. Em gắn Tag cho các tài nguyên EC2 thông qua cả Console và CLI, tạo Resource Groups để gom nhóm tài nguyên theo thẻ, sau đó thiết lập IAM Policy cho phép hoặc từ chối truy cập dựa trên giá trị Tag và Region. Việc kiểm thử các trường hợp bị deny do sai Region, sai Tag hoặc không thỏa điều kiện giúp em hiểu rõ hơn cách AWS kiểm soát truy cập ở mức tài nguyên.

Trong phần quản lý người dùng ứng dụng, em tìm hiểu dịch vụ Amazon Cognito, bao gồm User Pool để quản lý tài khoản và xác thực đăng nhập, cùng Identity Pool để cấp quyền truy cập tạm thời vào các dịch vụ AWS. Đồng thời, em cũng nghiên cứu mô hình vận hành đa tài khoản thông qua AWS Organizations và AWS Identity Center (SSO). Em đã thực hành tạo Organizational Unit (OU), phân tách môi trường, thiết lập đăng nhập tập trung bằng SSO, từ đó hiểu rõ cách quản lý tập trung trong hệ thống multi-account.

Về bảo mật dữ liệu, em đã học cách sử dụng AWS Key Management Service (KMS) để tạo và quản lý khóa mã hóa. Em áp dụng mã hóa cho dữ liệu lưu trữ trong Amazon S3, sau đó kiểm thử việc upload, truy cập và chia sẻ dữ liệu đã được mã hóa thông qua các quyền được cấp bởi IAM và Role. Đồng thời, em bật AWS CloudTrail để ghi lại toàn bộ hoạt động của tài khoản và sử dụng Amazon Athena để truy vấn log phục vụ công tác giám sát và kiểm tra an ninh.

Ngoài ra, em cũng kích hoạt và sử dụng AWS Security Hub để tổng hợp, đánh giá các tiêu chuẩn bảo mật mặc định. Thông qua các báo cáo và cảnh báo, em hiểu được các lỗi cấu hình phổ biến cũng như cách cải thiện mức độ an toàn của hệ thống.

Thông qua các nội dung thực hiện trong tuần 5, em đã có cái nhìn toàn diện về hệ sinh thái bảo mật của AWS, từ quản lý danh tính, phân quyền truy cập, kiểm soát tài nguyên bằng Tag, đến mã hóa dữ liệu, giám sát hoạt động và đánh giá tiêu chuẩn bảo mật. Đây là nền tảng quan trọng để triển khai các hệ thống cloud an toàn và đáp ứng yêu cầu vận hành thực tế.
