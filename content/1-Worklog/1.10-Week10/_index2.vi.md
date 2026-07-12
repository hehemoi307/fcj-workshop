---
title: "Nhật ký công việc - Tuần 10"
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu Tuần 10:
* Phối hợp cùng nhóm phác thảo sơ đồ kiến trúc hệ thống (Architecture Diagram), chịu trách nhiệm chính thiết kế phân lớp Edge & Delivery (Phân phối & Giao tiếp vùng biên) cho Frontend.
* Nghiên cứu tiêu chuẩn AWS Well-Architected Framework để tối ưu hóa thiết kế luồng phân phối tĩnh và tích hợp CI/CD.
* Rà soát, hợp nhất sơ đồ thành phần Frontend với hạ tầng VPC Backend của nhóm, đảm bảo tính khả thi và bám sát mã nguồn thực tế.

### Nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ chi tiết | Ngày bắt đầu | Ngày kết thúc | Tài liệu tham khảo |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 1 | - Phân tích luồng dữ liệu từ phía người dùng cuối (End-user) để phác thảo phân lớp Frontend.<br>- Sử dụng Draw.io để vẽ bản nháp các thành phần: Route 53, CloudFront, S3 (Frontend) và S3 (Media). | 22/06/2026 | 22/06/2026 | AWS Architecture Icon Set |
| 2 | - Nghiên cứu tài liệu AWS Well-Architected Framework (tập trung vào trụ cột Performance Efficiency và Security).<br>- Áp dụng lý thuyết để kiểm tra xem thiết kế CDN hiện tại đã tối ưu tốc độ và bảo mật chưa. | 23/06/2026 | 23/06/2026 | AWS Well-Architected Framework |
| 3 | - Thảo luận ghép nối sơ đồ: Đối chiếu luồng gọi API từ CloudFront (Frontend) xuyên qua Internet Gateway để đi vào Application Load Balancer / EC2 (Backend) của nhóm.<br>- Kiểm tra tính logic của các mũi tên định tuyến. | 24/06/2026 | 24/06/2026 | Sơ đồ khối hệ thống nhóm |
| 4 | - Cập nhật thêm luồng Triển khai liên tục (CI/CD) vào sơ đồ: Trực quan hóa quy trình GitHub Actions tự động build mã nguồn ReactJS và đẩy tệp tĩnh (Sync) lên Amazon S3. | 25/06/2026 | 25/06/2026 | CI/CD Architecture Patterns |
| 5 | - Hoàn thiện và chuẩn hóa giao diện bản vẽ tổng quan (Architecture Blueprint) cùng nhóm.<br>- Viết tài liệu giải thích chi tiết chức năng của từng block ở phân lớp Edge và cập nhật tiến độ lên Hugo. | 26/06/2026 | 26/06/2026 | |

### Kết quả đạt được trong tuần:

#### A. Thiết kế và chuẩn hóa kiến trúc Phân phối (Edge & Delivery Architecture)
* **Trực quan hóa luồng Frontend và CI/CD:**
  * Vẽ thành công luồng truy cập tối ưu cho khách hàng: Người dùng -> Route 53 (DNS) -> CloudFront (CDN Caching) -> S3 Bucket (ReactJS).
  * Đưa quy trình tự động hóa vào sơ đồ kiến trúc: Trình bày rõ ràng bước GitHub Actions thực hiện `npm build` và triển khai tự động lên hạ tầng lưu trữ, phản ánh đúng quy trình làm việc thực tế của nhóm.
* **Hợp nhất luồng giao tiếp chéo (Cross-layer Integration):**
  * Ghép nối thành công phân lớp Frontend với mạng VPC Backend của các thành viên khác. Xác định rõ các điểm chạm (Endpoints) và hướng mũi tên dữ liệu từ Client gọi API đi qua Load Balancer để vào Private Subnet một cách hợp lý.

#### B. Áp dụng tiêu chuẩn thiết kế (Well-Architected Alignment)
* **Tối ưu hóa hiệu suất và bảo mật:**
  * Thay vì chỉ tham khảo các bài mẫu cộng đồng, đã chủ động áp dụng các trụ cột của AWS Well-Architected Framework để thiết kế. 
  * Đảm bảo CloudFront đóng vai trò lá chắn (Edge Security), ép buộc truy cập qua HTTPS và bảo vệ S3 Bucket khỏi các truy cập trực tiếp trái phép thông qua Origin Access Control (OAC).

#### C. Thống nhất phương án thực tế (Practical Deployment Focus)
* **Loại bỏ sự rườm rà, tập trung vào tính khả thi:**
  * Thống nhất với nhóm loại bỏ ý tưởng vẽ các dịch vụ Serverless (như AWS Lambda) để xử lý ảnh upload. Quyết định áp dụng phương án lưu trữ trực tiếp file hình ảnh thú cưng vào S3 Media Bucket thông qua Pre-signed URL từ Backend. 
  * Quyết định này giúp sơ đồ kiến trúc bám sát khả năng code thực tế, giữ cho hệ thống đơn giản, dễ vận hành và bảo vệ trước hội đồng Mentor.