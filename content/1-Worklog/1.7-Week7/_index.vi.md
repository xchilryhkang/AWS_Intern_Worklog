---
title: "Worklog Tuần 7"
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Định hướng học tập trong tuần 7

- Làm quen với kiến trúc Serverless thông qua AWS Lambda và Amazon API Gateway.
- Hiểu nguyên lý hoạt động của các hệ thống Event-Driven trên nền tảng AWS.
- Biết cách xây dựng hệ thống xử lý bất đồng bộ bằng Amazon SQS và SNS.
- Thực hành xây dựng API kết nối Lambda với DynamoDB và S3 để xử lý dữ liệu.

---

### Nội dung triển khai trong tuần

| Thứ | Hoạt động chính | Bắt đầu | Kết thúc | Tham khảo |
|-----|------------------|----------|-----------|------------|
| 2 | Tìm hiểu về AWS Lambda: khái niệm function, cách phân quyền thông qua IAM Role; tìm hiểu Amazon API Gateway: các HTTP method, cơ chế CORS; thực hành tạo IAM Role cho Lambda, xây dựng Lambda function xử lý upload file, cấu hình API Gateway trigger Lambda và lưu dữ liệu vào DynamoDB | 11/08/2025 | 11/08/2025 | |
| 3 | Thực hành tích hợp Lambda với S3 và DynamoDB: tạo Lambda xử lý ảnh, tạo S3 Bucket, xây dựng IAM Policy cho Lambda, tạo và quản lý bảng trong DynamoDB, xây dựng Lambda function ghi dữ liệu và dọn dẹp tài nguyên | 12/08/2025 | 12/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 4 | Thực hành triển khai website tĩnh với S3: tạo Bucket, bật static hosting, gán policy và upload frontend; xây dựng hệ thống CRUD với DynamoDB và Lambda, cấu hình API Gateway, kiểm thử API bằng Postman và frontend, dọn dẹp tài nguyên | 14/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 5 | Tìm hiểu kiến trúc Event-Driven với Amazon SQS và SNS: nguyên lý publish/subscribe và message queue; thực hành tạo Queue và Topic SNS, xây dựng Lambda và API để tương tác với Queue và SNS, kiểm thử hoạt động hệ thống | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |
| 6 | Tìm hiểu AWS Step Functions và vai trò trong việc điều phối (orchestration) các microservices trong hệ thống Serverless | 15/08/2025 | 15/08/2025 | https://cloudjourney.awsstudygroup.com/ |

---

### Tổng hợp kết quả đạt được trong tuần 7

Trong tuần thứ bảy, em tập trung tìm hiểu và thực hành các mô hình kiến trúc Serverless và Event-Driven trên nền tảng AWS. Trước hết, em đã nghiên cứu cách hoạt động của AWS Lambda, hiểu được cơ chế triển khai hàm xử lý không cần quản lý máy chủ, cũng như vai trò của IAM Role trong việc cấp quyền truy cập tài nguyên cho Lambda theo nguyên tắc tối thiểu (least privilege).

Song song với đó, em tìm hiểu về Amazon API Gateway, bao gồm cách xây dựng các REST API, sử dụng các phương thức HTTP và thiết lập CORS để cho phép frontend gọi API một cách an toàn. Trong quá trình thực hành, em đã xây dựng thành công hệ thống trong đó API Gateway đóng vai trò làm cổng trung gian, kích hoạt Lambda xử lý request và ghi dữ liệu xuống DynamoDB.

Tiếp theo, em thực hành tích hợp Lambda với Amazon S3 và DynamoDB. Em đã xây dựng Lambda function để xử lý upload file lên S3, đồng thời lưu metadata xuống DynamoDB. Thông qua nội dung này, em hiểu rõ hơn quy trình xây dựng một hệ thống backend serverless hoàn chỉnh với ba thành phần chính: API Gateway – Lambda – DynamoDB.

Ngoài ra, em cũng triển khai thành công mô hình host website tĩnh bằng S3, kết hợp frontend gọi API thông qua API Gateway để thực hiện các thao tác thêm, sửa, xóa và truy vấn dữ liệu. Việc kiểm thử bằng Postman và trực tiếp trên giao diện web giúp em hiểu rõ luồng xử lý request trong môi trường thực tế.

Bên cạnh kiến trúc Serverless, em tiếp tục tìm hiểu mô hình Event-Driven thông qua Amazon SQS và SNS. Em đã tạo Queue và Topic SNS, xây dựng Lambda để xử lý message từ Queue, cũng như thực hành publish và subscribe để mô phỏng các hệ thống xử lý bất đồng bộ. Qua đó, em hiểu được vai trò của hàng đợi trong việc tách rời các thành phần trong hệ thống, tăng độ ổn định và khả năng mở rộng.

Cuối tuần, em có thêm kiến thức tổng quan về AWS Step Functions và khả năng điều phối các Lambda function trong hệ thống microservices theo từng luồng xử lý logic. Thông qua tuần học này, em đã nắm được nền tảng quan trọng của kiến trúc Serverless, Event-Driven và cách xây dựng các hệ thống backend hiện đại trên AWS với khả năng mở rộng, tiết kiệm chi phí và dễ bảo trì.

