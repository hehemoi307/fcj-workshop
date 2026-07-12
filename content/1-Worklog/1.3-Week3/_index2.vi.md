---
title: "Nhật ký công việc - Tuần 3"
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu Tuần 3:
- Hiểu rõ cơ chế quản lý lưu trữ đối tượng (Object Storage) trên đám mây AWS.
- Thực hành xây dựng không gian lưu trữ và tính năng phân phối nội dung tĩnh (Static Website Hosting) thông qua các bài lab thử nghiệm trên Amazon S3.
- Chủ động thiết lập các lớp bảo vệ tài khoản và giám sát tài chính để đảm bảo an toàn cho Credit thực tập.

| Ngày | Các công việc & Nhiệm vụ đã thực hiện | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|:---:|:---|:---:|:---:|:---|
| 1 | Truy cập AWS Billing Dashboard, thiết lập AWS Budgets để hệ thống tự động gửi email cảnh báo khi chi phí vượt mức hạn mức cho phép. | 04/05/2026 | 04/05/2026 | AWS Billing & Cost Management |
| 2 | Nghiên cứu kiến trúc của Amazon S3: Phân biệt sự khác nhau giữa Block Storage và Object Storage, tìm hiểu các Storage Classes. | 05/05/2026 | 05/05/2026 | Tài liệu Amazon S3 |
| 3 | Thực hành tạo S3 Bucket demo với tên `frontend-static-hosting-demo` nhằm mục đích thử nghiệm môi trường triển khai giao diện web cơ bản. | 06/05/2026 | 06/05/2026 | Giao diện điều khiển AWS |
| 4 | Tìm hiểu cấu hình quyền truy cập S3: Kích hoạt tính năng Static Website Hosting và viết cấu hình Bucket Policy (cấp quyền `PublicReadGetObject`) cho bucket demo. | 07/05/2026 | 07/05/2026 | Tài liệu S3 Bucket Policies |
| 5 | Áp dụng IAM Best Practices: Thiết lập Password Policy và tạo một IAM User thử nghiệm, gắn quyền `` để tập thao tác an toàn thay vì dùng Root user. | 08/05/2026 | 08/05/2026 | AWS IAM Best Practices |

### Kết quả đạt được trong tuần:

*   **Quản trị rủi ro:** Hoàn thiện lớp bảo vệ tài khoản đầu tiên với hệ thống cảnh báo ngân sách tự động, giúp yên tâm hơn khi thực hành các bài lab.
*   **Triển khai lưu trữ:** Cấu hình thành công S3 Bucket demo và mở quyền Public thông qua Bucket Policy, thử nghiệm thành công việc host một file giao diện HTML tĩnh đơn giản lên Internet.
*   **Bảo mật hệ thống:** Nắm vững quy trình quản lý định danh IAM, đảm bảo tuân thủ nguyên tắc quyền tối thiểu (Least Privilege).