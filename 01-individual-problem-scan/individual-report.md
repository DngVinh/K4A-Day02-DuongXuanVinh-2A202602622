# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

> **Quy ước bằng chứng:** Người nộp đã xác nhận đã sử dụng các dịch vụ được nêu trong phạm vi bài và xác nhận các số liệu dưới đây là quan sát thật. Các số liệu được đánh dấu `[OBSERVED — user-provided]`; loại bằng chứng được ghi rõ theo từng problem, nhưng artifact gốc chưa được đính kèm thành file trong repo.

## Thông tin cá nhân

- Họ và tên: Dương Xuân Vinh
- Mã học viên: 2A202602622
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): Người dùng phổ thông, đồng thời là sinh viên; đã sử dụng các dịch vụ thuộc phạm vi Xanh SM, VinFast, Vinhomes, Vincom và Vinpearl. Chi tiết từng sự kiện sử dụng chưa được ghi thành log trong repo.
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):
  - Đặt và theo dõi dịch vụ di chuyển trong các tình huống hằng ngày, gồm Xanh SM.
  - Tra cứu thông tin phương tiện và trạm sạc khi sử dụng VinFast.
  - Tra cứu tiện ích và kênh hỗ trợ tại Vinhomes.
  - Tìm thông tin chỗ đỗ, ưu đãi và dịch vụ tại trung tâm thương mại.
  - So sánh thông tin trước khi đặt dịch vụ nghỉ dưỡng hoặc giải trí.

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = problem cụ thể + actor + bối cảnh + trạng thái bằng chứng + cách đo. Số liệu do người nộp tự ghi nhận được đánh dấu `[OBSERVED — user-provided]`; nếu chưa có quan sát hoặc nguồn đối chiếu thì dùng `TO-VALIDATE` và nêu phép đo cần thực hiện.

