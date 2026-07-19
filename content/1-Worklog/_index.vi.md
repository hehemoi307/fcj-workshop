---
title: "Nhật ký công việc"
weight: 1
chapter: false
pre: " <b> 1. </b> "
---

Worklog này ghi lại hành trình thực tập 13 tuần tại **AWS First Cloud Journey** (từ ngày 17/04/2026 đến ngày 30/07/2026). Trong suốt quá trình này, sinh viên đã nghiên cứu sâu rộng các dịch vụ đám mây của AWS và triển khai thực tế hệ thống **Pet Resort & Care** — giải pháp web full-stack đặt lịch spa và mua sắm sản phẩm cho thú cưng.

---

### 📅 Giai đoạn 1: Nghiên cứu Công nghệ & Dịch vụ AWS (Tuần 1 - 10)

*   **Tuần 1 (17/04 - 23/04/2026):** [Nền tảng Đám mây & Công cụ Báo cáo](1.1-Week1/)
    *   Làm quen với hệ sinh thái AWS, tạo tài khoản Free Tier và áp dụng bảo mật ban đầu. Cài đặt và thực hành xây dựng trang tĩnh cục bộ bằng công cụ Hugo Generator.
*   **Tuần 2 (24/04 - 30/04/2026):** [Quản lý Quyền truy cập với AWS IAM](1.2-Week2/)
    *   Nghiên cứu cơ chế xác thực IAM, phân quyền dựa trên Least Privilege bằng cách tạo IAM User, Group, Customer Managed Policies và cấu hình IAM Roles an toàn.
*   **Tuần 3 (01/05 - 08/05/2026):** [Hạ tầng Mạng cơ sở Amazon VPC](1.3-Week3/)
    *   Tìm hiểu về mạng ảo VPC (Virtual Private Cloud). Thực hành tính toán IP CIDR, phân chia Public/Private Subnets và thiết lập Route Tables phù hợp cho hệ thống đa tầng.
*   **Tuần 4 (09/05 - 17/05/2026):** [Giao tiếp Mạng nâng cao & Định tuyến an toàn](1.4-Week4/)
    *   Cấu hình định tuyến đi Internet cho Private Subnet bằng NAT Gateway. Thiết lập kết nối nội bộ bảo mật đến các dịch vụ AWS bằng VPC Endpoints (Interface & Gateway).
*   **Tuần 5 (18/05 - 24/05/2026):** [Lưu trữ Đám mây với Amazon S3](1.5-Week5/)
    *   Học cách sử dụng Amazon S3 để làm nơi lưu trữ cho Frontend tĩnh và các tệp hình ảnh, tệp tin đa phương tiện (Media) tải lên từ API Backend.
*   **Tuần 6 (25/05 - 01/06/2026):** [Phân phối CDN CloudFront & Bảo mật biên với WAF](1.6-Week6/)
    *   Sử dụng CloudFront làm CDN tăng tốc độ tải trang toàn cầu. Tạo Web ACL trên AWS WAF tích hợp vào CloudFront để lọc traffic và ngăn chặn các cuộc tấn công web độc hại.
*   **Tuần 7 (02/06 - 09/06/2026):** [Máy chủ ảo Amazon EC2 cho Backend API](1.7-Week7/)
    *   Khởi tạo máy chủ ảo EC2, thiết lập Security Group chặt chẽ, cài đặt môi trường Java Corretto 17 để chạy ứng dụng Spring Boot Backend.
*   **Tuần 8 (10/06 - 17/06/2026):** [Cân bằng tải ALB & Tự động co giãn EC2 Auto Scaling](1.8-Week8/)
    *   Cấu hình Target Group và Application Load Balancer để phân phối lưu lượng. Thiết lập Launch Template và Auto Scaling Group để tự động scale server dựa trên tải thực tế.
*   **Tuần 9 (18/06 - 25/06/2026):** [Cơ sở Dữ liệu Amazon RDS & Bộ nhớ đệm ElastiCache](1.9-Week9/)
    *   Thiết lập Amazon RDS MySQL với mô hình Multi-AZ (Primary/Standby) đảm bảo tính sẵn sàng cao. Tích hợp Redis thông qua ElastiCache để lưu trữ cache và session.
*   **Tuần 10 (26/06 - 02/07/2026):** [Giám sát Hệ thống & Bảo mật thông tin cấu hình](1.10-Week10/)
    *   Mã hóa dữ liệu nhạy cảm bằng KMS và Secrets Manager. Cấu hình giám sát tài nguyên qua CloudWatch Metrics/Logs và thiết lập cảnh báo email qua Amazon SNS.

---

### 🚀 Giai đoạn 2: Thiết kế, Triển khai & Hoàn thiện Dự án (Tuần 11 - 13)

*   **Tuần 11 (03/07 - 10/07/2026):** [Thiết kế Kiến trúc Hệ thống & Lập kịch bản luồng dữ liệu](1.11-Week11/)
    *   Hệ thống hóa toàn bộ công nghệ đã học để phác thảo sơ đồ kiến trúc 3 lớp an toàn, chịu lỗi cao. Lên kế hoạch kết nối chi tiết giữa Frontend, Backend và Database.
*   **Tuần 12 (11/07 - 20/07/2026):** [Triển khai hệ thống đa tầng lên môi trường Cloud thực tế](1.12-Week12/)
    *   Deploy trực tiếp toàn bộ dự án lên AWS: Deploy Frontend tĩnh lên S3 + CloudFront; Tạo AMI từ EC2 cài Backend rồi deploy qua Auto Scaling và ALB; Kết nối Database RDS và cache Redis.
*   **Tuần 13 (21/07 - 30/07/2026):** [Kiểm thử QA (Load Test), Vá lỗi bảo mật & Tổng kết dự án](1.13-Week13/)
    *   Sử dụng công cụ kiểm thử tải Artillery để đo lường giới hạn chịu tải của hệ thống Backend. Phát hiện và sửa đổi cấu hình CORS, Database URL. Đóng gói mã nguồn và hoàn thiện báo cáo thực tập cuối kỳ.
