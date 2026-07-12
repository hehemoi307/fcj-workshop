---
title: "Nhật ký công việc - Tuần 5"
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu Tuần 5:
- Nghiên cứu các dịch vụ Tính toán (Compute Services) cốt lõi trên nền tảng AWS.
- Tìm hiểu cách ứng dụng máy chủ ảo (Amazon EC2) và kiến trúc phi máy chủ (AWS Lambda) trong các mô hình web hiện đại.
- Thực hành tư duy đánh giá ưu nhược điểm (Trade-offs) của các dịch vụ tính toán để đưa ra giải pháp triển khai tối ưu.

| Ngày | Các công việc & Nhiệm vụ đã thực hiện | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|:---:|:---|:---:|:---:|:---|
| 1 | Nghiên cứu chi tiết về Amazon EC2: Tìm hiểu về Amazon Machine Image (AMI), các dòng Instance Types và cách dùng EC2 User Data để tự động hóa cài đặt môi trường khi khởi chạy. | 18/05/2026 | 18/05/2026 | Tài liệu Amazon EC2 |
| 2 | Tiếp cận mô hình Serverless: Tìm hiểu khái niệm Function-as-a-Service (FaaS) và cơ chế xử lý hướng sự kiện (Event-driven) của dịch vụ AWS Lambda. | 19/05/2026 | 19/05/2026 | Tài liệu AWS Lambda |
| 3 | Phân tích lý thuyết ứng dụng: So sánh mô hình IaaS (EC2) và FaaS (Lambda) về mặt quản trị hạ tầng (Operational Overhead), cơ chế tự động mở rộng (Scaling) và bài toán chi phí. | 20/05/2026 | 20/05/2026 | AWS Compute Blog |
| 4 | Nghiên cứu các mẫu kiến trúc (Architecture Patterns): Đánh giá cách kết hợp AWS Lambda với Amazon S3 (ví dụ: dùng Lambda để tự động xử lý hình ảnh khi có file mới tải lên S3 Bucket). | 21/05/2026 | 21/05/2026 | Dữ liệu Lab AWS Event Triggers |
| 5 | Tổng hợp lại các kiến thức phân tích hệ thống đã học trong tuần, biên soạn tài liệu và cập nhật tiến độ lên trang báo cáo Hugo local. | 22/05/2026 | 22/05/2026 | |

### Kết quả đạt được trong tuần:

*   **Kiến trúc Compute:** Phân biệt rõ rệt sự khác biệt giữa việc cấp phát, duy trì một máy chủ ảo (EC2) so với việc thực thi mã nguồn theo yêu cầu mà không cần quản lý máy chủ (Lambda).
*   **Tư duy Tự động hóa:** Nắm bắt được cách sử dụng EC2 User Data để thiết lập môi trường khởi động và ý tưởng dùng S3 Trigger để kích hoạt Lambda, giúp hệ thống vận hành linh hoạt hơn.
*   **Phân tích giải pháp:** Tích lũy được khả năng nhận diện các "Use Cases" (kịch bản sử dụng) phù hợp cho từng loại dịch vụ tính toán, tạo tiền đề để lên bản Đề xuất kiến trúc (Proposal) cho giai đoạn tới.