| # | Lăng kính | Problem / giả thuyết (actor + context) | Ai chịu ảnh hưởng? | Bằng chứng hiện có, impact sơ bộ và cách đo |
|---|---|---|---|---|
| 1 | Pain từ người khác / Tốn thời gian | Người đặt Xanh SM tại khu đô thị hoặc địa điểm nhiều lối vào có thể không xác định được điểm đón đủ rõ, dẫn đến phải liên lạc hoặc điều chỉnh thủ công. | Người đặt xe, tài xế; bộ phận hỗ trợ nếu phát sinh sự cố | `[OBSERVED — user-provided]`: 4/10 chuyến gần nhất, phát sinh 4–8 phút; 3/4 lần phải gọi/nhắn; đổi điểm 2 lần, không huỷ. Bằng chứng: lịch sử cuộc gọi và lịch sử chuyến. |
| 2 | Lặp lại / Tốn thời gian | Người dùng VinFast có thể phải tự đối chiếu nhiều thông tin để chọn trạm sạc còn phù hợp với tuyến đường và tình trạng pin. | Người dùng VinFast, người lái | `[OBSERVED — user-provided]`: 5 lần, 6–12 phút/lần; so sánh 3–5 trạm; đổi lựa chọn 3/5 lần; đi vòng 2/5 lần. Bằng chứng: lịch sử tìm kiếm/bản đồ. |
| 3 | AI có thể tốt hơn / Tốn thời gian | Người dùng VinFast có thể khó cân bằng quãng đường, mức pin, tình trạng trạm và thời gian chờ khi chọn phương án sạc. | Người dùng VinFast, người lái | `[OBSERVED — user-provided]`: 4 lần, 8–15 phút/lần; mức pin 18–32%; đổi trạm 2/4 lần vì thời gian chờ cao hoặc trạm lệch tuyến. Bằng chứng: hành trình và mức pin. |
| 4 | Lặp lại | Người dùng xe VinFast có thể gặp khó khăn khi chuẩn bị thông tin và chọn khung giờ đặt lịch bảo dưỡng. | Người dùng xe VinFast, nhân viên xưởng dịch vụ | `[OBSERVED — user-provided]`: 3 lần, 9–14 phút/lần; sửa/bổ sung thông tin 2/3 lần; thêm 2–4 trường; đổi khung giờ 1/3 lần. Bằng chứng: lịch sử đặt lịch. |
| 5 | Pain từ người khác / Lặp lại | Người dùng dịch vụ Vinhomes có thể không biết chọn kênh hoặc loại yêu cầu nào khi báo hỏng tiện ích hay sự cố trong khu đô thị. | Người dùng/cư dân, ban quản lý, kỹ thuật viên | `[OBSERVED — user-provided]`: 5 yêu cầu, 7–11 phút/yêu cầu; bị hỏi bổ sung 3/5 lần; chuyển bộ phận 2/5 lần. Bằng chứng: ticket/chat. |
| 6 | Tốn thời gian | Người dùng dịch vụ Vinhomes có thể phải hỏi nhiều nơi để biết tiện ích đang mở, vị trí và quy định sử dụng. | Người dùng/cư dân, khách của cư dân | `[OBSERVED — user-provided]`: 6 lần, 5–13 phút/lần; mở 2–4 nguồn; hỏi người khác 3/6 lần; thông tin không thống nhất 2/6 lần. Bằng chứng: lịch sử tìm kiếm/chat. |
| 7 | Tốn thời gian / Pain từ người khác | Người đến Vincom có thể khó tìm khu vực đỗ xe hoặc lối vào phù hợp trong giờ cao điểm. | Khách đến Vincom, nhân viên bảo vệ | `[OBSERVED — user-provided]`: 5 lần, 8–18 phút từ cổng đến chỗ đỗ; hỏi bảo vệ 3/5 lần; đổi hướng/tầng 4/5 lần. Bằng chứng: thời gian hành trình. |
| 8 | Lặp lại / AI có thể tốt hơn | Người dùng có thể khó so sánh ưu đãi và điều kiện áp dụng giữa các dịch vụ Vin trước khi mua. | Khách hàng, gia đình/nhóm đi cùng | `[OBSERVED — user-provided]`: 4 lần, 12–22 phút/lần; mở 3–6 nguồn; hiểu nhầm điều kiện 2/4 lần. Bằng chứng: screenshot/notes. |
| 9 | Tốn thời gian | Người đặt dịch vụ nghỉ dưỡng hoặc giải trí có thể phải nhập lại thông tin khi chuyển từ tìm hiểu sang đặt dịch vụ. | Khách đặt phòng/vé, nhân viên chăm sóc khách hàng | `[OBSERVED — user-provided]`: 5 booking flow; nhập lại 4/5 lần, 3–7 trường; quay lại bước trước 2/5 lần; thêm 4–9 phút. Bằng chứng: screen recording. |
| 10 | AI có thể tốt hơn / Pain từ người khác | Khi cần hỗ trợ, khách hàng có thể không biết kênh phù hợp và phải lặp lại bối cảnh khi chuyển giữa các bộ phận. | Khách hàng, tổng đài/chăm sóc khách hàng | `[OBSERVED — user-provided]`: 5 case; bị chuyển 1–3 lần/case; kể lại vấn đề 4/5 case; đến owner mất 10–26 phút; gửi lại thông tin 3/5 case. Bằng chứng: chat/call log. |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: “Hãy gợi ý các problem cụ thể trong hệ sinh thái Vingroup theo 4 lăng kính, mỗi problem có actor, workflow và cách đo; không bắt đầu bằng ý tưởng xây Agent.”
- Ý dùng được: Các hypothesis về xác nhận điểm đón Xanh SM, chọn trạm sạc VinFast và báo sự cố Vinhomes vì đều có thể thu hẹp thành một workflow cụ thể để validation.
- Ý cần thận trọng: Các con số được người nộp xác nhận là quan sát thật và có nguồn bằng chứng tương ứng. Report không suy rộng chúng thành claim cho toàn bộ người dùng; khi nộp chính thức nên đính kèm hoặc lưu giữ bản che thông tin nhạy cảm của các artifact gốc.

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + kế hoạch đo cụ thể
- [x] Dùng cả 4 lăng kính
- [x] Không có dòng chỉ viết chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Evidence hiện có | Điều còn chưa chắc |
|---|---|---|---|---|
| 1 | Xác nhận điểm đón Xanh SM | Workflow hẹp, bottleneck nằm ở một điểm chuyển giao và có thể so sánh phương án non-AI với AI hỗ trợ ngôn ngữ. | `[OBSERVED — user-provided]`: 4/10 chuyến, 4–8 phút phát sinh, 3/4 lần liên lạc, đổi điểm 2 lần. Bằng chứng: lịch sử cuộc gọi và lịch sử chuyến. | Cần phân biệt nguyên nhân chính là dữ liệu bản đồ, mô tả điểm đón hay giao tiếp giữa khách và tài xế. |
| 2 | Chọn trạm sạc VinFast | Có các biến số rõ gồm mức pin, quãng đường, tình trạng trạm và thời gian chờ; có thể thiết kế phép đo trước/sau. | `[OBSERVED — user-provided]`: 5 lần, 6–12 phút/lần, đổi lựa chọn 3/5 lần, đi vòng 2/5 lần. Bằng chứng: lịch sử tìm kiếm/bản đồ. | Cần tách phần dữ liệu thời gian thực khỏi phần gợi ý lựa chọn trạm. |
| 3 | Báo và theo dõi sự cố Vinhomes | Có nhiều actor và handoff; dễ chỉ ra boundary giữa form/rule, AI và người xử lý. | `[OBSERVED — user-provided]`: 5 yêu cầu, 7–11 phút/yêu cầu, bị hỏi bổ sung 3/5 lần, chuyển bộ phận 2/5 lần. Bằng chứng: ticket/chat. | Cần thống nhất kênh tiếp nhận và loại yêu cầu được đưa vào pilot. |

