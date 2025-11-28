---
title: "Worklog Tuần 4"
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Định hướng học tập trong tuần 4

- Tìm hiểu các dịch vụ lưu trữ dữ liệu trên AWS, đặc biệt là S3 và các giải pháp lưu trữ lai (hybrid).
- Nắm được các cơ chế sao lưu, khôi phục và chiến lược phòng chống thảm họa cho hệ thống.
- Thực hành triển khai các mô hình lưu trữ có tính sẵn sàng cao, an toàn và dễ mở rộng.

---

### Nội dung triển khai trong tuần

| Thứ | Hoạt động chính | Bắt đầu | Kết thúc | Tham khảo |
|-----|------------------|----------|-----------|------------|
| 2 | Tìm hiểu chi tiết về Amazon S3: bucket, object, access point, các lớp lưu trữ, versioning, CORS, control access, static website, CloudFront, replication và tối ưu hiệu năng; thực hành tạo bucket, upload dữ liệu, triển khai static website và sao chép dữ liệu giữa các region | 11/08/2025 | 11/08/2025 | |
| 3 | Tìm hiểu kiến trúc AWS Backup, xây dựng kế hoạch sao lưu, thiết lập thông báo qua SNS; thực hành tạo Backup Plan, theo dõi hoạt động backup và kiểm thử khả năng khôi phục | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Tìm hiểu Snow Family, Storage Gateway (File, Volume, Tape Gateway) và các khái niệm Disaster Recovery (RTO, RPO); thực hành tạo File Gateway, chia sẻ dữ liệu và kết nối với môi trường on-premise | 13/08/2025 | 13/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Tìm hiểu AWS Import/Export; thực hành import máy ảo từ VMware lên AWS và export EC2 từ AWS về môi trường on-premise | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | Tìm hiểu dịch vụ Amazon FSx; thực hành triển khai hệ thống file server Multi-AZ với SSD và HDD, kiểm tra hiệu năng, giám sát, cấu hình snapshot, scale dung lượng và throughput | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

### Tổng hợp kết quả đạt được trong tuần 4

Trong tuần thứ tư, em tập trung tìm hiểu các giải pháp lưu trữ dữ liệu trên AWS cũng như các cơ chế sao lưu và khôi phục nhằm đảm bảo an toàn cho hệ thống.

Trước hết, em đã nắm được cách hoạt động của Amazon S3, bao gồm cấu trúc bucket, object, access point cùng các cơ chế kiểm soát truy cập thông qua ACL, policy, CORS và versioning. Em thực hành tạo bucket, upload dữ liệu, triển khai website tĩnh trực tiếp trên S3, đồng thời tích hợp CloudFront để tăng tốc phân phối nội dung. Ngoài ra, em cũng thực hiện sao chép dữ liệu giữa các region nhằm nâng cao khả năng sẵn sàng.

Bên cạnh S3, em đã tìm hiểu các giải pháp lưu trữ kết hợp giữa on-premise và AWS thông qua Storage Gateway, bao gồm File Gateway, Volume Gateway và Tape Gateway. Việc kết nối file share từ môi trường nội bộ lên AWS giúp em hiểu rõ hơn mô hình lưu trữ hybrid trong thực tế. Em cũng tìm hiểu Snow Family và các kịch bản di chuyển dữ liệu lớn trong doanh nghiệp.

Về sao lưu và khôi phục dữ liệu, em đã nghiên cứu kiến trúc của AWS Backup, cách xây dựng Backup Plan, cơ chế lưu trữ trong Backup Vault và quy trình khôi phục dữ liệu. Em cấu hình thành công hệ thống sao lưu tự động, tích hợp SNS để gửi thông báo và thực hiện kiểm thử restore dữ liệu. Đồng thời, em cũng hiểu rõ các chiến lược Disaster Recovery như RTO, RPO, Pilot Light, Warm Standby và Active-Active để đảm bảo khả năng vận hành liên tục cho hệ thống khi xảy ra sự cố.

Trong phần lưu trữ file hệ thống, em đã thực hành với Amazon FSx bằng cách triển khai các mô hình Multi-AZ với ổ SSD và HDD, tạo file share, theo dõi hiệu năng, bật cơ chế chống trùng lặp dữ liệu, shadow copy và quản lý phiên làm việc của người dùng. Ngoài ra, em cũng thực hiện mở rộng dung lượng lưu trữ và thông lượng để đáp ứng nhu cầu sử dụng tăng cao.

Ngoài ra, em đã thực hành quy trình Import/Export máy ảo giữa môi trường on-premise và AWS. Cụ thể, em export máy ảo từ VMware, upload lên S3, import thành AMI và khởi chạy EC2. Ở chiều ngược lại, em cũng thực hiện export EC2 về lại môi trường ảo hóa nội bộ.

Thông qua các nội dung đã thực hiện trong tuần 4, em đã nắm được toàn cảnh về các giải pháp lưu trữ, sao lưu, khôi phục và phòng chống thảm họa trên AWS. Đây là nền tảng quan trọng để xây dựng các hệ thống có tính sẵn sàng cao, an toàn và dễ mở rộng trong thực tế.
