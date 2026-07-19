---
title: "Nhật ký công việc - Tuần 8"
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu Tuần 8: Cân bằng tải ALB & Tự động co giãn EC2 Auto Scaling
*   Khoảng thời gian: từ **10/06/2026** đến **17/06/2026**.
*   Nội dung chính: Học tập và thực hiện các nhiệm vụ liên quan đến **Cân bằng tải ALB & Tự động co giãn EC2 Auto Scaling**.

| Ngày | Các công việc & Nhiệm vụ đã thực hiện | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|:---:|:---|:---:|:---:|:---|
| 1 | Tìm hiểu Application Load Balancer (ALB). Cấu hình Target Group cho cổng 8080 và khởi tạo ALB trên Public Subnets. | 10/06/2026 | 11/06/2026 | ALB Developer Guide |
| 2 | Nghiên cứu cơ chế EC2 Auto Scaling. Thực hành tạo Launch Template chứa cấu hình máy chủ, AMI và kịch bản khởi động (User Data). | 12/06/2026 | 14/06/2026 | Launch Templates Docs |
| 3 | Thiết lập Auto Scaling Group (ASG) tích hợp cùng Target Group của ALB. | 15/06/2026 | 16/06/2026 | Auto Scaling Groups Guide |
| 4 | Cấu hình Scaling Policy tự động scale-out/scale-in dựa trên CPUUtilization: Desired 2, Min 2, Max 4. | 17/06/2026 | 17/06/2026 | ASG Dynamic Scaling Policies |

### Kết quả đạt được trong tuần:

*   **Hiểu cơ chế hoạt động của ALB để phân bổ tải Frontend-Backend.**
*   **Tự thiết lập hệ thống tự động co giãn ASG.**
*   **Cấu hình User Data để tự cài ứng dụng Spring Boot khi khởi động instance mới.**
