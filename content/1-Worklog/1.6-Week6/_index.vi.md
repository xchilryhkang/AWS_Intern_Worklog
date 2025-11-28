---
title: "Worklog Tuần 6"
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

### Định hướng học tập trong tuần 6

- Tìm hiểu các dịch vụ cơ sở dữ liệu quan hệ (SQL) và phi quan hệ (NoSQL) trên nền tảng AWS.
- Biết cách triển khai, vận hành và sao lưu dữ liệu an toàn trong môi trường cloud.
- Làm quen với các cơ chế tăng tốc truy vấn bằng bộ nhớ đệm (cache) thông qua Amazon ElastiCache.
- Thực hành lập trình tương tác với cơ sở dữ liệu AWS thông qua Python SDK.

---

### Nội dung triển khai trong tuần

| Thứ | Hoạt động chính | Bắt đầu | Kết thúc | Tham khảo |
|-----|------------------|----------|-----------|------------|
| 2 | Tìm hiểu tổng quan về Amazon RDS và Amazon Aurora; các hệ quản trị cơ sở dữ liệu như MySQL, PostgreSQL; kiến trúc Multi-AZ; cơ chế Read Replicas; sao lưu và khôi phục dữ liệu tự động | 11/08/2025 | 11/08/2025 | |
| 3 | Thực hành triển khai hệ thống RDS: chuẩn bị hạ tầng gồm VPC, EC2, Security Group và DB Subnet Group; triển khai EC2 và RDS trong Private Subnet; kết nối EC2 với RDS; triển khai ứng dụng; cấu hình sao lưu tự động và dọn dẹp tài nguyên | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Tìm hiểu Amazon DynamoDB (NoSQL): cấu trúc bảng, Primary Key, Sort Key, mô hình Read/Write Capacity (On-demand, Provisioned); thực hành tạo bảng, ghi – đọc – cập nhật – truy vấn dữ liệu, tạo Global Secondary Index và truy vấn dữ liệu qua index | 13/08/2025 | 13/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Tìm hiểu AWS SDK cho Python gồm Botocore và Boto3; cấu hình AWS CLI; sử dụng Python thao tác với DynamoDB: tạo bảng, ghi, đọc, cập nhật, xóa dữ liệu, quét bảng, tải dữ liệu mẫu và xóa toàn bộ tài nguyên | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | Tìm hiểu Amazon ElastiCache for Redis: cluster, node, shard; tạo Access Key cấu hình AWS CLI; tạo ElastiCache Cluster qua Console và CLI; sử dụng AWS SDK để đọc – ghi dữ liệu: string, hash, publish/subscribe và stream | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

### Tổng hợp kết quả đạt được trong tuần 6

Trong tuần thứ sáu, em tập trung tìm hiểu và thực hành về hệ thống cơ sở dữ liệu và các dịch vụ lưu trữ, xử lý dữ liệu trên nền tảng AWS. Trước tiên, em đã nghiên cứu dịch vụ Amazon RDS và Aurora, hiểu rõ đặc điểm của các engine cơ sở dữ liệu phổ biến như MySQL và PostgreSQL, cũng như cách AWS đảm bảo tính sẵn sàng cao thông qua kiến trúc Multi-AZ. Bên cạnh đó, em cũng nắm được cơ chế Read Replicas nhằm tăng hiệu năng đọc và khả năng mở rộng hệ thống, cùng với cơ chế sao lưu và khôi phục dữ liệu tự động để đảm bảo an toàn dữ liệu.

Trong phần thực hành RDS, em đã triển khai hoàn chỉnh một hệ thống bao gồm EC2 và RDS trong môi trường Private Subnet. Em cấu hình Security Group và DB Subnet Group phù hợp để đảm bảo kết nối giữa ứng dụng và cơ sở dữ liệu diễn ra an toàn. Em cũng thực hiện backup tự động và kiểm thử khôi phục dữ liệu, qua đó hiểu rõ hơn quy trình vận hành thực tế của một hệ quản trị cơ sở dữ liệu trên cloud.

Tiếp theo, em tìm hiểu về Amazon DynamoDB – dịch vụ cơ sở dữ liệu NoSQL của AWS. Em nắm được cấu trúc bảng, vai trò của Partition Key và Sort Key, cũng như nguyên lý phân bổ dung lượng Read/Write theo hai chế độ On-demand và Provisioned. Trong quá trình thực hành, em đã tạo bảng dữ liệu, thực hiện các thao tác ghi, đọc, cập nhật, truy vấn dữ liệu, đồng thời xây dựng Global Secondary Index để tối ưu truy vấn theo các trường dữ liệu khác nhau.

Song song với đó, em cũng làm quen với hệ sinh thái AWS SDK cho Python, bao gồm Botocore và Boto3. Em cấu hình AWS CLI để kết nối với tài khoản và sử dụng Python để lập trình thao tác trực tiếp với DynamoDB như tạo bảng, thêm dữ liệu, truy vấn, quét toàn bộ bảng và xóa dữ liệu. Việc lập trình tự động giúp em hiểu sâu hơn cách các ứng dụng thực tế làm việc với dịch vụ AWS thông qua API.

Ngoài ra, em còn tìm hiểu và thực hành với Amazon ElastiCache for Redis – dịch vụ bộ nhớ đệm phân tán của AWS. Em đã tạo ElastiCache Cluster, kết nối thông qua AWS SDK và thực hiện các thao tác đọc – ghi dữ liệu như set/get string, set/get hash, publish/subscribe và làm việc với stream. Thông qua đó, em hiểu được vai trò quan trọng của cache trong việc tăng tốc truy xuất dữ liệu và giảm tải cho hệ thống cơ sở dữ liệu chính.

Kết thúc tuần học, em đã có cái nhìn tương đối toàn diện về các mô hình cơ sở dữ liệu trên AWS, từ cơ sở dữ liệu quan hệ, NoSQL đến hệ thống cache. Đồng thời, em cũng nắm được cách triển khai, lập trình, sao lưu và tối ưu hiệu năng dữ liệu – đây là nền tảng quan trọng cho việc xây dựng và vận hành các hệ thống ứng dụng trên môi trường cloud.

