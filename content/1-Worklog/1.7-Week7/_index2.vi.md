---
title: "Nhật ký công việc - Tuần 7"
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu Tuần 7: Máy chủ ảo Amazon EC2 cho Backend API
*   Khoảng thời gian: từ **02/06/2026** đến **09/06/2026**.
*   Nội dung chính: Học tập và thực hiện các nhiệm vụ liên quan đến **Máy chủ ảo Amazon EC2 cho Backend API**.

| Ngày | Các công việc & Nhiệm vụ đã thực hiện | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|:---:|:---|:---:|:---:|:---|
| 1 | Nghiên cứu Amazon EC2. So sánh Instance Types, cấu hình lưu trữ EBS (Elastic Block Store). | 02/06/2026 | 03/06/2026 | Amazon EC2 User Guide |
| 2 | Thực hành khởi tạo EC2 Instance chạy Amazon Linux 2023 đặt trong Private Subnet để đảm bảo an toàn. | 04/06/2026 | 05/06/2026 | EC2 Console Hands-on |
| 3 | Thiết lập Security Group `SG_Backend` chặn mọi truy cập trực tiếp từ Internet, chỉ mở cổng 8080 cho Load Balancer. | 06/06/2026 | 07/06/2026 | EC2 Security Groups Docs |
| 4 | Cài đặt môi trường ứng dụng: Kết nối an toàn qua AWS Systems Manager Session Manager, cài đặt Java Corretto 17. | 08/06/2026 | 09/06/2026 | AWS Systems Manager User Guide |

### Kết quả đạt được trong tuần:

*   **Hiểu cách vận hành và lựa chọn cấu hình máy chủ EC2.**
*   **Triển khai EC2 an toàn trong Private Subnet không có IP public.**
*   **Quản trị máy chủ hoàn toàn thông qua Systems Manager, loại bỏ port SSH 22 truyền thống.**
