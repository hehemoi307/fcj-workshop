---
title: "Nhật ký công việc - Tuần 12"
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu Tuần 12:
* Hoàn thiện cấu hình giám sát (Monitoring) và kiểm thử sức chịu tải (Load Testing) cho toàn bộ hệ thống *Pet Resort & Care System* trên môi trường AWS.
* Thực hiện rà soát và tối ưu chi phí (FinOps) bằng cách dọn dẹp các tài nguyên dư thừa.
* Tổng kết hành trình 12 tuần thực tập, đóng gói tài liệu kỹ thuật và chuẩn bị slide, kịch bản Demo cho buổi nghiệm thu dự án.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :---: | :--- | :---: | :---: | :--- |
| 2 | - Kiểm thử toàn diện (End-to-End Testing): Chạy rà soát các kịch bản test tổng thể từ đầu đến cuối để đảm bảo các luồng chức năng (Đăng ký, Đặt lịch, Thanh toán) hoạt động xuyên suốt và không có độ trễ bất thường. | 06/07/2026 | 06/07/2026 | Kịch bản Test hệ thống của nhóm |
| 3 | - Giám sát & Cảnh báo: Rà soát lại các bảng điều khiển (Dashboards) trên Amazon CloudWatch.<br>- Kiểm tra các luồng cảnh báo (Alarms) để đảm bảo hệ thống luôn trong tầm kiểm soát nếu có sự cố. | 07/07/2026 | 07/07/2026 | AWS CloudWatch Docs |
| 4 | - Đánh giá chịu tải (Load/Stress Testing): Phối hợp cùng nhóm giả lập lượng truy cập lớn để kiểm tra khả năng phản hồi, mức độ ổn định của kiến trúc và sự phối hợp giữa các tài nguyên khi bị quá tải. | 08/07/2026 | 08/07/2026 | System Performance Guide |
| 5 | - Tối ưu tài nguyên (FinOps): Kiểm tra lại bảng tính chi phí (AWS Billing Console), dọn dẹp các tài nguyên thử nghiệm không còn sử dụng (snapshot cũ, bucket nháp, IP thừa) để đảm bảo chi phí nhóm không vượt ngân sách. | 09/07/2026 | 09/07/2026 | AWS Billing Console |
| 6 | - Hoàn thiện Deliverables: Cùng nhóm chốt lại tài liệu kiến trúc (Architecture Blueprint), viết báo cáo tổng kết và tập dượt kịch bản thuyết trình (Demo) cho buổi bảo vệ đồ án. | 10/07/2026 | 10/07/2026 | Project Documentation |

### Kết quả đạt được trong tuần 12:

* **Vận hành hệ thống (Ở mức đáp ứng cơ bản):** Hệ thống *Pet Resort & Care System* đã có thể vận hành ổn định trên môi trường Cloud thực tế và đáp ứng trơn tru các luồng tính năng cốt lõi. Tuy nhiên, qua quá trình kiểm thử chịu tải, nhóm nhận thấy một số điểm thắt cổ chai (bottlenecks) cần được tối ưu thêm về mặt kiến trúc nếu muốn mở rộng quy mô lớn hơn trong tương lai.
* **Giám sát & Tối ưu chi phí:** Đã thiết lập được luồng giám sát cơ bản và dọn dẹp tài nguyên hiệu quả, giữ chi phí trong mức an toàn. Mặc dù vậy, hệ thống nhật ký (logging) hiện tại vẫn còn khá rời rạc, cần tích hợp một giải pháp phân tích log tập trung chuyên sâu hơn để dễ dàng dò lỗi (debug).
* **Nhìn nhận thiếu sót & Bài học rút ra:** Khép lại 12 tuần thực tập, bản thân nhận thấy hệ thống hiện tại chủ yếu vẫn đang được triển khai và cấu hình thủ công. Việc thiếu hụt một luồng CI/CD (Triển khai liên tục) tự động hoàn toàn là một điểm yếu cần khắc phục để giảm thiểu rủi ro khi cập nhật phiên bản mới.
* **Tổng kết kỳ thực tập:** Đóng gói thành công toàn bộ tài liệu kỹ thuật và sẵn sàng tâm lý tự tin, cầu thị cho buổi bảo vệ đồ án. Những kiến thức đạt được trong kỳ thực tập này là một bệ phóng vững chắc để bản thân tiếp tục nghiên cứu sâu hơn về kiến trúc đám mây và tự động hóa trong tương lai.