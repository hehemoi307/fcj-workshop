---
title: "Nhật ký công việc - Tuần 7"
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu Tuần 7:
* Tối ưu hóa quy trình làm việc: Chuyển đổi từ việc dùng giao diện web (AWS Console) sang quản lý tài nguyên đám mây trực tiếp trên Visual Studio Code (VS Code).
* Tìm hiểu sâu về bộ công cụ giám sát và quan sát hệ thống (Observability) của AWS.
* Quản lý bảo mật thông tin nhạy cảm (mật khẩu, chuỗi kết nối) bằng các dịch vụ quản lý bí mật.

### Nhiệm vụ thực hiện trong tuần:
| Ngày | Các công việc & Nhiệm vụ đã thực hiện | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
| :---: | :--- | :---: | :---: | :--- |
| 1 | - Cài đặt AWS CLI và tiện ích AWS Toolkit trên Visual Studio Code.<br>- Thực hành xác thực (AWS Configure) và quản lý các tài nguyên cơ bản (như S3, EC2) trực tiếp từ giao diện và Terminal tích hợp của VS Code. | 01/06/2026 | 01/06/2026 | AWS Toolkit for VS Code |
| 2 | - Nghiên cứu dịch vụ Amazon CloudWatch: Tìm hiểu khái niệm Metrics (Chỉ số), Logs (Nhật ký) và Alarms (Cảnh báo).<br>- Thực hành tạo CloudWatch Alarm để tự động gửi email khi CPU của máy chủ ảo vượt quá ngưỡng cho phép. | 02/06/2026 | 02/06/2026 | Amazon CloudWatch Docs |
| 3 | - Phân biệt CloudWatch và AWS CloudTrail.<br>- Kích hoạt CloudTrail để ghi nhận lại toàn bộ lịch sử các lời gọi API. Thực hành tải các file log định dạng JSON về VS Code để đọc hiểu và phân tích cấu trúc truy vết. | 03/06/2026 | 03/06/2026 | AWS CloudTrail User Guide |
| 4 | - Nghiên cứu dịch vụ AWS Secrets Manager và AWS Systems Manager (Parameter Store).<br>- Thực hành lab lưu trữ an toàn các thông tin nhạy cảm (như mật khẩu Database) thay vì hardcode trực tiếp vào mã nguồn. | 04/06/2026 | 04/06/2026 | AWS Secrets Manager Docs |
| 5 | - Đóng gói kiến thức và viết một bài blog ngắn tóm tắt sự khác nhau giữa CloudWatch và CloudTrail.<br>- Cập nhật nội dung worklog của tuần lên hệ thống Hugo local bằng VS Code. | 05/06/2026 | 05/06/2026 | |

### Kết quả đạt được trong tuần:

* **Tối ưu hóa môi trường làm việc:** Tích hợp thành công môi trường AWS vào thẳng trình soạn thảo mã nguồn VS Code. Việc sử dụng AWS CLI và AWS Toolkit giúp thao tác tạo, sửa, xóa tài nguyên nhanh chóng và chuyên nghiệp hơn rất nhiều so với click chuột trên web.
* **Tư duy giám sát hệ thống (Observability):**
  * Hiểu rõ cách giám sát hiệu suất và sức khỏe của hệ thống thông qua biểu đồ CloudWatch.
  * Thiết lập thành công cơ chế truy vết bảo mật với CloudTrail, rèn luyện kỹ năng đọc file log JSON cấu trúc phức tạp.
* **Bảo mật dữ liệu ứng dụng:** Nắm được phương pháp quản lý các biến môi trường và chuỗi kết nối Database một cách an toàn thông qua Secrets Manager, loại bỏ hoàn toàn rủi ro lộ lọt mật khẩu trong source code.