---
title: "Nhật ký công việc - Tuần 6"
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu Tuần 6:
- Có mặt tại văn phòng để tham gia chuỗi ngày tự học, đồng bộ tiến độ và giải quyết các bài toán kiến trúc cùng các thành viên trong nhóm.
- Ôn tập và củng cố nền tảng 4 trụ cột dịch vụ AWS (Compute, Network, Storage, Security).
- Đào sâu nghiên cứu các giải pháp tăng tốc độ tải trang và phân phối nội dung tĩnh trên toàn cầu.

| Ngày | Các công việc & Nhiệm vụ đã thực hiện | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
|:---:|:---|:---:|:---:|:---|
| 1 | Tự học tại văn phòng: Rà soát lại hệ thống phân quyền IAM. Tập trung vào việc viết các Custom Policies để cấp quyền truy cập an toàn cho tài nguyên tĩnh. | 25/05/2026 | 25/05/2026 | AWS IAM Documentation |
| 2 | Ôn tập chuyên sâu Amazon S3: Nghiên cứu kỹ về cơ chế CORS (Cross-Origin Resource Sharing) và các rủi ro bảo mật khi mở Public Bucket để host web. | 26/05/2026 | 26/05/2026 | Amazon S3 Guide |
| 3 | Tham gia buổi thảo luận kiến trúc mạng cùng nhóm: Hiểu rõ luồng đi của dữ liệu từ Frontend (truy cập Public) gọi vào Backend (được giấu trong VPC/Private Subnet). | 27/05/2026 | 27/05/2026 | |
| 4 | Nghiên cứu giải pháp phân phối nội dung: Đọc tài liệu về Amazon CloudFront (CDN), phân tích ưu điểm khi kết hợp S3 và CloudFront (Tốc độ Cache, hỗ trợ SSL/HTTPS). | 28/05/2026 | 28/05/2026 | AWS CloudFront Blog |
| 5 | Đóng gói nội dung tự học. Ghi chú lại một số thắc mắc về cơ chế xóa bộ nhớ đệm (Cache Invalidation) của CDN để nhờ Mentor tư vấn. Cập nhật worklog lên Hugo. | 29/05/2026 | 29/05/2026 | |

### Kết quả đạt được trong tuần:

*   **Củng cố nền tảng:** Hoàn thiện và đóng gói toàn bộ kiến thức về các dịch vụ cốt lõi của AWS, tự tin hơn trong việc lựa chọn dịch vụ để thiết kế hệ thống.
*   **Chốt phương án Frontend:** Xác định rõ chiến lược triển khai giao diện: Không chỉ dừng lại ở S3 Static Hosting thông thường mà sẽ tích hợp thêm CloudFront CDN để đảm bảo website load nhanh và có chứng chỉ bảo mật HTTPS.
*   **Kỹ năng làm việc:** Duy trì kỷ luật tự học tại văn phòng hiệu quả, tương tác và hỗ trợ các thành viên khác trong nhóm làm rõ bức tranh kiến trúc tổng thể.