### Scorecard sơ bộ trước validation

Điểm 1–5 dưới đây là đánh giá để ưu tiên, không thay thế bằng chứng gốc. Evidence được chấm dựa trên số liệu và loại nguồn người nộp đã cung cấp; artifact gốc chưa được đính kèm trong repo.

| Candidate | Actor clarity | Workflow observability | Bottleneck clarity | Evidence strength | Impact measurability | Lab scope | Non-AI comparability | AI-fit investigability | Validation feasibility | Personal familiarity | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Xác nhận điểm đón Xanh SM | 4 | 4 | 4 | 4 | 4 | 5 | 5 | 3 | 5 | 5 | 43 |
| Chọn trạm sạc VinFast | 4 | 3 | 3 | 4 | 4 | 4 | 5 | 3 | 4 | 5 | 39 |
| Báo và theo dõi sự cố Vinhomes | 4 | 4 | 4 | 4 | 4 | 4 | 5 | 3 | 4 | 5 | 41 |

**Kết luận:** Xác nhận điểm đón Xanh SM được xếp thứ nhất vì evidence định lượng rõ nhất trong ba card, scope nhỏ, workflow dễ quan sát và có phương án non-AI để so sánh. Cần giữ nguyên thứ hạng nếu artifact gốc đối chiếu được với các số liệu đã ghi.

### Card muốn pitch nhất

**Card tôi muốn pitch nhất:** Problem Card #1 — Xác nhận điểm đón Xanh SM.

**Vì sao:** Đây là card có scope hẹp nhất, bottleneck nằm ở một handoff cụ thể và baseline đã có cách đo rõ. Card cũng cho phép nhóm so sánh process fix/rule với AI hỗ trợ mà không cần trao quyền tự động thay đổi điểm đón.

**Câu hỏi tôi muốn nhóm challenge:**

1. Pain chính nằm ở dữ liệu điểm đón, cách khách diễn đạt hay việc tài xế không có cùng quy ước vị trí?
2. Rule chuẩn hóa cổng/lối vào đã đủ giảm phần lớn liên lạc thủ công chưa, trước khi cần AI?

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Xác nhận điểm đón Xanh SM

