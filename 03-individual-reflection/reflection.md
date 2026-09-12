# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Dương Xuân Vinh
- Mã học viên: 2A202602622
- Nhóm: AInoob - Zone A
- Candidate problem nhóm chọn: Học viên phải liên tục kiểm tra nhiều nguồn để biết có lab, task hoặc deadline mới.

> Các nội dung liên quan đến hoạt động nhóm dưới đây được điền theo vai trò, thảo luận và dữ liệu nhóm đã cung cấp; trước khi nộp, tôi sẽ đối chiếu lại với diễn biến thực tế của nhóm.

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Tôi scan 10 problem từ các điểm chạm đã dùng trong hệ sinh thái Vin, gồm Xanh SM, VinFast, Vinhomes, Vincom và Vinpearl. Tôi ghi actor, bối cảnh, tần suất/thời gian quan sát, loại bằng chứng và cách đo. | Tôi có một danh sách problem đủ rộng nhưng vẫn cụ thể, từ đó chọn được Top 3 để đi sâu. |
| Pitch Problem Card | Tôi trình bày các problem cá nhân, ưu tiên những bài có workflow rõ và đo được bottleneck. Khi pitch, tôi nói rõ actor, các bước hiện tại và điểm nghẽn thay vì nhảy thẳng sang giải pháp AI. | Nhóm có thêm các candidate cụ thể từ Xanh SM, VinFast, Vinhomes, Vincom và Vinpearl; các card được so sánh theo actor, workflow, evidence và metric. |
| Challenge bài của bạn khác | Khi nhóm thảo luận candidate theo dõi lab/task/deadline, tôi hỏi pain chính nằm ở khó tìm thông tin hay không biết nguồn nào là bản mới và chính thức. Tôi cũng challenge việc dùng Agent quá sớm vì source-of-truth và Rule có thể đã giải quyết phần lớn pain. | Nhóm thu hẹp problem vào việc đối chiếu nhiều nguồn, xác định bản mới/chính thức và chốt Workflow có human review thay vì Agent tự động. |
| Gom trùng / cluster | Tôi cùng nhóm gom các candidate có pattern giống nhau, đặc biệt các problem liên quan đến tìm kiếm, cập nhật và đồng bộ thông tin từ nhiều nguồn. | Việc cluster làm lộ pain chung của cụm thông tin phân tán, giúp nhóm không đánh giá từng ý riêng lẻ và đưa candidate theo dõi lab/task/deadline vào shortlist. |
| Chọn candidate problem | Tôi đồng ý chọn bài toán theo dõi lab/task/deadline vì đây là workflow nhiều người trong nhóm đều hiểu, actor rõ và dễ validation hơn các candidate phụ thuộc dữ liệu bên ngoài. | Nhóm chọn candidate số 1 và có thể so sánh No AI, Rule, Workflow và Agent trên cùng một bài toán. |
| Validation / research | Tôi tham gia xác định các dữ liệu cần thu thập như số nguồn phải mở, thời gian kiểm tra, số lần tìm lại thông tin và trường hợp bỏ sót cập nhật. Khi research, tôi chú ý đến pattern source-of-truth, search và timeline hơn là mặc định phải xây Agent. | Nhóm dùng interview, survey, baseline seed và các nguồn nghiên cứu để giữ pain ở mức có thể đo; các số liệu chưa có log gốc được đánh dấu là cần kiểm định thêm. |
| Workflow nhóm | Tôi tập trung vào phần workflow và metric. Cùng nhóm, tôi mô tả current flow từ lúc có thông báo mới đến khi học viên tự mở VLearn, Discord, Messenger, đối chiếu thông tin rồi ghi lại việc cần làm. | Bottleneck được chốt ở bước đối chiếu giữa nhiều nguồn; future workflow lấy source-of-truth, Rule, dedup, timeline và human review làm boundary. |
| Problem Statement | Tôi góp ý để Problem Statement không viết quá rộng kiểu “học viên có quá nhiều thông báo”, mà phải chỉ rõ actor, workflow, bottleneck, impact, metric và boundary. Những số liệu chưa được xác nhận được ghi rõ là baseline tạm thời. | Bản v0/v1 chuyển từ pain search chung sang việc xác định nguồn chính, bản cập nhật mới và deadline có hiệu lực; metric có baseline, target, cách đo và guardrail. |
| Rule / Workflow / Agent | Tôi ủng hộ chọn Workflow thay vì Agent. Rule xử lý source-of-truth, format và loại trùng; Workflow nối nhiều nguồn và tạo timeline; AI chỉ hỗ trợ tóm tắt hoặc phát hiện thay đổi sau khi dữ liệu được chuẩn hoá. | Nhóm bổ sung phương án No AI/process fix, chọn Workflow cho pilot và không cho Agent tự đọc mọi kênh hoặc tự gửi deadline. |
| Decision | Tôi tham gia chốt **Go có giới hạn** cho pilot Rule/Workflow thủ công, đồng thời giữ AI Agent ở trạng thái chưa chọn. | Quyết định dựa trên interview 3 học viên, survey 8 học viên, baseline seed và trade-off giữa effort đối chiếu với rủi ro deadline sai, spam hoặc mất link nguồn. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Phần rõ nhất của tôi là scan cá nhân: tôi chuyển các trải nghiệm sử dụng dịch vụ Vin thành problem có actor, workflow, bottleneck và cách đo. Trong phần nhóm, dấu tay của tôi nằm ở workflow và metric: xác định bottleneck là bước đối chiếu nhiều nguồn, đề xuất source-of-truth + Rule làm lõi và chỉ dùng AI hỗ trợ sau human review.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Gợi ý thêm problem trong hệ sinh thái Vingroup theo các lăng kính của worksheet. | Giúp tôi mở rộng danh sách candidate và nhìn ra các điểm chạm khác nhau. | AI dễ đề xuất pain chung chung hoặc kéo sang ý tưởng Agent khi chưa có trải nghiệm cụ thể. | Tôi chỉ giữ các problem gắn với dịch vụ mình đã dùng và ghi rõ actor, bối cảnh, số liệu quan sát cùng loại bằng chứng. |
| Problem Card | Phản biện Top 3 và ép mỗi card phải có bottleneck, metric, non-AI alternative và human boundary. | Giúp tôi phát hiện card quá rộng và tách phần AI có thể làm khỏi dữ liệu cần có sẵn. | AI có thể viết workflow nghe hợp lý nhưng chưa chắc đúng với luồng thực tế. | Tôi đối chiếu lại với trải nghiệm và hạ mức chắc chắn ở các điểm chưa có artifact gốc xuống `TO-VALIDATE`. |
| Workflow | Giúp phác thảo current/future workflow cho ba card. | Giúp nhìn rõ handoff và đặt AI ở một bước cụ thể thay vì nói “tối ưu toàn bộ”. | Nếu không kiểm soát, workflow sau dễ nhảy sang AI trước khi thử rule/process fix. | Tôi đặt phương án non-AI trước, quy định human boundary và thêm fallback khi dữ liệu thiếu hoặc gợi ý sai. |
| Research | Không dùng trong phần scan cá nhân; tôi chưa đưa nguồn bên ngoài vào để thay thế bằng chứng trải nghiệm. | — | — | Tôi giữ các claim ngoài phạm vi quan sát ở mức cần kiểm định, không biến thành fact. |
| Problem Statement | Nhờ AI phản biện 6 field của Problem Statement và chỉ ra chỗ còn mơ hồ. | Giúp tôi nhận ra metric và boundary ban đầu chưa đủ cụ thể. | AI dễ nhảy sang đề xuất Agent hoặc solution khi problem chưa được validate kỹ. | Tôi giữ problem ở mức workflow hiện tại, bổ sung source-of-truth, cách đo và human boundary trước khi nghĩ đến AI. |
| Rule / Workflow / Agent | Dùng để so sánh giả thuyết No AI / Rule / AI hỗ trợ trong Top 3. | Giúp tách việc chuẩn hoá bằng rule khỏi phần AI chỉ nên hỗ trợ giải thích hoặc chuẩn hoá ngôn ngữ. | AI có xu hướng khiến giải pháp trông phức tạp hơn pain thật. | Tôi giữ rule/process fix là phương án phải kiểm tra trước và không cho AI tự đổi điểm đón, tự chọn trạm hoặc tự đóng ticket. |
| Decision | Không dùng AI để chốt quyết định cuối của nhóm ở phần hiện có. | — | — | Tôi tự xếp Top 3 dựa trên scope, evidence, khả năng đo và mức độ quen thuộc với workflow. |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text


