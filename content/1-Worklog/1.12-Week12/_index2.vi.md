---
title: "Nhật ký công việc - Tuần 12"
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu Tuần 12: Triển khai hệ thống đa tầng lên môi trường Cloud thực tế
*   Khoảng thời gian: từ **11/07/2026** đến **20/07/2026**.
*   Nội dung chính: Học tập và thực hiện các nhiệm vụ liên quan đến **Triển khai hệ thống đa tầng lên môi trường Cloud thực tế**.

| Ngày | Các công việc & Nhiệm vụ đã thực hiện | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|:---:|:---|:---:|:---:|:---|
| 1 | Triển khai hạ tầng cơ sở: Tạo VPC, chia Subnets, tạo Internet Gateway, NAT Gateway, cấu hình Route Tables và Security Groups. | 11/07/2026 | 12/07/2026 | Infrastructure-as-Code Basics |
| 2 | Deploy Frontend: Đóng gói code ReactJS thành file tĩnh, upload lên S3 Bucket, tạo CloudFront Distribution tích hợp AWS WAF. | 13/07/2026 | 14/07/2026 | S3 & CloudFront Deployment |
| 3 | Triển khai Database RDS MySQL Multi-AZ và ElastiCache Redis cluster trên Private Subnets. | 15/07/2026 | 16/07/2026 | RDS & Redis Provisioning |
| 4 | Deploy Backend: Khởi chạy máy chủ EC2 gốc, cấu hình ứng dụng Spring Boot Backend, kết nối Database RDS và cache Redis. | 17/07/2026 | 17/07/2026 | Spring Boot EC2 Setup |
| 5 | Tạo Amazon Machine Image (AMI) từ EC2 Backend gốc. Tạo Launch Template sử dụng AMI này và thiết lập Auto Scaling Group. | 18/07/2026 | 19/07/2026 | AWS EC2 AMI Creation |
| 6 | Khởi tạo Application Load Balancer, liên kết với Target Group của Auto Scaling Group. Cấu hình CORS và DNS kết nối Frontend-Backend. | 20/07/2026 | 20/07/2026 | ALB Routing Setup |

### Kết quả đạt được trong tuần:

*   **Triển khai hoạt động thành công hệ thống đa tầng bảo mật trên Cloud.**
*   **Tự động hóa cấu hình môi trường khởi tạo thông qua AMI và Launch Template.**
*   **Tích hợp kết nối Frontend và Backend an toàn qua HTTPS.**
