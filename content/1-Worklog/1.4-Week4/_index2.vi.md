---
title: "Nhật ký công việc - Tuần 4"
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu Tuần 4:
- Nghiên cứu kiến trúc mạng ảo độc lập (Amazon VPC) để xây dựng môi trường triển khai hệ thống an toàn.
- Tiếp cận giải pháp quản lý cơ sở dữ liệu đám mây với Amazon RDS và thực hành các bài lab cấu hình tối ưu.
- Thiết lập cơ chế kiểm soát truy cập tầng mạng (Security Groups) cho các thành phần lưu trữ dữ liệu.

| Ngày | Các công việc & Nhiệm vụ đã thực hiện | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|:---:|:---|:---:|:---:|:---|
| 1 | Học lý thuyết về Amazon VPC: Khái niệm về CIDR block, cách phân chia Public Subnet (cho các tài nguyên mở) và Private Subnet (cho các tài nguyên nội bộ cần giấu IP). | 11/05/2026 | 11/05/2026 | Tài liệu Amazon VPC |
| 2 | Nghiên cứu dịch vụ Amazon RDS: So sánh mô hình tự quản trị (Database trên EC2) và mô hình được AWS quản lý (Managed Service) về mặt vận hành, sao lưu. | 12/05/2026 | 12/05/2026 | Tài liệu Amazon RDS |
| 3 | Thực hành Lab tạo một cơ sở dữ liệu Relational Database (MySQL) trên Amazon RDS, tìm hiểu các tùy chọn lưu trữ và cơ chế tự động Backup. | 13/05/2026 | 13/05/2026 | AWS RDS Console |
| 4 | Cấu hình bảo mật tầng mạng: Tạo một Security Group riêng cho Database, thiết lập Rule chỉ cho phép kết nối từ dải IP nội bộ thuộc Private Subnet, chặn hoàn toàn truy cập trực tiếp từ Internet. | 14/05/2026 | 14/05/2026 | AWS Security Best Practices |
| 5 | Nghiên cứu kiến trúc nâng cao của RDS: Tìm hiểu cách hoạt động của cơ chế dự phòng Multi-AZ (High Availability) và mở rộng vùng đọc dữ liệu với Read Replicas. | 15/05/2026 | 15/05/2026 | Tài liệu Amazon RDS Architecture |

### Kết quả đạt được trong tuần:

*   **Tư duy hệ thống:** Nắm rõ nguyên lý thiết kế mạng an toàn trên Cloud, biết cách phân tách tài nguyên vào các vùng Subnet có mức độ bảo mật khác nhau.
*   **Quản trị Database:** Khởi tạo và kiểm tra thành công trạng thái hoạt động của một máy chủ Database MySQL trên Amazon RDS trong môi trường Lab thử nghiệm.
*   **Bảo mật hạ tầng:** Thiết lập thành công lớp tường lửa Security Group (Inbound/Outbound Rules) giúp cô lập hoàn toàn Database, bảo vệ dữ liệu trước các nguy cơ tấn công mạng.