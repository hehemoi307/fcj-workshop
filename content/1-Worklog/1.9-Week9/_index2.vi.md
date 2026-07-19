---
title: "Nhật ký công việc - Tuần 9"
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu Tuần 9: Cơ sở Dữ liệu Amazon RDS & Bộ nhớ đệm ElastiCache
*   Khoảng thời gian: từ **18/06/2026** đến **25/06/2026**.
*   Nội dung chính: Học tập và thực hiện các nhiệm vụ liên quan đến **Cơ sở Dữ liệu Amazon RDS & Bộ nhớ đệm ElastiCache**.

| Ngày | Các công việc & Nhiệm vụ đã thực hiện | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|:---:|:---|:---:|:---:|:---|
| 1 | Nghiên cứu Amazon RDS. So sánh các mô hình triển khai Single-AZ vs Multi-AZ. | 18/06/2026 | 19/06/2026 | Amazon RDS User Guide |
| 2 | Khởi tạo RDS MySQL DB Instance chạy chế độ Multi-AZ (Primary/Standby) đặt trên Subnet Group riêng của Private Subnets. | 20/06/2026 | 21/06/2026 | RDS Multi-AZ Deployment |
| 3 | Thiết lập Security Group của Database chỉ cho phép kết nối ở cổng 3306 từ Security Group `SG_Backend` của EC2. | 22/06/2026 | 23/06/2026 | RDS Security Groups Docs |
| 4 | Tìm hiểu Amazon ElastiCache. Khởi tạo một Redis cluster chạy trong Private Subnet để lưu cache danh mục sản phẩm của Pet Shop. | 24/06/2026 | 25/06/2026 | Amazon ElastiCache Docs |

### Kết quả đạt được trong tuần:

*   **Hiểu và cấu hình RDS Multi-AZ để tăng độ tin cậy của dữ liệu.**
*   **Bảo mật lớp cơ sở dữ liệu ở mức tối đa bằng Security Groups.**
*   **Tích hợp bộ nhớ đệm Redis để tăng hiệu năng đọc của ứng dụng.**
