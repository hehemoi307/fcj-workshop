---
title: "Nhật ký công việc - Tuần 9"
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu Tuần 9:
* Tối ưu hóa hiệu suất tải trang (Performance Tuning) và bảo mật cấu hình môi trường cho mã nguồn Frontend ReactJS.
* Nghiên cứu chuyên sâu về cơ chế bộ nhớ đệm (Caching) của Amazon CloudFront và các công cụ giám sát tài nguyên tĩnh.
* Kiểm thử và xử lý các kịch bản ngoại lệ (Edge Cases) trên giao diện người dùng (UI/UX) ở môi trường local trước khi đưa lên Cloud.

### Nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ chi tiết | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
| :---: | :--- | :---: | :---: | :--- |
| 1 | - Rà soát và tối ưu hóa mã nguồn ReactJS.<br>- Triển khai kỹ thuật Code Splitting và Lazy Loading để chia nhỏ kích thước tệp tĩnh (bundle size), giúp tăng tốc độ tải trang lần đầu (First Contentful Paint). | 15/06/2026 | 15/06/2026 | React Performance Optimization |
| 2 | - Tìm hiểu lý thuyết chuyên sâu về **Amazon CloudFront**.<br>- Nghiên cứu các khái niệm Time-to-Live (TTL), Cache Policies và cơ chế ép làm mới dữ liệu (Cache Invalidation) khi cập nhật phiên bản web mới. | 16/06/2026 | 16/06/2026 | Tài liệu Amazon CloudFront |
| 3 | - Bảo mật mã nguồn Frontend: Tách các cấu hình như địa chỉ Base URL gọi API, các Public Key của dịch vụ bên thứ ba ra khỏi mã nguồn thuần túy.<br>- Cấu hình sử dụng biến môi trường (Environment Variables) thông qua tệp `.env`. | 17/06/2026 | 17/06/2026 | React Environment Variables |
| 4 | - Tìm hiểu cách giám sát Frontend thông qua **Amazon CloudWatch**.<br>- Học cách phân tích các chỉ số của S3 và CloudFront (như Tỉ lệ Cache Hit/Miss Rate, lượng băng thông tiêu thụ, tỉ lệ lỗi 4xx/5xx). | 18/06/2026 | 18/06/2026 | AWS CloudWatch Metrics |
| 5 | - Thực hiện kiểm thử các kịch bản lỗi cục bộ (Error Scenarios) phía giao diện: Giả lập trạng thái mất kết nối mạng, Backend API không phản hồi hoặc gửi về Token JWT đã hết hạn.<br>- Cấu hình `Axios Interceptors` để đánh chặn và xử lý lỗi tập trung. | 19/06/2026 | 19/06/2026 | Guide to Axios Error Handling |

### Kết quả đạt được trong tuần:

* **Tối ưu hóa mã nguồn và hiệu suất Frontend (Frontend Performance Tuning):**
  * Giảm đáng kể dung lượng JavaScript tải xuống ở lần truy cập đầu tiên nhờ áp dụng Lazy Loading cho các component không hiển thị ngay, giúp website Pet Resort load mượt mà hơn.
  * Triển khai giải pháp bảo vệ cấu hình: Loại bỏ hoàn toàn việc viết cứng (Hardcode) URL API Backend vào mã nguồn. Chuyển cấu trúc sang nạp động thông qua tệp `.env`, đảm bảo an toàn tuyệt đối khi push code lên kho lưu trữ GitHub.

* **Nắm vững cơ chế mạng phân phối nội dung (CDN Caching & Monitoring):**
  * Hiểu rõ cách thức CloudFront lưu trữ đệm dữ liệu ở các Edge Location. Biết cách thao tác tạo Invalidation để xóa cache cũ, ép CDN cập nhật nội dung website mới nhất ngay lập tức.
  * Nhận biết được các chỉ số quan trọng (Cache Hit Rate, Error Rate) trên CloudWatch để có thể giám sát sức khỏe của hệ thống phân phối nội dung tĩnh sau khi đưa lên hoạt động thực tế.

* **Hoàn thiện trải nghiệm người dùng trong các kịch bản lỗi (Robust UI Error Handling):**
  * Nâng cấp luồng xử lý lỗi phía Frontend bằng `Axios Interceptors`: Khi hệ thống nhận về mã lỗi 401 (Unauthorized) do JWT hết hạn, Frontend sẽ tự động điều hướng người dùng về trang `LoginPage` một cách trơn tru, thay vì hiển thị giao diện trắng (white screen).
  * Xây dựng thành công các màn hình báo lỗi dự phòng (Fallback UI / Error Boundaries) thân thiện, giúp giữ chân khách hàng khi Backend xảy ra sự cố đột ngột.

* **Chuẩn bị sẵn sàng tài liệu triển khai:**
  * Tổng hợp danh sách toàn bộ các biến môi trường (Environment Variables) cần thiết phía Frontend để chuẩn bị cho quá trình nạp tự động vào luồng CI/CD (GitHub Actions) trong các giai đoạn sắp tới.