```text
Problem 1 câu: [OBSERVED] Người đặt Xanh SM tại khu đô thị hoặc địa điểm nhiều lối vào gặp bottleneck ở việc xác định và truyền đạt điểm đón, dẫn đến liên lạc thủ công, đổi điểm và kéo dài thời gian chờ.

Actor: Người đặt xe và tài xế; bộ phận hỗ trợ chỉ tham gia nếu phát sinh sự cố. Người nộp đã xác nhận đã dùng Xanh SM; vai trò và bối cảnh của từng chuyến cần được ghi lại khi validation.

Thời điểm / bối cảnh: Khi đặt xe tại khu đô thị, trung tâm thương mại, cổng trường hoặc tòa nhà có nhiều lối vào.

Current workflow 3-7 bước:
1. Mở ứng dụng và nhập điểm đến.
2. Chọn vị trí đón trên bản đồ.
3. Thêm ghi chú hoặc gọi cho tài xế để mô tả cổng/lối vào.
4. Chờ tài xế xác nhận và di chuyển đến điểm đón.
5. Nếu hai bên hiểu khác nhau, khách điều chỉnh vị trí hoặc huỷ/chờ chuyến mới.

Bottleneck: Điểm chuyển giao giữa pin bản đồ/ghi chú của khách và việc tài xế tìm đúng vị trí ở bước 3–4. Cần kiểm tra xem nguyên nhân chính là dữ liệu điểm đón, cách diễn đạt hay việc hai bên không có cùng quy ước vị trí.

Impact: `[OBSERVED — user-provided]`: trong 4/10 chuyến gần nhất phát sinh khoảng 4–8 phút; 3/4 lần phải gọi/nhắn; đổi điểm 2 lần và không huỷ chuyến. Quan sát cho thấy pin bản đồ xác định đúng khu vực nhưng chưa đủ để khách và tài xế thống nhất cửa đón. `[INFERENCE]` Nếu lặp lại trong giờ đông hoặc tại địa điểm nhiều cổng, bottleneck có thể làm tăng thời gian chờ và rủi ro đón không thành công; cần đo riêng, không suy rộng từ 10 chuyến.

Success metric:
- Baseline: 4/10 chuyến phát sinh vấn đề; trong nhóm chuyến có vấn đề, thời gian phát sinh 4–8 phút, 3/4 lần phải gọi/nhắn và đổi điểm 2 lần.
- Target đề xuất: giảm số chuyến phải gọi/nhắn từ 3/4 xuống tối đa 1/4 chuyến có điểm đón phức tạp; giảm thời gian phát sinh so với khoảng 4–8 phút hiện tại; không tăng tỷ lệ huỷ hoặc đón không thành công.
- Measurement: ghi thời gian, số lần gọi/nhắn, số lần đổi điểm, huỷ chuyến và kết quả của từng chuyến.
- Guardrail: tỷ lệ huỷ chuyến và tỷ lệ tài xế phải tìm lại vị trí không được tăng.

Non-AI alternative: Cho phép chọn cổng/lối vào được chuẩn hoá, lưu điểm đón ưa thích, hiển thị vùng đón hợp lệ và thêm ảnh/biển hiệu cho từng điểm.

AI hypothesis:
- AI can: chuẩn hoá ghi chú tự do và gợi ý một cổng/lối vào từ danh sách điểm đón đã biết.
- AI cannot: tự đổi điểm đón, tự gửi chỉ dẫn chưa được xác nhận hoặc cam kết thời gian đón.
- Human must: khách xác nhận gợi ý; tài xế vẫn là người xác nhận khả năng tiếp cận; bộ phận hỗ trợ xử lý ngoại lệ.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[ ] Agent
[x] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — thời lượng baseline cần đo

[1 Chọn điểm trên bản đồ] → [2 Thêm ghi chú] → [3 Tài xế tìm điểm đón] → [4 Nhắn/gọi và điều chỉnh]  <-- bottleneck: handoff vị trí

FUTURE STATE — target thiết lập sau khi đo baseline

[1 Chọn vùng/cổng chuẩn] → [2 Rule kiểm tra pin/ghi chú] → [3 AI gợi ý khi ghi chú mơ hồ] → [4 Khách xác nhận + tài xế nhận hướng dẫn]  <-- human boundary

Human boundary: Không có gợi ý nào được gửi hoặc thay đổi điểm đón nếu khách chưa xác nhận.

Fallback: Gợi ý sai, thiếu dữ liệu hoặc tài xế không tiếp cận được → bỏ gợi ý, chọn điểm đón thủ công hoặc gọi tài xế.
```

File ảnh riêng: không có; workflow được trình bày bằng ASCII ngay trong report để không tạo artifact ngoài phạm vi chỉnh sửa.

**Điều cần validate:**
- Lịch sử cuộc gọi và lịch sử chuyến có đối chiếu được 4/10 chuyến và các lần liên lạc/đổi điểm không?
- Điểm nghẽn có lặp lại ở nhiều địa điểm hay chỉ là một trường hợp cá biệt?
- Chuẩn hoá điểm đón bằng rule đã giải quyết phần lớn pain chưa, trước khi thử AI?

