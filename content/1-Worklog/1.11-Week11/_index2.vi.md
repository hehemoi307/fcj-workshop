---
title: "Nhật ký công việc - Tuần 11"
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu Tuần 11:

* Tiếp nhận đánh giá (feedback) từ Admin/Mentor để hiệu chỉnh luồng giao tiếp tại lớp Biên (Edge Layer) và chốt bản vẽ kiến trúc AWS tổng thể.
* Chịu trách nhiệm chính trong việc triển khai (Deploy) giao diện tĩnh Frontend (ReactJS) và thiết lập mạng phân phối nội dung (CloudFront) cho dự án Pet Resort & Care System.
* Phối hợp cùng nhóm hoàn thiện hạ tầng bảo mật, tích hợp bộ nhớ đệm (ElastiCache) để tăng tốc độ phản hồi cho hệ thống.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :---: | :--- | :---: | :---: | :--- |
| 2 | - Tiếp nhận feedback từ Admin: Điều chỉnh lại luồng định tuyến của CloudFront đối với Frontend và Media Bucket để tối ưu hóa bộ đệm (Caching) và tránh lỗi cross-origin.<br>- Cùng nhóm chốt bản vẽ kiến trúc AWS cuối cùng. | 29/06/2026 | 29/06/2026 | Feedback từ Admin AWS Study Group |
| 3 | - Phối hợp triển khai lớp Mạng & Bảo mật: Khởi tạo VPC, phân chia Subnet.<br>- Thiết lập Security Groups: Cấu hình Inbound rules cho phép lưu lượng từ CloudFront đi vào Application Load Balancer (ALB) một cách an toàn. | 30/06/2026 | 30/06/2026 | AWS Documentation (VPC, Security Groups) |
| 4 | - Tham gia triển khai lớp Dữ liệu (Data Tier): Trong khi nhóm dựng Amazon RDS MySQL, tiến hành cấu hình cụm Amazon ElastiCache (Redis) theo mô hình Cache-Aside để giảm tải cho Database chính. | 01/07/2026 | 01/07/2026 | AWS Documentation (RDS, ElastiCache) |
| 5 | - Cấu hình lại các biến môi trường (Environment Variables) của bản build ReactJS, cập nhật Base URL trỏ thẳng về Endpoint của ALB vừa được nhóm khởi tạo.<br>- Test luồng API từ local lên máy chủ EC2. | 02/07/2026 | 03/07/2026 | React Environment Config |
| 7 | - Triển khai lớp Biên (Edge Tier): Upload mã nguồn tĩnh ReactJS lên S3 Frontend, tạo S3 Media phục vụ lưu trữ ảnh.<br>- Cấu hình CloudFront phân luồng request và gắn tường lửa AWS WAF để bảo vệ website khỏi các rủi ro bảo mật (như SQL Injection, XSS). | 04/07/2026 | 04/07/2026 | AWS Documentation (CloudFront, S3, WAF) |

### Kết quả đạt được trong tuần:

#### A. Hoàn thiện Kiến trúc Hệ thống (Architecture Finalization)
* Sửa thành công lỗi logic trong thiết kế luồng dữ liệu (Data Flow) theo góp ý của Admin: Tách biệt rõ ràng vai trò của CloudFront kết hợp S3 cho Frontend tĩnh, và luồng gọi tài nguyên Media trực tiếp.
* Chốt được sơ đồ kiến trúc dự án một cách chặt chẽ, chuẩn bị sẵn sàng cho quá trình báo cáo nghiệm thu cuối kỳ.

#### B. Triển khai phân lớp Frontend và Bảo mật (Edge & Delivery Deployment)
* Đưa thành công giao diện *Pet Resort & Care System* lên môi trường Cloud thực tế.
* Tích hợp thành công CloudFront CDN, giúp trang web load cực nhanh nhờ cơ chế phân phối qua các điểm hiện diện (Edge Locations) và đảm bảo mã hóa dữ liệu với HTTPS.
* Gắn Web Application Firewall (WAF) vào CloudFront, thiết lập thành công các Rule cơ bản để đánh chặn các truy cập độc hại từ bên ngoài, tuân thủ nguyên tắc bảo mật phòng thủ chiều sâu.

#### C. Thiết lập hạ tầng cốt lõi của nhóm (Team Core Infrastructure Setup)
* **Cấu hình mạng (VPC & Networking):** Phân chia thành công các Subnet, Route Table và Internet Gateway, đảm bảo tính sẵn sàng cao (Multi-AZ) cho toàn bộ hệ thống.
* **Bảo mật nhiều lớp (Security Groups):** Cấu hình chi tiết các quy tắc tường lửa cho ALB, Backend, Database và Cache, giúp cô lập an toàn các tài nguyên nội bộ khỏi mạng Public.
* **Cơ sở dữ liệu (Amazon RDS):** Khởi tạo thành công phiên bản cơ sở dữ liệu MySQL (`petshop-database-1`), lưu trữ an toàn các thông số Endpoint nội bộ và tối ưu hóa các tùy chọn cấu hình để kiểm soát chi phí hàng tháng.