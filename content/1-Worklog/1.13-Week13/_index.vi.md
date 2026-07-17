---
title: "Worklog Tuần 13"
weight: 13
chapter: false
pre: " <b> 1.13. </b> "
---

### Mục tiêu tuần 13:
* Khắc phục hoàn toàn các lỗi phát sinh (CORS, Mixed Content) khi triển khai thực tế trên môi trường Cloud.
* Hoàn thiện toàn bộ báo cáo thực tập , chốt và nộp lên portal
* Thực hiện bàn giao tài nguyên dự án, hồ sơ đánh giá thực tập và tham gia buổi báo cáo nghiệm thu cuối kỳ.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Sửa lỗi & Khắc phục sự cố: Rà soát log lỗi khi chạy thực tế, xử lý triệt để các lỗi kết nối Database/Cache và kiểm tra tính toàn vẹn của dữ liệu sau khi chạy thử nghiệm trên Cloud. | 13/07/2026   | 13/07/2026      | Logs của ALB & EC2/RDS                    |
| 3   | - Tối ưu hóa cấu hình DNS & CDN: Cấu hình chứng chỉ SSL/HTTPS qua ACM, cập nhật cấu hình định tuyến của CloudFront và xử lý lỗi Mixed Content khi Frontend gọi API. | 14/07/2026   | 14/07/2026      | AWS ACM, CloudFront Console               |
| 4   | - Viết Báo cáo cuối kỳ: Tập hợp nội dung công việc của 12 tuần thực tập vào báo cáo chính thức, vẽ lại sơ đồ kiến trúc hoàn thiện và cập nhật các số liệu thực nghiệm. | 15/07/2026   | 15/07/2026      | Tài liệu dự án và kết quả test            |
| 5   | - Tổng duyệt & Chạy thử: Tập dượt thuyết trình cùng các thành viên trong nhóm thực tập, tối ưu hóa slide báo cáo và kiểm tra kịch bản chạy thử (demo) dự án. | 16/07/2026   | 16/07/2026      | Kịch bản demo cuối khóa                   |
| 6   | - Hoàn thiện thủ tục: Soạn thảo biên bản bàn giao mã nguồn dự án, chuẩn bị hồ sơ đánh giá kết quả thực tập và xin chữ ký xác nhận của Mentor phụ trách. | 17/07/2026   | 17/07/2026      | Mẫu hồ sơ thực tập của AWS                |
| 2   | - Báo cáo nghiệm thu: Tham gia buổi bảo vệ báo cáo thực tập cuối khóa trước ban giám khảo AWS Vietnam, thực hiện tắt/xóa tài nguyên AWS để tránh phát sinh chi phí và kết thúc kỳ thực tập. | 20/07/2026   | 20/07/2026      | Slide báo cáo, AWS Billing Console        |

### Kết quả đạt được tuần 13:

* **Khắc phục lỗi Cloud hoàn tất:** Đã giải quyết triệt để các lỗi Mixed Content và CORS giúp ứng dụng *Pet Resort & Care System* chạy mượt mà trên môi trường Production Cloud.
* **Hoàn thiện Hồ sơ Báo cáo:** Báo cáo thực tập chi tiết và slide thuyết trình đã được hoàn thiện đúng hạn, truyền tải đầy đủ kiến thức tích lũy suốt 13 tuần.
* **Nghiệm thu thành công:** Hoàn thành xuất sắc buổi báo cáo nghiệm thu cuối kỳ trước đội ngũ Mentors của AWS Vietnam, nhận được nhiều phản hồi tích cực và đóng góp chuyên môn quý báu.
* **Bàn giao và Dọn dẹp tài nguyên:** Đã hoàn tất các thủ tục đánh giá, bàn giao mã nguồn dự án và tắt sạch các tài nguyên AWS đã tạo để đảm bảo tối ưu chi phí (giữ ngân sách an toàn).