---

#### Problem Card #2 — Chọn trạm sạc VinFast phù hợp

```text
Problem 1 câu: [OBSERVED] Người dùng VinFast trong một hành trình cụ thể gặp bottleneck ở việc chọn trạm sạc phù hợp với mức pin, quãng đường, tình trạng trạm và thời gian chờ, dẫn đến đổi phương án hoặc đi vòng.

Actor: Người dùng VinFast đang cần sạc; người lái là người chịu trách nhiệm quyết định cuối cùng. Người nộp đã xác nhận đã dùng VinFast; cần xác định trải nghiệm cụ thể có phải luồng tìm trạm sạc hay không.

Thời điểm / bối cảnh: Trước hoặc trong chuyến đi, đặc biệt khi pin thấp hoặc đi qua khu vực chưa quen.

Current workflow 3-7 bước:
1. Ước lượng mức pin và quãng đường còn lại.
2. Mở bản đồ/ứng dụng để tìm các trạm gần tuyến đường.
3. Kiểm tra loại trạm, khả năng tương thích và tình trạng chỗ sạc.
4. So sánh thời gian đi vòng và thời gian chờ.
5. Chọn trạm; nếu đến nơi không còn chỗ thì quay lại bước 2.

Bottleneck: Bước 3–4 — người lái phải tự tổng hợp dữ liệu trạm, tuyến đường và mức pin để chọn một phương án; cần tách vấn đề thiếu dữ liệu khỏi vấn đề xếp hạng lựa chọn.

Impact: `[OBSERVED — user-provided]`: trong 5 lần, thời gian chọn trạm là 6–12 phút; phải so sánh 3–5 trạm/lần; đổi lựa chọn 3/5 lần và đi vòng 2/5 lần, khoảng 2–4 km. Quan sát cho thấy người dùng phải tự cân bằng khoảng cách, tình trạng trạm và thời gian chờ. `[INFERENCE]` Nếu thông tin tình trạng trạm không kịp thời, việc chọn sai có thể làm tăng quãng đường, thời gian chờ hoặc rủi ro pin thấp; cần kiểm tra bằng dữ liệu trạm và hành trình thực tế.

Success metric:
- Baseline: 5 lần quan sát; thời gian chọn trạm 6–12 phút/lần; đổi lựa chọn 3/5 lần; đi vòng 2/5 lần, khoảng 2–4 km.
- Target đề xuất: giảm thời gian ra quyết định ít nhất 30%, giảm số lần đổi lựa chọn từ 3/5 xuống tối đa 1/5 và không tạo hành trình khiến người dùng thiếu pin.
- Measurement: ghi mức pin, các trạm được xem, thời gian chọn, khoảng cách đi vòng, thời gian chờ và việc có phải đổi trạm hay không.
- Guardrail: không có khuyến nghị khiến người lái không đủ pin hoặc bỏ qua cảnh báo dữ liệu trạm không chắc chắn.

Non-AI alternative: Bộ lọc theo loại trạm, công suất, khoảng cách, tình trạng chỗ sạc và nút so sánh các trạm trên cùng tuyến.

AI hypothesis:
- AI can: tổng hợp các tiêu chí đã có và giải thích trade-off giữa quãng đường, mức pin và thời gian chờ.
- AI cannot: tự đảm bảo tình trạng trạm theo thời gian thực, tự điều hướng sang phương án mới hoặc quyết định thay người lái.
- Human must: kiểm tra dữ liệu đầu vào và xác nhận trạm trước khi di chuyển.

Quick gut:
[ ] No AI / process fix
[x] Rule
[ ] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — thời lượng baseline cần đo

[1 Ước lượng mức pin] → [2 Tìm các trạm trên tuyến] → [3 Kiểm tra tình trạng và tương thích] → [4 So sánh tuyến/chờ]  <-- bottleneck: tổng hợp tiêu chí

FUTURE STATE — target thiết lập sau khi đo baseline

[1 Rule lọc theo dữ liệu chắc chắn] → [2 Bảng so sánh/xếp hạng minh bạch] → [3 AI giải thích trade-off nếu cần] → [4 Người lái review và chọn]  <-- human boundary

Human boundary: Người lái kiểm tra mức pin, dữ liệu trạm và tuyến trước khi xác nhận; không tự động thực hiện hành động có rủi ro.

Fallback: Dữ liệu trạm không cập nhật hoặc gợi ý không an toàn → hiển thị dữ liệu hiện có, cảnh báo độ tin cậy và để người dùng chọn thủ công.
```