Điều tôi thấy khó nhất trong lab là tách problem khỏi solution. Ban đầu khi thấy thông tin nằm ở nhiều nơi, phản xạ khá tự nhiên là nghĩ ngay đến một AI assistant đọc hết các nguồn rồi nhắc việc. Sau khi nghe Top 3 của các bạn và vẽ workflow, tôi nhận ra phần quan trọng hơn là xác định nguồn nào là chính thức, thông tin nào mới nhất và ai chịu trách nhiệm cập nhật. Tôi cũng thay đổi cách nhìn về candidate này sau khi challenge việc dùng Agent quá sớm: nếu source-of-truth và Rule chưa rõ thì Agent chỉ làm hệ thống phức tạp hơn. Nếu phần nền chưa ổn định, AI có thể tóm tắt sai hoặc làm người học dùng nhầm deadline. Điều tôi học được là AI không phải mục tiêu cuối cùng; lựa chọn tốt là mức giải pháp đơn giản nhất nhưng vẫn giải quyết bottleneck và đo được kết quả. Trong nhóm, tôi đóng góp chính ở workflow và metric, giúp làm rõ bottleneck nằm ở bước đối chiếu nhiều nguồn và đề xuất human review. Vì vậy nhóm chọn Go có giới hạn cho pilot Rule/Workflow thủ công, còn Agent và tự động gửi deadline chưa được bật. Nếu làm lại, tôi sẽ thu thập baseline sớm hơn thay vì đợi đến sau khi đã chọn candidate. Tôi sẽ ghi trong vài ngày xem mỗi lần phải mở bao nhiêu nguồn, mất bao lâu và có lần nào phải hỏi lại hoặc phát hiện muộn thông tin hay không. Có dữ liệu này từ đầu sẽ giúp nhóm chấm candidate và quyết định chắc hơn.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI

