---
title: "Worklog Tuần 2"
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

### Định hướng học tập và thực hành trong tuần 2

- Tìm hiểu cách xây dựng hạ tầng mạng trên AWS theo mô hình chuẩn.
- Nắm được các cơ chế bảo mật trong môi trường VPC.
- Thiết lập các hình thức kết nối an toàn giữa hệ thống nội bộ và hệ thống Cloud.

---

### Nội dung triển khai trong tuần

| Thứ | Hoạt động chính | Bắt đầu | Kết thúc | Tham khảo |
|-----|------------------|----------|-----------|------------|
| 2 | Nghiên cứu tổng quan Amazon VPC, phạm vi hoạt động theo Region, AZ, CIDR; tìm hiểu các thành phần mạng như Subnet, Route Table, Internet Gateway, NAT Gateway; tìm hiểu cơ chế bảo mật bằng Security Group và Network ACL; thực hành tạo mới VPC và các thành phần cơ bản | 11/08/2025 | 11/08/2025 | |
| 3 | Tìm hiểu EC2 cơ bản: loại instance, AMI, key pair, cấu hình mạng; các hình thức kết nối vào EC2; tìm hiểu Elastic IP, Reachability Analyzer, Session Manager và CloudWatch | 13/08/2025 | 13/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Triển khai hệ thống EC2 đa vùng khả dụng; tạo NAT Gateway; giám sát VPC bằng CloudWatch; thiết lập Instance Connect Endpoint, sử dụng Session Manager; thực hiện dọn dẹp toàn bộ tài nguyên sau khi hoàn thành | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Tìm hiểu các mô hình kết nối mạng: Site-to-Site VPN, Transit Gateway và VPC Peering | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | Thực hành cấu hình VPN kết nối giữa AWS và môi trường giả lập on-premise; thiết lập VPC Peering và Transit Gateway | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

### Tổng hợp kết quả đạt được trong tuần 2

Trong tuần thứ hai, em đã tập trung tìm hiểu và xây dựng hệ thống mạng cơ bản trên AWS, đồng thời triển khai các mô hình kết nối và bảo mật phổ biến trong thực tế.

Cụ thể, em đã tự tay thiết kế và tạo thành công một hệ thống VPC hoàn chỉnh, bao gồm một VPC chính với dải địa chỉ IP 10.0.0.0/16. Bên trong VPC, em triển khai hai subnet public và private nằm ở hai Availability Zone khác nhau để đảm bảo khả năng sẵn sàng cao. Hệ thống định tuyến được cấu hình đầy đủ thông qua Route Table, Internet Gateway và NAT Gateway nhằm đảm bảo các máy chủ ở private subnet vẫn có thể truy cập Internet một cách an toàn. Đồng thời, em cũng kích hoạt VPC Flow Logs và theo dõi lưu lượng mạng thông qua CloudWatch Logs.

Bên cạnh đó, em đã nắm được quy trình triển khai và vận hành EC2, bao gồm việc tạo instance tại cả public subnet và private subnet, gán Elastic IP cho máy chủ public và thực hiện các hình thức truy cập như SSH, EC2 Instance Connect và Session Manager. Việc giám sát tài nguyên EC2 được thực hiện thông qua Amazon CloudWatch với các chỉ số về CPU, Network và trạng thái hệ thống.

Về mặt bảo mật, em đã cấu hình thành công Security Group để kiểm soát truy cập ở mức máy chủ và Network ACL để kiểm soát ở mức subnet. Ngoài ra, em cũng thiết lập CloudWatch Alarm để cảnh báo khi tài nguyên EC2 có dấu hiệu hoạt động bất thường.

Trong phần kết nối mạng nâng cao, em đã tìm hiểu và thực hành mô hình AWS Site-to-Site VPN, bao gồm việc tạo Virtual Private Gateway, Customer Gateway và thiết lập đường hầm IPSec giữa AWS và hệ thống on-premise mô phỏng. Đồng thời, em cũng triển khai VPC Peering nhằm kết nối hai VPC trong cùng khu vực, và làm quen với mô hình AWS Transit Gateway để kết nối nhiều mạng với nhau theo kiến trúc tập trung.

Ngoài ra, em cũng hiểu rõ hơn cách sử dụng AWS Systems Manager trong quản lý và vận hành hệ thống mà không cần truy cập trực tiếp thông qua SSH, giúp tăng mức độ bảo mật cho hạ tầng.

Thông qua các nội dung đã thực hiện, em đã nắm được nền tảng về thiết kế hạ tầng mạng, bảo mật và kết nối trên AWS, tạo tiền đề cho việc triển khai các hệ thống phức tạp hơn trong các tuần tiếp theo.