File ảnh riêng: không có; workflow được trình bày bằng ASCII ngay trong report để không tạo artifact ngoài phạm vi chỉnh sửa.

**Điều cần validate:**
- Lịch sử tìm kiếm/bản đồ có đối chiếu được 5 lần, số trạm đã so sánh và số lần đổi lựa chọn không?
- Dữ liệu tình trạng trạm có đủ tin cậy để đưa vào phép đo không?
- Bộ lọc và bảng so sánh cố định đã giải quyết phần lớn pain trước khi cần AI chưa?

---

#### Problem Card #3 — Báo và theo dõi sự cố tại Vinhomes

```text
Problem 1 câu: [OBSERVED] Người dùng Vinhomes khi báo sự cố tại căn hộ hoặc khu vực chung gặp bottleneck ở việc chọn đúng kênh và cung cấp đủ thông tin, dẫn đến bị hỏi bổ sung hoặc chuyển bộ phận.

Actor: Người dùng/cư dân Vinhomes là người tạo yêu cầu; ban quản lý là owner phân loại/handoff; kỹ thuật viên là người xử lý. Người nộp đã xác nhận đã dùng Vinhomes; cần xác định vai trò thực tế trong luồng báo sự cố.

Thời điểm / bối cảnh: Khi phát hiện sự cố tại căn hộ, khu tiện ích, bãi xe hoặc khu vực chung.

Current workflow 3-7 bước:
1. Phát hiện và chụp ảnh sự cố.
2. Tìm kênh liên hệ hoặc biểu mẫu phù hợp.
3. Viết mô tả, chọn loại sự cố và gửi yêu cầu.
4. Chờ ban quản lý phân loại/chuyển việc.
5. Kiểm tra trạng thái hoặc hỏi lại nếu chưa có phản hồi.

Bottleneck: Bước 2–3 — cư dân phải tự chọn kênh, loại sự cố và nội dung cần cung cấp; đây là điểm handoff dễ tạo yêu cầu thiếu hoặc sai tuyến.

Impact: `[OBSERVED — user-provided]`: trong 5 yêu cầu, thời gian tạo là 7–11 phút; bị hỏi bổ sung 3/5 lần và chuyển bộ phận 2/5 lần. Thông tin thường thiếu là vị trí chính xác, ảnh và mức độ khẩn cấp; bottleneck xuất hiện trước khi kỹ thuật viên bắt đầu xử lý. `[INFERENCE]` Nếu thiếu thông tin tiếp tục xảy ra, thời gian đến đúng owner và thời gian xử lý có thể kéo dài; cần tách riêng delay do tạo ticket khỏi delay sau handoff.

Success metric:
- Baseline: 5 yêu cầu; thời gian tạo 7–11 phút/yêu cầu; bị hỏi bổ sung 3/5 lần và chuyển bộ phận 2/5 lần.
- Target đề xuất: giảm số yêu cầu bị hỏi bổ sung từ 3/5 xuống tối đa 1/5 và giảm số lần chuyển bộ phận từ 2/5 xuống tối đa 1/5, không làm giảm chất lượng thông tin.
- Measurement: lấy các yêu cầu cùng một nhóm sự cố, ghi thời gian, trường thông tin thiếu, số lần chuyển tuyến và số lần cư dân hỏi lại.
- Guardrail: không tự động đóng yêu cầu hoặc gán trách nhiệm cuối cùng nếu ban quản lý chưa xác nhận.

Non-AI alternative: Form có danh mục sự cố rõ, checklist thông tin bắt buộc, trạng thái xử lý thống nhất và mã theo dõi cho từng yêu cầu.

AI hypothesis:
- AI can: gợi ý nhóm sự cố, phát hiện thông tin còn thiếu trong mô tả/ảnh và soạn bản nháp yêu cầu.
- AI cannot: tự kết luận nguyên nhân kỹ thuật, tự gán trách nhiệm cuối cùng hoặc tự đóng yêu cầu.
- Human must: cư dân xác nhận nội dung trước khi gửi; ban quản lý xác nhận phân loại, mức ưu tiên và handoff.

Quick gut:
[ ] No AI / process fix
[x] Rule
[ ] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — thời lượng baseline cần đo

[1 Chụp ảnh và ghi mô tả] → [2 Tìm kênh] → [3 Chọn loại sự cố, bổ sung thông tin và gửi] → [4 Theo dõi/hỏi lại]  <-- bottleneck: phân loại và handoff

FUTURE STATE — target thiết lập sau khi đo baseline

[1 Chụp ảnh + mô tả] → [2 Form/rule kiểm tra trường bắt buộc] → [3 AI chỉ gợi ý phân loại hoặc thông tin thiếu nếu rule chưa đủ] → [4 Cư dân review + gửi]  <-- human boundary

Human boundary: Cư dân duyệt nội dung trước khi gửi; ban quản lý duyệt phân loại, mức ưu tiên và người nhận xử lý.

Fallback: Phân loại không chắc hoặc ảnh không đủ rõ → chuyển sang form tổng quát, giữ nguyên bằng chứng đầu vào và yêu cầu ban quản lý phân loại thủ công.
```

