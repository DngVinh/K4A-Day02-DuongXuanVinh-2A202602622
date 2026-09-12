# 02 — Group Validation Notes

**Nhóm:** AInoob - Zone A
**Candidate được kiểm chứng:** Học viên phải liên tục kiểm tra nhiều nguồn để biết có lab, task hoặc deadline mới.

## Phạm vi và nguồn dữ liệu

Các ghi chú dưới đây là bản tổng hợp dữ liệu nhóm cung cấp cho bài làm. Quote và số liệu được giữ theo nội dung nhóm đã ghi nhận; file này không khẳng định đã có log hệ thống hoặc bằng chứng độc lập từ VLearn/Discord/Messenger. Khi chạy pilot, nhóm cần lưu timestamp, link nguồn và log thao tác theo cùng định nghĩa để kiểm định lại baseline.

## 1. Interview nhanh

| Mẫu | Quote nguyên văn | Tín hiệu |
|---|---|---|
| Học viên 1/3 | “Ngày nào mình cũng phải mở ít nhất VLearn với Discord để xem có thay đổi gì không.” | Phải kiểm tra nhiều nguồn để phát hiện cập nhật. |
| Học viên 2/3 | “Có hôm link workshop bị trôi khá sâu trong Discord, mình phải hỏi lại.” | Phải tìm lại hoặc hỏi lại khi thông tin khó truy xuất. |
| Học viên 3/3 | “Mình thường tự ghi deadline ra note vì sợ quên.” | Handoff từ thông báo sang hành động vẫn thủ công. |

**Tín hiệu phản bác:** 1/3 người cho rằng nếu Discord channel được tổ chức tốt thì việc kiểm tra không quá mất thời gian.

**Insight:** Pain không chỉ là “không tìm được thông tin”, mà là phải đối chiếu nhiều nguồn và xác định bản mới/chính thức.

## 2. Survey / poll

| Chỉ báo | Kết quả nhóm cung cấp |
|---|---:|
| Cỡ mẫu | 8 học viên |
| Mở từ 3 nguồn trở lên mỗi ngày | 6/8 |
| Từng hỏi lại deadline/link | 5/8 |
| Từng bỏ sót hoặc phát hiện muộn một cập nhật | 4/8 |
| Tín hiệu phản bác: tự ghi lịch nên ít bị ảnh hưởng | 2/8 |

**Cách dùng:** Dùng các chỉ báo trên làm baseline tạm thời cho pilot; không suy diễn thành tỷ lệ đại diện cho toàn bộ học viên.

## 3. Log / review seed

| Chỉ báo | Kết quả nhóm cung cấp |
|---|---:|
| Số lượt kiểm tra trung bình | 4,1 lượt/ngày |
| Số nguồn mở trong mỗi lượt | 3–4 nguồn |
| Thời gian mỗi lượt | 5–8 phút |
| Trường hợp phải tìm lại link cũ | 2 trường hợp |
| Trường hợp phát hiện muộn thay đổi workshop | 1 trường hợp |
| Missed deadline nghiêm trọng | Chưa có bằng chứng trong sample seed |

**Giới hạn:** Đây là sample seed do nhóm cung cấp, chưa có file log gốc trong repo. Trước khi dùng làm evidence cuối cùng, nhóm cần chốt định nghĩa “một lượt kiểm tra”, khoảng thời gian quan sát và cách ghi missed/late update.

## 4. Kế hoạch đo pilot

| Metric | Baseline hiện có | Cách ghi trong pilot | Guardrail |
|---|---|---|---|
| Thời gian xác định cập nhật cần hành động | 5–8 phút/lượt | Timestamp từ thông báo đầu tiên đến khi học viên xác định được bản có hiệu lực | Không bỏ link nguồn hoặc tự tạo deadline. |
| Số nguồn / vòng mở | 3–4 nguồn/lượt | Ghi từng nguồn và số lần quay lại nguồn cũ | Không gửi thông báo trùng. |
| Hỏi lại / bỏ sót / phát hiện muộn | 5/8 hỏi lại; 4/8 bỏ sót hoặc phát hiện muộn | Audit timeline và ghi từng case theo tuần | Case mâu thuẫn phải gắn `PENDING_CONFIRMATION` và được người review xử lý. |

**Target đề xuất:** giảm ít nhất 30% thời gian đối chiếu; hỏi lại không quá 2/8; phát hiện muộn không quá 1/8. Các target này chỉ được coi là đạt sau khi có log pilot lặp lại.

## 5. Research links đã kiểm tra

- [Discord — How to Use Search](https://support.discord.com/hc/en-us/articles/115000468588-How-to-Use-Search)
- [Slack — Search in Slack](https://slack.com/help/articles/202528808-Search-in-Slack%21)
- [Google Drive Help — Search for files](https://support.google.com/drive/answer/2375114?hl=en-pg)

**Kết luận research:** Search trong một nguồn có thể giảm công sức tìm lại, nhưng không tự xác định nguồn nào là deadline chính thức khi nhiều kênh mâu thuẫn. Vì vậy nhóm chọn source-of-truth + Rule + Workflow có người review; AI chỉ là lớp tóm tắt tùy chọn sau khi dữ liệu đã có link, owner và timestamp.
