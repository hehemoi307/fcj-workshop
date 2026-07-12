---
title: "Nhật ký công việc - Tuần 8"
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu Tuần 8:
* Hoàn tất việc tối ưu và đóng gói mã nguồn ReactJS của dự án Pet Resort thành các tệp tĩnh (static assets) dùng cho môi trường Production.
* Nghiên cứu và phân tích các giải pháp triển khai Frontend trên AWS: Sử dụng dịch vụ trọn gói (AWS Amplify) vs Tự xây dựng hạ tầng nguyên bản (Amazon S3 kết hợp CloudFront).
* Thống nhất lộ trình cùng nhóm và mentor: Chuyển hướng sang tự cấu hình S3 và CloudFront để rèn luyện kỹ năng quản trị mạng và lưu trữ chuyên sâu.

### Nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ chi tiết | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
| :---: | :--- | :---: | :---: | :--- |
| 1 | - Tạm dừng phát triển giao diện UI mới, tìm hiểu quy trình tối ưu hóa (Minify/Uglify) và biên dịch mã nguồn ReactJS.<br>- Đọc tài liệu về cơ chế Build tĩnh để chuẩn bị đưa ứng dụng lên mây. | 08/06/2026 | 08/06/2026 | React Deployment Guide |
| 2 | - Thực hành chạy lệnh `npm run build` trên Terminal của VS Code để biên dịch dự án Frontend Pet Resort thành thư mục `build`.<br>- Phân tích và xử lý các cảnh báo (warnings) về dung lượng tệp tin (Chunk size) quá lớn để tối ưu tốc độ tải. | 09/06/2026 | 09/06/2026 | Webpack & NPM Docs |
| 3 | - Cài đặt gói thư viện `serve` để chạy thử nghiệm độc lập thư mục `build` trên môi trường localhost.<br>- Kiểm tra kỹ lại các luồng điều hướng (React Router) xem có bị lỗi 404 khi chạy ở chế độ Production hay không. | 10/06/2026 | 10/06/2026 | React Router Documentation |
| 4 | - Tìm hiểu sơ bộ **AWS Amplify** — dịch vụ nền tảng giúp tự động hóa hoàn toàn CI/CD, kết nối GitHub và host web tĩnh dễ dàng chỉ với vài cú click.<br>- Phân tích sự đánh đổi (Trade-off) giữa Amplify (nhanh gọn, tự động) và mô hình S3 + CloudFront (cấu hình thủ công, kiểm soát sâu). | 11/06/2026 | 11/06/2026 | AWS Amplify Hosting Guide |
| 5 | - Cùng nhóm và mentor tham vấn giải pháp kiến trúc tổng thể. Phía Backend chọn EC2, do đó phần Frontend cũng quyết định chọn **S3 + CloudFront** thay vì Amplify.<br>- Lý do: Tự tay thiết lập cơ chế Caching, cấu hình bảo mật Bucket Policy và xin cấp phát chứng chỉ SSL/TLS sẽ mang lại kiến thức hạ tầng vững chắc hơn rất nhiều. | 12/06/2026 | 12/06/2026 | AWS CloudFront Best Practices |

### Kết quả đạt được trong tuần:

* **Làm chủ quy trình đóng gói Frontend (Static Build & Optimization):**
  * Hiểu rõ sự khác biệt giữa môi trường `development` (chạy qua dev-server với Hot Reload) và môi trường `production` (các tệp HTML, CSS, JS đã được nén gọn nhẹ).
  * Xử lý thành công việc đóng gói dự án ReactJS và xác nhận mã nguồn tĩnh hoạt động hoàn hảo, không gặp lỗi điều hướng (Routing) khi chạy độc lập.

* **Hình thành tư duy đánh giá giải pháp kiến trúc (Architecture Evaluation):**
  * Nắm bắt được ưu và nhược điểm của các giải pháp Hosting trên AWS dành cho Frontend (Amplify vs S3 + CDN).
  * Biết cách đặt câu hỏi đánh giá: Giữa việc triển khai nhanh chóng để kịp tiến độ và việc tự cấu hình để hiểu sâu bản chất hệ thống, điều gì quan trọng hơn cho mục tiêu thực tập?

* **Xác định rõ lộ trình triển khai hạ tầng cho giai đoạn nước rút:**
  * Đồng bộ định hướng với toàn nhóm: Chấp nhận con đường "khó hơn" là tự thiết lập Amazon S3 kết hợp mạng phân phối nội dung CloudFront. Lựa chọn này đòi hỏi nhiều công sức cấu hình phân quyền và bộ nhớ đệm, nhưng lại hoàn toàn đáp ứng được mục tiêu tích lũy kinh nghiệm thực chiến chuyên sâu của chương trình.