File ảnh riêng: không có; workflow được trình bày bằng ASCII ngay trong report để không tạo artifact ngoài phạm vi chỉnh sửa.

**Điều cần validate:**
- Ticket/chat có đối chiếu được 5 yêu cầu, các lần bị hỏi bổ sung và chuyển bộ phận không?
- Sự cố thường bị kẹt ở chọn kênh, thiếu thông tin hay ở khâu xử lý sau handoff?
- Form/rule và trạng thái theo dõi có đủ giải quyết pain trước khi thêm AI không?

---

---

## Evidence cần xác minh trước khi nộp chính thức

| Claim cần kiểm tra | Trạng thái | Cần kiểm bằng gì |
|---|---|---|
| Người nộp có điểm chạm với Xanh SM, VinFast, Vinhomes, Vincom và Vinpearl | `SUPPORTED — user confirmation` | Chọn một bối cảnh cụ thể của từng dịch vụ và đối chiếu với lịch sử sử dụng hoặc lời kể có thể kiểm tra |
| Các số liệu tần suất, thời gian và tỷ lệ trong bảng scan và Top 3 | `OBSERVED — user-provided` | Đối chiếu từng con số với loại artifact đã nêu; artifact gốc chưa được đính kèm trong repo nên chưa có kiểm định độc lập |
| Điểm đón Xanh SM gây phát sinh liên lạc hoặc điều chỉnh | `OBSERVED — user-provided` | Đối chiếu 10 chuyến gần nhất với lịch sử cuộc gọi/lịch sử chuyến; kiểm tra riêng 4 chuyến có vấn đề và 2 lần đổi điểm |
| Việc chọn trạm sạc VinFast tạo ra effort hoặc rủi ro đi vòng | `OBSERVED — user-provided` | Đối chiếu 5 lần với lịch sử tìm kiếm/bản đồ; kiểm tra số trạm đã so sánh, thời gian chọn, 3 lần đổi lựa chọn và 2 lần đi vòng |
| Cư dân Vinhomes gặp khó ở chọn kênh hoặc thiếu thông tin khi báo sự cố | `OBSERVED — user-provided` | Đối chiếu 5 yêu cầu với ticket/chat; kiểm tra 3 lần bị hỏi bổ sung, 2 lần chuyển bộ phận và các trường thông tin thiếu |
| Rule/process fix có giải quyết phần lớn pain trước AI không | `TO-VALIDATE` | Chạy thử thủ công với điểm đón chuẩn, bộ lọc trạm hoặc form phân loại; so sánh với workflow hiện tại bằng cùng một bộ metric |
| Baseline, target và guardrail của Top 3 | `OBSERVED baseline / TO-VALIDATE target` | Baseline lấy từ quan sát người nộp; cần xác nhận sample, định nghĩa metric và kiểm tra target/guardrail bằng một đợt đo hoặc pilot riêng |

### Self-check nộp phần 01
- [x] Có 5+ problems + top 3 Cards đủ field
- [x] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [x] Các uncertainty còn lại đã được ghi ở cuối từng Card và trong Evidence ledger
