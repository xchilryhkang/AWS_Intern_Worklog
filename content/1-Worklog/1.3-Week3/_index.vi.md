---
title: "Worklog Tuần 3"
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Định hướng học tập trong tuần 3

- Tìm hiểu sâu về dịch vụ máy chủ ảo Amazon EC2 – nền tảng cốt lõi của hạ tầng AWS.
- Nắm được cách vận hành, giám sát và mở rộng hệ thống máy chủ theo mô hình thực tế.

---

### Nội dung triển khai trong tuần

| Thứ | Hoạt động chính | Bắt đầu | Kết thúc | Tham khảo |
|-----|------------------|----------|-----------|------------|
| 2 | Nghiên cứu tổng quan về dịch vụ EC2 và các thành phần liên quan như: instance type, AMI, key pair, EBS, instance store, user data, meta data, auto scaling, EFS/FSx, Lightsail và MGN | 11/08/2025 | 11/08/2025 | |
| 3 | Thực hành tạo EC2 trên Windows và Linux, snapshot sao lưu dữ liệu, cài đặt ứng dụng trên EC2, quản lý tài nguyên bằng tag và resource group, phân quyền với IAM và dọn dẹp tài nguyên | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Tìm hiểu và cấu hình Amazon CloudWatch: giám sát chỉ số, thu thập log, thiết lập cảnh báo và xây dựng dashboard theo dõi trạng thái hệ thống | 13/08/2025 | 13/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Nghiên cứu mô hình EC2 Auto Scaling, các cơ chế scale, launch template và elastic load balancer; thực hành triển khai hệ thống có khả năng tự động mở rộng và thu hẹp | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | Làm quen với Amazon Lightsail, triển khai các instance ứng dụng và database, cấu hình load balancer, snapshot backup và nâng cấp cấu hình máy chủ | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

### Tổng hợp kết quả đạt được trong tuần 3

Trong tuần thứ ba, em tập trung tìm hiểu chuyên sâu về dịch vụ EC2 – thành phần quan trọng trong việc triển khai hạ tầng máy chủ trên AWS. Thông qua quá trình học tập và thực hành, em đã hiểu rõ hơn về kiến trúc của EC2 cũng như cách lựa chọn cấu hình phù hợp với từng nhu cầu sử dụng. Em có thể phân biệt được các nhóm instance phổ biến như nhóm tổng hợp, nhóm tối ưu CPU, tối ưu bộ nhớ và tối ưu lưu trữ.

Bên cạnh đó, em đã nắm được vai trò của AMI, key pair, EBS và instance store trong quá trình khởi tạo và vận hành máy chủ. Việc sử dụng user data và meta data cũng giúp em tự động hóa quá trình thiết lập môi trường ngay từ khi EC2 được khởi tạo. Ngoài ra, em cũng làm quen với EFS và FSx để phục vụ nhu cầu lưu trữ và chia sẻ dữ liệu giữa nhiều máy chủ.

Về thực hành, em đã tự triển khai và kết nối thành công máy chủ EC2 trên cả hai hệ điều hành Windows và Linux. Em biết cách tạo snapshot để sao lưu dữ liệu và khôi phục khi cần thiết, đồng thời cài đặt được các ứng dụng web cơ bản phục vụ cho việc thử nghiệm. Việc sử dụng tag và resource group giúp em quản lý tài nguyên một cách khoa học hơn. Đồng thời, thông qua IAM, em đã biết cách giới hạn quyền truy cập nhằm đảm bảo an toàn cho hệ thống.

Trong phần giám sát, em đã tìm hiểu và áp dụng Amazon CloudWatch để theo dõi hoạt động của hệ thống. Em cấu hình được các chỉ số giám sát EC2, thu thập log từ ứng dụng, tạo cảnh báo khi CPU hoặc lưu lượng mạng vượt ngưỡng và xây dựng dashboard tổng hợp giúp theo dõi tình trạng toàn bộ hệ thống một cách trực quan.

Về khả năng mở rộng, em đã hiểu rõ cơ chế hoạt động của EC2 Auto Scaling, bao gồm cách mở rộng thủ công, mở rộng theo lịch và mở rộng tự động dựa trên tải thực tế. Em cũng đã triển khai thành công auto scaling group kết hợp với load balancer để đảm bảo hệ thống có khả năng tự điều chỉnh số lượng máy chủ khi lưu lượng thay đổi.

Cuối tuần, em tiếp cận thêm dịch vụ Amazon Lightsail – một nền tảng triển khai nhanh các ứng dụng phổ biến. Em đã thực hành triển khai các mô hình như website WordPress, hệ thống bán hàng PrestaShop và phần mềm kế toán Akaunting. Ngoài ra, em cũng sử dụng Lightsail Database để lưu trữ dữ liệu, Lightsail Load Balancer để phân phối tải, tạo snapshot để sao lưu và thực hiện nâng cấp cấu hình instance khi cần thiết.

Thông qua các nội dung đã thực hiện trong tuần 3, em đã nắm được quy trình triển khai, vận hành, giám sát và mở rộng hệ thống máy chủ trên AWS, tạo nền tảng vững chắc để tiếp tục học và triển khai các hệ thống thực tế ở những giai đoạn tiếp theo.
