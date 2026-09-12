# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

**Tên nhóm:** AInoob - Zone A

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
|-----|-----------|-------------|---------------------------------------------------------------|
| 1 | Dương Xuân Vinh | `2A202602622` | Workflow & metric |
| 2 | Đinh Tiến Mạnh | `2A202602458` | Validation & research |
| 3 | Nguyễn Quang Minh | `2A202602440` | Cluster & Problem Statement |
| 4 | Nguyễn Minh Tuấn | `2A202602850` | Facilitator & convergence |
| 5 | Nguyễn Thế Hưng | `2A202602381` | Rule/Workflow/Agent & decision |

**Candidate problem nhóm chọn (1 câu):**

> **Candidate đã chốt:** Học viên phải liên tục kiểm tra nhiều nguồn để biết có lab, task hoặc deadline mới. Nhóm chọn hướng pilot Rule/Workflow có người review; chưa chọn Agent tự động.

### Quy tắc nguồn và đồng thuận nhóm

| Loại thông tin | Nguồn ưu tiên | Nguồn phụ | Owner đề xuất | Quy tắc khi mâu thuẫn |
|---|---|---|---|---|
| Lab / yêu cầu nộp bài | **VLearn** | Discord announcement | BTC / người phụ trách lab | VLearn là bản chính nếu có timestamp mới hơn. Nếu Discord báo đã đổi nhưng VLearn chưa cập nhật, gắn `PENDING_CONFIRMATION`. |
| Workshop / lịch / link Meet | **Discord announcement của BTC** | VLearn / Messenger nhóm | BTC / facilitator | Chỉ hợp lệ khi message có ngày giờ và link rõ; nếu có nhiều message thì dùng message mới nhất từ owner. |
| Task nội bộ nhóm | **Messenger/Discord group channel đã chốt** | Note cá nhân | Facilitator / task owner | Chỉ có hiệu lực khi có owner + deadline; thiếu một trong hai thì giữ `PENDING_CONFIRMATION`. |
| Thay đổi khẩn cấp | **Thông báo mới nhất từ owner chính thức** | Các nguồn còn lại | Owner tương ứng | Không tự suy diễn; luôn giữ link nguồn và timestamp. |

| Thành viên | Quan điểm về candidate | Lo ngại chính | Kết luận nhóm |
|---|---|---|---|
| Dương Xuân Vinh | Đồng ý vì gắn với workflow học hằng ngày và dễ đo | Scope bị kéo thành “AI đọc mọi thứ” | Source-of-truth + Rule là lõi. |
| Đinh Tiến Mạnh | Đồng ý vì validation với học viên khả thi hơn các candidate VinFast/Xanh SM | Chưa có baseline thật và owner nguồn | Ưu tiên validation + research trước pilot. |
| Nguyễn Quang Minh | Đồng ý vì có thể viết Problem Statement và metric rõ | Cần phân biệt pain do search với pain do thông tin mâu thuẫn | Giữ scope ở phát hiện thông tin mới/chính thức. |
| Nguyễn Minh Tuấn | Đồng ý candidate số 1 vì cả nhóm đều hiểu domain | Lo thông báo trùng và spam | Pilot phải có dedup + guardrail. |
| Nguyễn Thế Hưng | Đồng ý Workflow, không chọn Agent | Agent có thể hiểu sai deadline hoặc tự gửi cảnh báo sai | AI chỉ dùng cho tóm tắt/change highlight sau khi workflow ổn định. |

**Trạng thái dữ liệu:** Các bảng trên và bảng validation ở Phase 4 là dữ liệu nhóm cung cấp trong bài làm; các log định lượng cần được lưu lại theo cùng định nghĩa nếu nhóm tiếp tục pilot.

### Phân công pilot và trạng thái xác nhận owner

| Hạng mục | Owner chính thức cần xác nhận | Người phụ trách nội bộ pilot | Việc phụ trách | Trạng thái |
|---|---|---|---|---|
| Lab / yêu cầu nộp bài | BTC / người phụ trách lab | Dương Xuân Vinh + Đinh Tiến Mạnh | Kiểm tra VLearn, timestamp và ghi vào timeline | `PENDING_CONFIRMATION` — chưa có tên/kênh owner chính thức |
| Workshop / lịch / link Meet | BTC / facilitator | Nguyễn Minh Tuấn | Kiểm tra message Discord mới nhất có ngày giờ và link rõ | `PENDING_CONFIRMATION` — chưa có tên/kênh owner chính thức |
| Task nội bộ nhóm | Facilitator / task owner | Nguyễn Thế Hưng | Chỉ đưa vào timeline khi đủ owner + deadline; dedup thông báo | `PENDING_CONFIRMATION` — cần chốt task owner theo từng việc |
| Thay đổi khẩn cấp / mâu thuẫn nguồn | Owner tương ứng | Nguyễn Quang Minh | Giữ link + timestamp, gắn `PENDING_CONFIRMATION`, không tự suy diễn | `PENDING_CONFIRMATION` — cần xác nhận owner tương ứng |

---

## Phase 3 — Group Convergence: từ 9-12 candidates về 1

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Nguyễn Minh Tuấn | Học viên phải kiểm tra nhiều nguồn để biết lab, task hoặc deadline mới | Học viên | Chuyển qua lại VLearn, Discord, Messenger để tổng hợp | Pain rõ nhưng phạm vi rộng, cần chọn một workflow cụ thể. |
| 2 | Nguyễn Minh Tuấn | Tìm lại deadline, link hoặc hướng dẫn cũ khi cần | Học viên / thành viên nhóm | Search lịch sử chat khó và có thể bỏ sót thông tin | Có thể gộp với cụm tìm kiếm thông tin phân tán. |
| 3 | Dương Xuân Vinh | Đặt Xanh SM tại nơi có nhiều cửa vào nhưng không xác định rõ điểm đón | Người đặt xe và tài xế | Pin bản đồ/mô tả chưa đủ để hai bên thống nhất cửa đón | Scope hẹp, có baseline 4/10 chuyến và thời gian phát sinh 4–8 phút. |
| 4 | Dương Xuân Vinh | Chọn trạm sạc VinFast phải tự cân bằng khoảng cách, pin, tình trạng trạm và thời gian chờ | Người dùng/người lái VinFast | Tổng hợp nhiều tiêu chí và có thể phải đổi trạm hoặc đi vòng | Có metric nhưng phụ thuộc dữ liệu tình trạng trạm theo thời gian thực. |
| 5 | Đinh Tiến Mạnh | Deadline, task và cập nhật của intern bị phân tán giữa chat, email và công cụ quản lý | Intern và thành viên mới | Không biết nguồn nào là phiên bản chính của yêu cầu | Có pain rõ nhưng cần xác định owner và phạm vi nguồn. |
| 6 | Đinh Tiến Mạnh | Sau họp nhóm chưa có recap rõ về đầu việc, người phụ trách và deadline | Intern, quản lý và thành viên dự án | Thiếu bước chuẩn hoá action item và handoff sau họp | Dễ đo nhưng cần log họp hoặc ví dụ cụ thể. |
| 7 | Đinh Tiến Mạnh | Người phụ trách phải trả lời lặp lại câu hỏi về quy trình, deadline, tài liệu hoặc người liên hệ | Người hướng dẫn, quản lý nhóm, thành viên mới | Câu trả lời nằm rải rác trong tài liệu và tin nhắn cũ | Có thể gộp với cụm knowledge base/search. |
| 8 | Nguyễn Quang Minh | Học viên dễ quên hoặc nhầm deadline khi có nhiều lab và workshop | Học viên | Deadline nằm ở nhiều nguồn và thiếu timeline tập trung | Có rủi ro sai sót rõ, nhưng cần log tần suất quên/nhầm. |
| 9 | Nguyễn Quang Minh | Khó nhận ra thông báo mới đã thay đổi deadline, link meeting hoặc yêu cầu task | Học viên / thành viên nhóm | Không có cơ chế phát hiện, tóm tắt và làm nổi bật phần thay đổi | AI có thể hỗ trợ so sánh phiên bản, cần kiểm soát nguồn. |
| 10 | Nguyễn Thế Hưng | Phân loại và gắn tag thủ công cho ticket phản hồi khách hàng thiếu nhất quán | Support Specialist / Product team | Định nghĩa tag khác nhau giữa người xử lý, dẫn đến báo cáo lệch | Có thể đo thời gian 30–45 phút và tỷ lệ tag sai nếu có log. |
| 11 | Nguyễn Thế Hưng | Đọc và tóm tắt meeting transcript dài để trích action items | Scrum Master / Note Taker / người tham gia | Action item viết không rõ khiến người tham gia quên task | Có thể thử rule/template trước AI tóm tắt. |
| 12 | Nguyễn Thế Hưng | Tìm và tổng hợp case study/giải pháp tương tự cho presales | Presales / Solution team | Không tìm thấy nguồn phù hợp nên phải làm lại từ đầu | Có impact thời gian lớn nhưng cần kiểm tra phạm vi và quyền truy cập dữ liệu. |

### 3.2. Gom trùng / cluster (gom 9-12 ý thành 3-4 cụm)

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A — Tìm kiếm và đồng bộ thông tin | 1, 2, 5, 7, 8, 9 | Thông tin nằm ở nhiều nguồn, người dùng phải tự tìm, so sánh hoặc phát hiện thay đổi | Có thể giải một phần bằng source-of-truth, rule và workflow trước AI. |
| B — Handoff và thực thi sau giao tiếp | 6, 11 | Sau họp hoặc khi chuyển việc, action item/owner/deadline chưa đi theo đầy đủ | Cần tách pain do ghi nhận khỏi pain do theo dõi. |
| C — Vận hành dịch vụ Vin | 3, 4 | Người dùng phải tự xác nhận điểm/địa điểm hoặc tổng hợp nhiều tiêu chí để hoàn thành dịch vụ | Hai candidate phù hợp bối cảnh VinGroup và có workflow quan sát được. |
| D — Phân loại và tái sử dụng tri thức | 10, 12 | Tốn công phân loại hoặc tìm lại case/giải pháp tương tự | Cần dữ liệu log và quyền truy cập rõ trước khi thử AI. |

### 3.3. Shortlist (giữ 2-3 bài trả lời được 7 câu hỏi worksheet)

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| Theo dõi thông báo lab/task/deadline từ nhiều nguồn | Actor rõ; pain xuất hiện trong workflow hằng ngày của học viên; đã có interview, survey và baseline seed để thiết kế pilot source-of-truth, rule và workflow. | Cần kiểm tra lại log theo cách đo lặp lại; vẫn phải xác định owner và tránh gửi thông báo trùng. |
| Xác nhận điểm đón Xanh SM | Scope hẹp; actor và handoff rõ; có số liệu người dùng cung cấp: 4/10 chuyến, 4–8 phút phát sinh, 3/4 lần liên lạc. | Chưa có log gốc trong repo; chưa biết nguyên nhân chính là bản đồ, metadata cổng hay giao tiếp khách–tài xế. |
| Chọn trạm sạc VinFast | Có biến số cụ thể: mức pin, khoảng cách, tình trạng trạm, thời gian chờ; có thể đo thời gian chọn và đi vòng. | Dữ liệu tình trạng trạm có thể thay đổi; cần tránh để AI tạo khuyến nghị khi dữ liệu không cập nhật. |

### 3.4. Score để đồng thuận (chấm 1-5, ép nói rõ vì sao cho 5 / cho 3)

> Điểm dưới đây là điểm tổng hợp để hội tụ từ bảng candidate và ý kiến thành viên; nhóm dùng validation ở Phase 4 để quyết định pilot, không coi điểm số là bằng chứng định lượng độc lập.

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Theo dõi thông báo lab/task/deadline từ nhiều nguồn | 5 | 4 | 4 | 4 | 5 | 5 | 5 | 32 |
| Xác nhận điểm đón Xanh SM | 5 | 4 | 4 | 4 | 5 | 5 | 4 | 31 |
| Chọn trạm sạc VinFast | 4 | 4 | 4 | 4 | 4 | 5 | 4 | 29 |

**Candidate nhóm chọn (1 bài duy nhất):**

```text
Học viên phải liên tục kiểm tra nhiều nguồn để biết có lab, task hoặc deadline mới.
```

**Vì sao chọn (4-5 câu):**

```text
Candidate này có actor và workflow quen thuộc với toàn bộ nhóm: học viên phải rà nhiều nguồn để biết thông tin mới. Validation do nhóm cung cấp cho thấy 6/8 người mở từ 3 nguồn trở lên mỗi ngày, 5/8 từng phải hỏi lại deadline/link và 4/8 từng bỏ sót hoặc phát hiện muộn một cập nhật. Bài toán có phương án Rule/Workflow rõ là source-of-truth, owner, timestamp, dedup và timeline; AI chỉ nên tóm tắt thay đổi sau khi workflow nền ổn định. Nhóm đủ cơ sở để Go vào pilot nhỏ có human review, không Go vào Agent tự động.
```

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**

```text
Xác nhận điểm đón Xanh SM: pain và baseline cụ thể nhưng cần dữ liệu từ người dùng/tài xế và phụ thuộc metadata venue. Chọn trạm sạc VinFast: có nhiều biến số thời gian thực và rủi ro an toàn, nên khó kiểm chứng trong thời lượng lab. Các candidate còn lại vẫn đáng giữ ở backlog, nhưng hiện chưa có đủ evidence nhóm để thu hẹp workflow và so sánh giải pháp.
```

**Disagreement (nếu có — ai lo gì, chốt ra sao):**

```text
Dương Xuân Vinh đồng ý vì candidate gắn với workflow hằng ngày và đo được, nhưng lo scope bị kéo thành “AI đọc mọi thứ”; nhóm chốt source-of-truth + Rule là lõi. Đinh Tiến Mạnh ủng hộ vì validation học viên dễ thực hiện hơn các candidate VinFast/Xanh SM, nhưng yêu cầu baseline và owner nguồn rõ. Nguyễn Quang Minh yêu cầu phân biệt pain do search với pain do thông tin mâu thuẫn; Nguyễn Minh Tuấn lo thông báo trùng/spam; Nguyễn Thế Hưng ủng hộ Workflow và không chọn Agent vì rủi ro hiểu sai deadline. Nhóm chốt pilot có dedup, guardrail, link nguồn và human review.
```

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

| Nguồn | Số người / mẫu | Tín hiệu xác nhận (kèm quote nguyên văn) | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Interview | 3 học viên | `[OBSERVED — user-provided group table]`: “Ngày nào mình cũng phải mở ít nhất VLearn với Discord để xem có thay đổi gì không.” / “Có hôm link workshop bị trôi khá sâu trong Discord, mình phải hỏi lại.” / “Mình thường tự ghi deadline ra note vì sợ quên.” | 1/3 người cho rằng nếu Discord channel được tổ chức tốt thì việc kiểm tra không quá mất thời gian. | Thu hẹp pain: không phải đơn giản là “không tìm được thông tin”, mà là phải đối chiếu nhiều nguồn và xác định bản mới/chính thức. |
| Survey / poll | 8 học viên | `[OBSERVED — user-provided group table]`: 6/8 mở từ 3 nguồn trở lên mỗi ngày; 5/8 từng hỏi lại deadline/link; 4/8 từng bỏ sót hoặc phát hiện muộn một cập nhật. | 2/8 cho biết họ có thói quen tự ghi lịch nên ít bị ảnh hưởng hơn. | Giữ focus vào nhóm học viên phải kiểm tra nhiều nguồn; metric phải đo thời gian đối chiếu và số lần bỏ sót, không chỉ số lượng thông báo. |
| Log / ticket / review (nếu có) | Mẫu seed do nhóm cung cấp | `[OBSERVED — user-provided group table]`: trung bình 4,1 lượt kiểm tra/ngày; mỗi lượt mở 3–4 nguồn; mất 5–8 phút/lượt; 2 trường hợp phải tìm lại link cũ và 1 trường hợp phát hiện muộn thay đổi workshop. | Chưa có bằng chứng về missed deadline nghiêm trọng trong sample seed. | Dùng baseline này để thiết kế pilot; trước khi coi là evidence cuối cùng cần lưu log thật theo cùng định nghĩa. |

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text
Validation cho thấy pain chính không phải mọi hoạt động search đều khó, mà là việc học viên phải kiểm tra 3–4 nguồn, đối chiếu bản mới/chính thức và đôi khi hỏi lại hoặc tìm lại link. Nhóm chọn source-of-truth + Rule dedup/timestamp + timeline làm nền; AI chỉ được cân nhắc cho tóm tắt thay đổi sau khi người học vẫn có thể kiểm tra link gốc.
```

Bằng chứng đính kèm: [bản tổng hợp validation notes](../02-group-problem-statement-validation-notes.md). File này ghi lại dữ liệu nhóm cung cấp và quote đã dùng trong báo cáo; chưa thay thế cho ảnh/log gốc nếu giảng viên yêu cầu kiểm tra độc lập. Khi nộp chính thức nên ẩn thông tin nhạy cảm và giữ định nghĩa sample nhất quán.

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Discord Search | [Discord — How to Use Search](https://support.discord.com/hc/en-us/articles/115000468588-How-to-Use-Search-on-Discord) | Tìm lại announcement, file hoặc tin nhắn trong server bằng từ khoá, người gửi, ngày, channel và loại nội dung | Có bộ lọc giúp giảm thời gian lướt thủ công trong một nguồn | Chỉ giải quyết Discord; không biết thông tin nào là deadline chính thức nếu nhiều nguồn mâu thuẫn | Có thể chuẩn hoá từ khoá, channel và format thông báo trước khi đưa thêm AI. |
| Slack Search / nguồn tri thức tập trung | [Slack — Search in Slack](https://slack.com/help/articles/202528808-Search-in-Slack%21) | Tìm message, file, people, channel hoặc canvas và lọc kết quả | Cho thấy pattern search theo loại nội dung và bộ lọc trong một workspace | Khác hệ thống nhóm; search tốt vẫn không thay thế source-of-truth hoặc quyền truy cập đúng | Cần phân biệt “tìm được” với “biết bản mới nhất”; nên có owner và trường ngày hiệu lực. |
| Google Drive Search + source-of-truth | [Google Drive Help — Search for files](https://support.google.com/drive/answer/2375114?hl=en-pg) | Tìm file theo tên, loại, owner, vị trí hoặc điều kiện liên quan | Có thể gom tài liệu vào một nơi và lọc theo thuộc tính | Không tự đồng bộ nội dung từ VLearn/Discord/Messenger; tài liệu vẫn có thể trùng hoặc cũ | Thử một bảng/timeline chính có link về nguồn gốc, owner và ngày cập nhật; AI chỉ tóm tắt sau khi nguồn được chuẩn hoá. |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text
Nên bắt đầu bằng source-of-truth cho lab/task/deadline: một kênh hoặc bảng chính có owner, ngày hiệu lực, trạng thái và link về nguồn gốc. Workflow có thể thu thập link từ các kênh đã quy định, loại bản trùng và tạo timeline; không nên bắt đầu bằng Agent tự đọc mọi kênh hoặc tự gửi thông báo khi chưa có quy tắc ưu tiên nguồn. AI chỉ đáng thử ở lớp phụ trợ: tóm tắt thay đổi và gợi ý mục cần chú ý, luôn kèm link nguồn để người học kiểm tra.
```

> Lưu ý: không dùng số liệu AI đưa nếu không verify được link chính thức. Ghi rõ giả định chưa chắc.

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: `02-group-problem-statement-workflow.png/pdf/md`

```text
[1 Nhận thông báo mới] → [2 Mở từng nguồn: VLearn/Discord/Messenger] → [3 Tìm lab/task/deadline] → [4 Đối chiếu thông tin — bottleneck] → [5 Ghi nhớ hoặc tự ghi lại]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1 | Người đăng thông báo / hệ thống | Lab, task hoặc deadline mới | Thông báo xuất hiện ở một hoặc nhiều nguồn | Chưa có timestamp tổng hợp | Cần áp dụng bảng source-of-truth và owner tương ứng. |
| 2 | Học viên | Thông báo từ VLearn, Discord, Messenger và kênh liên quan | Mở được các nguồn cần kiểm tra | `[OBSERVED]` Trung bình 4,1 lượt/ngày; mỗi lượt mở 3–4 nguồn và mất 5–8 phút | Đây là bước lặp lại, dễ bỏ sót nguồn. |
| 3 | Học viên | Từ khoá, tiêu đề, ngày và nội dung thông báo | Danh sách lab/task/deadline cần chú ý | Nằm trong baseline 5–8 phút/lượt | Có thể tìm nhầm thông báo cũ hoặc trùng. |
| 4 | Học viên | Các kết quả từ nhiều nguồn | Một thông tin được coi là mới/chính thức | `[OBSERVED]` 5/8 từng hỏi lại deadline/link; 4/8 từng bỏ sót hoặc phát hiện muộn cập nhật | Phải đối chiếu nội dung, ngày hiệu lực và nguồn ưu tiên; đây là bottleneck chính. |
| 5 | Học viên | Thông tin đã tự tổng hợp | Note, lịch cá nhân hoặc hành động tiếp theo | Chưa có log riêng cho thời gian handoff | Handoff từ thông báo sang hành động vẫn thủ công. |
| 6 | — | — | — | — | Không dùng trong workflow thu hẹp 5 bước. |
| 7 | — | — | — | — | Không dùng trong workflow thu hẹp 5 bước. |

**Bottleneck chính (2-3 câu):**

```text
Bottleneck nằm ở bước đối chiếu: học viên phải chuyển qua lại nhiều app/kênh chat để xác định thông tin nào mới và có hiệu lực. Dữ liệu nhóm cung cấp cho thấy trung bình 4,1 lượt kiểm tra/ngày, mỗi lượt mở 3–4 nguồn trong 5–8 phút; 5/8 người từng hỏi lại deadline/link và 4/8 từng bỏ sót hoặc phát hiện muộn một cập nhật. Vì vậy pilot tập trung vào source-of-truth, timestamp, owner và dedup; log lặp lại trong pilot sẽ kiểm định target trước/sau.
```

### 5.2. Future workflow bản nhóm

Phải nhìn ra 5 thứ: bước nào máy (Rule), bước nào AI, bước nào người, boundary ở đâu, fallback khi AI sai.

```text
[1 Rule xác định nguồn chính và ngày hiệu lực] → [2 Workflow gom link/thông báo từ kênh đã quy định] → [3 Rule loại trùng và xếp theo deadline] → [4 AI tóm tắt thay đổi nếu cần] → [5 Học viên review và ghi hành động — human boundary]

Fallback: nguồn không truy cập được, thông tin mâu thuẫn hoặc AI không trích được nguồn → giữ nguyên link gốc, gắn nhãn “cần xác minh”, không tự gửi deadline và để học viên kiểm tra thủ công.
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Tổng thời gian | `[OBSERVED — user-provided]` 5–8 phút/lượt kiểm tra | Đề xuất pilot: giảm ít nhất 30%, còn khoảng 3,5–5,5 phút/lượt (`TO-VALIDATE`) | Bấm giờ từ thông báo đầu tiên đến khi học viên xác định được thông tin cần hành động. |
| Số bước | 5 bước trong workflow mô tả | 5 bước; giảm số vòng mở app và quay lại nguồn cũ | Ghi timestamp và số lần quay lại từng nguồn. |
| Số bước thủ công | `[OBSERVED — user-provided]` mỗi lượt mở 3–4 nguồn; 6/8 người mở từ 3 nguồn trở lên mỗi ngày | Một source-of-truth + workflow gom link; học viên vẫn review | Đếm số nguồn mở, copy/paste và tự ghi chú. |
| Bottleneck chính | `[OBSERVED — user-provided]` 5/8 từng hỏi lại deadline/link; 4/8 từng bỏ sót hoặc phát hiện muộn cập nhật | Giảm thời gian đối chiếu và số lần hỏi lại; target hỏi lại ≤2/8 và phát hiện muộn ≤1/8 (`TO-VALIDATE`) | Audit timeline, câu hỏi lặp lại và mẫu thông báo theo tuần. |
| Risk mới | Dùng nhầm deadline cũ, bỏ sót thay đổi hoặc nhận thông báo trùng | Không tạo deadline sai, không tăng spam và mọi tóm tắt đều có link nguồn | Kiểm tra source/date/owner và ghi false positive/negative. |

### 5.2.1. Định nghĩa metric và quy tắc ghi pilot

Để tránh trộn số liệu survey với kết quả pilot, nhóm sẽ ghi baseline và kết quả pilot theo cùng một data dictionary:

| Metric | Định nghĩa vận hành | Cách ghi / mẫu số |
|---|---|---|
| Một lượt kiểm tra | Bắt đầu khi học viên mở nguồn đầu tiên để kiểm tra một cập nhật; kết thúc khi xác định được bản chính có hiệu lực và ghi hành động tiếp theo. | Ghi `start_timestamp`, `end_timestamp`, người thực hiện và mã cập nhật. |
| Thời gian xác định cập nhật | `end_timestamp - start_timestamp`; chỉ tính các lượt có đủ timestamp. | Báo cáo trung vị và trung bình theo cùng một khoảng thời gian. |
| Số nguồn / vòng mở | Số nguồn khác nhau được mở trong một lượt, cộng số lần quay lại nguồn cũ. | Ghi tên nguồn và số lần mở; không suy ra từ số lượng thông báo. |
| Hỏi lại | Học viên phải hỏi owner hoặc thành viên khác vì chưa xác định được bản chính, deadline hoặc link có hiệu lực. | Đếm theo case có mã cập nhật, không đếm câu hỏi trao đổi không liên quan. |
| Phát hiện muộn | Cập nhật chỉ được học viên xác nhận sau timestamp phát hành bản chính hoặc sau mốc hiệu lực ghi trong nguồn. Nếu nguồn không có timestamp, gắn `PENDING_CONFIRMATION` và không tính vào target. | Ghi timestamp của nguồn, timestamp xác nhận đầu tiên và lý do muộn. |
| Trùng / cần sửa | Hai bản cùng một case hoặc một bản phải sửa owner/ngày hiệu lực/deadline sau review. | Ghi từng case và loại lỗi; không gộp trùng với bỏ sót. |

**Quy tắc so sánh:** số liệu survey `5/8` và `4/8` chỉ là baseline định hướng. Kết quả pilot phải ghi lại cohort, khoảng thời gian và mẫu số riêng; chỉ so sánh trước/sau khi các điều kiện này giống nhau. Trước khi chạy pilot, nhóm còn phải chốt khoảng thời gian quan sát và xác nhận định nghĩa “phát hiện muộn” với owner.

### 5.3. Problem Statement v0 (mỗi field 2-3 câu)

| Field | Nội dung |
|---|---|
| **Actor** | Học viên là người cần biết lab/task/deadline mới; người đăng thông báo hoặc owner môn học/nhóm là nguồn phát hành. |
| **Workflow** | Học viên nhận thông báo, mở VLearn/Discord/Messenger và kênh liên quan, tìm nội dung mới, đối chiếu ngày hiệu lực rồi tự ghi lại hành động. |
| **Bottleneck** | Học viên phải tự nối thông tin giữa nhiều nguồn và chưa có quy tắc rõ nguồn nào là bản chính, thông tin nào thay đổi và deadline nào có hiệu lực. |
| **Impact** | `[OBSERVED — user-provided group table]` 6/8 người mở từ 3 nguồn trở lên mỗi ngày, 5/8 từng hỏi lại deadline/link và 4/8 từng bỏ sót hoặc phát hiện muộn một cập nhật. `[INFERENCE]` Pain có thể làm tăng effort kiểm tra và rủi ro hành động theo thông tin cũ; chưa khẳng định missed deadline nghiêm trọng. |
| **Success Metric** | Baseline: 4,1 lượt kiểm tra/ngày; 3–4 nguồn/lượt; 5–8 phút/lượt; 5/8 hỏi lại deadline/link; 4/8 bỏ sót hoặc phát hiện muộn. Target đề xuất: giảm ít nhất 30% thời gian và số vòng kiểm tra, hỏi lại ≤2/8, phát hiện muộn ≤1/8; đo timestamp, history và audit mẫu; guardrail không tạo deadline sai, thông báo trùng hoặc mất link nguồn. |
| **Boundary** | Làm: xác định source-of-truth, gom link từ nguồn đã cho phép, phát hiện bản trùng/thay đổi và hiển thị link gốc. Không làm: tự phán đoán deadline khi nguồn mâu thuẫn, tự gửi thông báo đến toàn bộ học viên hoặc tự thay nội dung của owner. |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field nào mơ hồ: chưa biết nguồn nào là source-of-truth, “thông tin mới” được định nghĩa thế nào và pain chính là search, thông báo trùng hay thiếu quy tắc ưu tiên nguồn.
- Tôi sửa gì: thu hẹp vào việc phát hiện lab/task/deadline mới, dùng baseline nhóm cung cấp để thiết kế pilot, bổ sung measurement/guardrail và đặt source-of-truth + workflow trước AI.

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp (suy nghĩ nhanh, không thay quyết định cuối)

- Độ mơ hồ: [ ] Thấp (có đúng/sai rõ) / [x] Cao (nhiều cách trả lời vẫn OK) — Vì sao: nhiều nguồn có thể đăng cùng một thông tin, nội dung có thể thay đổi và chưa có quy tắc xác định bản chính.
- Độ phức tạp: [ ] Thấp (1-2 bước) / [x] Cao (3+ bước/nguồn, phụ thuộc nhau) — Vì sao: phải nhận thông báo, mở nhiều nguồn, tìm nội dung, đối chiếu ngày hiệu lực và chuyển thành hành động cá nhân.

**Bài toán nhóm nằm ở ô nào:**

```text
Cao mơ hồ / cao phức tạp ở workflow hiện tại; validation xác nhận việc đối chiếu nhiều nguồn là pain chính, nên phần giải pháp hạ xuống Workflow với source-of-truth và Rule làm lõi, AI chỉ là lớp tùy chọn.
```

**Vì sao (2-3 câu):**

```text
Không chỉ có một thao tác search, vì cần thu thập nhiều nguồn, xác định bản mới nhất và chuyển thông tin thành hành động. Validation hiện có chưa chứng minh Agent tự lập kế hoạch là cần thiết; nhóm nên kiểm tra source-of-truth, Rule và workflow tổng hợp trước.
```

### 6.1. So sánh No AI / Rule / Workflow / Agent (so trên cùng 1 bài)

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **No AI / process fix** | Quy ước nguồn chính, template thông báo, bảng/timeline thủ công và người review; không tự động đọc hay tóm tắt | Đủ khi số nguồn ít, thông báo có format và nhóm chấp nhận cập nhật thủ công | Vẫn tốn công kiểm tra; owner có thể quên cập nhật; khó phát hiện bản trùng | Dùng làm baseline và fallback; chưa chọn làm phương án chính vì pain nằm ở việc nối nhiều nguồn. |
| **Rule** | Quy định một source-of-truth, trường bắt buộc gồm loại thông tin, owner, ngày hiệu lực, deadline và link nguồn; loại bản trùng theo mã/thời gian | Đủ cho thông báo có format chuẩn và nguồn đã được quy định | Owner quên cập nhật, nguồn mâu thuẫn hoặc thông báo không theo format | Dùng ở bước chuẩn hoá và kiểm tra trước khi thêm AI. |
| **Workflow** | Thu thập từ kênh cho phép → gắn source/date/owner → phát hiện trùng/thay đổi → đưa vào timeline → học viên review | Đủ khi cần nối nhiều nguồn và vẫn giữ người chịu trách nhiệm xác nhận | Cần cấu hình quyền truy cập và xử lý ngoại lệ; có thể còn bước review thủ công | **Chọn cho pilot** ở luồng theo dõi lab/task/deadline. |
| **Agent** | Tự đọc mọi kênh, tự phán đoán thông báo mới nhất, tóm tắt và tự gửi nhắc việc | Chỉ cân nhắc khi workflow có nguồn chuẩn và có nhiều nhánh cần xử lý | Bỏ sót nguồn, hiểu sai deadline, lộ thông tin hoặc gửi cảnh báo sai | Chưa chọn; chỉ thử AI tóm tắt có trích link sau khi workflow nền ổn định. |

**5 câu hỏi chốt (trả lời câu đầy đủ):**
1. Chưa thể kết luận Rule giải được 70–80% case chỉ từ mẫu hiện tại; nhóm đã có interview, survey và baseline seed nhưng vẫn sẽ đo trên các thông báo lab/task/deadline trong cùng một khoảng thời gian.
2. Luồng chuẩn có thể đi một đường với nguồn đã quy định, nhưng phải có nhánh khi nguồn mâu thuẫn, không truy cập được hoặc nội dung không có ngày hiệu lực.
3. Chưa có bằng chứng cần Agent tự lập kế hoạch và gọi tool; bài toán hiện phù hợp hơn với source-of-truth, Rule và Workflow có người review.
4. Học viên hoặc owner thông báo phát hiện sai ở bước review; owner nguồn chịu trách nhiệm sửa bản chính, còn hệ thống không tự thay deadline hay gửi cảnh báo chưa có link nguồn.
5. Có thể hạ từ Agent xuống Workflow rồi Rule: pilot bắt đầu bằng Rule + timeline tập trung, chỉ thêm AI nếu log cho thấy phần tóm tắt/thay đổi vẫn là bottleneck.

**Mức chọn:**

```text
[Workflow]
```

**Vì sao chọn (3-4 câu):**

```text
Nhóm chọn Workflow vì pain nằm ở việc nối nhiều nguồn và chuyển thông báo thành một danh sách hành động, không chỉ ở thao tác search. Workflow cho phép Rule xác định source-of-truth, gắn owner/ngày hiệu lực và xử lý bản trùng trước khi học viên review. AI chỉ là can thiệp tùy chọn để tóm tắt thay đổi hoặc làm nổi bật thông tin, luôn kèm link nguồn. Cách này giữ được quyền xác nhận của owner/học viên và có thể rollback về bảng/timeline thủ công.
```

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**

```text
Rule thuần có thể xử lý format chuẩn và bản trùng nhưng chưa đủ khi phải nối nhiều kênh, phát hiện thay đổi và chuyển thành timeline. Nhóm không chọn Agent vì chưa có evidence về nhu cầu tự lập kế hoạch, trong khi hậu quả của gợi ý sai là bỏ sót hoặc dùng nhầm deadline.
```

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | Học viên là người cần biết lab/task/deadline mới; owner môn học hoặc người đăng thông báo là nguồn phát hành và chịu trách nhiệm về nội dung. |
| **Workflow** | Nhận thông báo → mở VLearn/Discord/Messenger và kênh liên quan → tìm nội dung mới → đối chiếu ngày hiệu lực/nguồn → ghi lại hành động. |
| **Bottleneck** | Học viên phải tự nối nhiều nguồn và chưa có quy tắc rõ nguồn nào là bản chính, nội dung nào thay đổi và deadline nào có hiệu lực. |
| **Impact** | `[OBSERVED — user-provided group table]` trung bình 4,1 lượt kiểm tra/ngày; mỗi lượt mở 3–4 nguồn và mất 5–8 phút; có 2 trường hợp tìm lại link cũ và 1 trường hợp phát hiện muộn thay đổi workshop. `[INFERENCE]` Việc đối chiếu nhiều nguồn có thể làm chậm hành động tiếp theo; cần tiếp tục đo trên log thật. |
| **Success Metric** | Baseline: 4,1 lượt/ngày, 3–4 nguồn/lượt, 5–8 phút/lượt, 5/8 hỏi lại và 4/8 bỏ sót/phát hiện muộn. Target đề xuất: giảm 30% thời gian đối chiếu; timeline chính có link nguồn, owner và ngày hiệu lực; guardrail không tạo deadline sai, spam hoặc bỏ sót cập nhật quan trọng. |
| **Boundary** (làm / không làm) | Làm source-of-truth, gom link từ nguồn được phép, gắn owner/ngày hiệu lực, phát hiện trùng/thay đổi và hiển thị link gốc. Không làm tự phán đoán deadline mâu thuẫn, tự sửa thông báo của owner hoặc tự gửi cảnh báo diện rộng khi chưa review. |
| **AI intervention point** (can thiệp sau bước nào, trước bước nào) | Sau khi Workflow đã thu thập và gắn nguồn/ngày hiệu lực, trước bước học viên review: AI chỉ tóm tắt thay đổi hoặc gợi ý mục cần chú ý, luôn kèm link gốc. |
| **Mức chọn** (Rule / Workflow / Agent + 1 câu vì sao) | Workflow — vì cần nối nhiều nguồn, Rule ưu tiên/bắt buộc trường và bước review; chưa có bằng chứng cần Agent tự lập kế hoạch. |
| **Rủi ro & người thật kiểm tra** (rủi ro lớn nhất + ai kiểm tra bằng cách nào) | Rủi ro lớn nhất là tóm tắt sai hoặc chọn nhầm deadline. Owner thông báo kiểm tra bản chính; học viên review trước khi hành động; hệ thống giữ link, gắn “cần xác minh” khi nguồn mâu thuẫn và rollback về timeline thủ công. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | Yes | Actor và 5 bước workflow đã rõ; bảng nguồn đã xác định kênh ưu tiên, nguồn phụ và owner đề xuất cho từng loại thông tin. |
| Baseline + metric đo được chưa? | Yes — provisional | Nhóm đã cung cấp interview 3 học viên, survey 8 học viên và baseline seed 4,1 lượt kiểm tra/ngày, 3–4 nguồn/lượt, 5–8 phút/lượt. Cần ghi log lặp lại trong pilot để kiểm định target trước/sau. |
| Data/input đủ dùng chưa? | Yes — for manual pilot | Đủ để chạy thủ công với link nguồn, owner, timestamp, ngày hiệu lực, deadline và trạng thái; chưa đủ để tự động đọc mọi kênh hoặc tích hợp Agent. |
| AI sai, hậu quả chấp nhận được không? | Not Yet — AI out of pilot | AI chưa nằm trong phần bắt buộc của pilot; nếu bổ sung, mọi tóm tắt phải có link nguồn và học viên/owner review trước khi hành động. |
| Có người review/owner không? | Yes — internal roles assigned; external confirmation pending | Nhóm đã phân công người phụ trách nội bộ theo từng hạng mục; owner chính thức vẫn phải xác nhận tên/kênh liên hệ trước khi chạy pilot. |
| Có cách non-AI đơn giản hơn không? | Yes | Source-of-truth + format thông báo + timeline thủ công là phương án đơn giản cần thử trước AI. |

**Decision:**

```text
[Go]
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text
Candidate có actor, workflow và bottleneck rõ; đồng thuận nhóm cũng xác định source-of-truth, owner, timestamp, dedup và human review là các điều kiện bắt buộc. Interview 3 học viên, survey 8 học viên và baseline seed do nhóm cung cấp cùng chỉ về việc phải mở nhiều nguồn, hỏi lại hoặc phát hiện muộn cập nhật. Vì vậy nhóm **Go có giới hạn** vào pilot Rule/Workflow thủ công trong một tuần, chưa Go vào Agent hoặc tự động gửi deadline. Trước khi kết luận cuối cùng, nhóm sẽ lưu log lặp lại và kiểm định các target trước/sau.
```

**Nếu Go — pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**

```text
Chạy tay trong một tuần trên các thông báo lab/task/deadline của nhóm. Tạo một bảng chính có trường nguồn, owner, timestamp, ngày hiệu lực, deadline, trạng thái và link; áp dụng đúng quy tắc ưu tiên ở đầu báo cáo, rồi so sánh với cách mỗi thành viên tự kiểm tra. Đo 3 số: thời gian đến khi xác định được cập nhật, số nguồn/vòng mở và số thông tin bị trùng hoặc cần sửa; chỉ thêm AI tóm tắt sau khi Rule + timeline hoạt động ổn định.
```

**Nếu Not Yet — cần validate gì trước:**

```text
Nếu mở rộng từ pilot thủ công sang AI, cần lặp lại validation trên log thật, chốt tên/kênh liên hệ của từng owner, kiểm tra quyền truy cập và audit các trường hợp mâu thuẫn. Chỉ bật AI khi timeline có đủ link nguồn, timestamp và quy tắc xử lý `PENDING_CONFIRMATION`; nếu chưa đạt thì giữ Workflow thủ công.
```

**Nếu No-Go — làm gì thay AI:**

```text
Dùng một bảng/timeline source-of-truth, quy ước kênh chính, format thông báo và người owner; không triển khai Agent. Nếu Workflow không giảm thời gian hoặc làm tăng deadline sai/thông báo trùng, giữ cách kiểm tra thủ công và chỉ sửa cấu trúc nguồn, quyền truy cập hoặc UX.
```

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**

```text
Dừng AI khi tóm tắt thiếu link nguồn, chọn nhầm bản chính, tạo deadline sai, bỏ sót cập nhật quan trọng hoặc tỷ lệ cảnh báo trùng tăng. Khi dừng, ẩn lớp AI, giữ bảng/timeline và chuyển về đối chiếu thủ công giữa các nguồn; owner sửa bản chính trước khi phát hành lại.
```

### Chỉ mục bằng chứng và trạng thái sẵn sàng nộp

| Nội dung | Vị trí bằng chứng hiện có | Trạng thái | Việc còn cần làm |
|---|---|---|---|
| Convergence và quyết định candidate | Phần Phase 3 của báo cáo này | Có bản ghi | Đối chiếu lại số thành viên và số candidate theo quy tắc mỗi người Top 3. |
| Quy mô nhóm và độ đầy đủ candidate | Bảng thành viên và bảng trình bày Top 3 ở Phase 3 | Cần xác nhận | Báo cáo đang ghi 5 thành viên nhưng worksheet nêu nhóm 3–4 người; nếu giữ 5 người thì cần bổ sung/giải thích 3 candidate còn thiếu. |
| Interview, survey và baseline seed | `02-group-problem-statement-validation-notes.md` | Có bản tổng hợp, chưa có log gốc | Lưu artifact đã ẩn thông tin nhạy cảm nếu cần kiểm tra độc lập. |
| Research links | Bảng Research của báo cáo này và validation notes | Đã có 3 nguồn | Tiếp tục giữ link, ngày kiểm tra và claim tương ứng. |
| Workflow, metric, PS v0/v1 | Phần Phase 5–6 của báo cáo này | Đã có | Chốt cohort, khoảng thời gian và data dictionary trước pilot. |
| Owner chính thức | Bảng phân công pilot | Chưa xác nhận | Bổ sung tên/kênh owner tương ứng trước khi chạy pilot. |
| Bản copy của các thành viên khác | Ngoài phạm vi repo hiện tại | Chưa kiểm tra được | Từng thành viên xác nhận repo của mình đã có report và validation notes. |

### Cổng quyết định sau pilot

Sau một tuần pilot thủ công, nhóm chỉ chuyển sang bước có AI hỗ trợ nếu cùng một cohort và khoảng thời gian cho thấy: thời gian xác định cập nhật giảm ít nhất 30%, số lần hỏi lại không quá 25% cohort (tương đương tối đa 2/8 nếu vẫn dùng mẫu 8 người), số lần phát hiện muộn không quá 12,5% cohort (tương đương tối đa 1/8), không có deadline sai hoặc mất link nguồn, và thông báo trùng không tăng. Nếu thiếu timestamp, owner chưa được xác nhận hoặc không đạt một guardrail an toàn, quyết định là `Not Yet` và giữ Workflow thủ công. Nếu phát sinh deadline sai, tự gửi cảnh báo diện rộng hoặc mất khả năng truy nguyên nguồn, tắt lớp AI và rollback về timeline/source-of-truth thủ công.

---

### Việc còn mở trước khi nộp

- [x] Chốt tên nhóm, thành viên, mã học viên và vai trò nội bộ.
- [x] Chốt candidate số 1, convergence, shortlist, score và disagreement.
- [x] Bổ sung source-of-truth, validation quote/survey/baseline và research links.
- [x] Bổ sung file [validation notes](../02-group-problem-statement-validation-notes.md).
- [x] Bổ sung so sánh đầy đủ No AI / Rule / Workflow / Agent và quyết định `[Go]` có giới hạn.
- [ ] Xác nhận tên/kênh liên hệ của BTC, facilitator và task owner chính thức; hiện vẫn giữ `PENDING_CONFIRMATION` vì nhóm chưa cung cấp thông tin này.
- [ ] Xác nhận quy mô nhóm theo quy định 3–4 người và xử lý chênh lệch 12/15 candidate nếu danh sách 5 người được giữ.
- [ ] Nếu muốn dùng số liệu làm evidence cuối cùng, lưu ảnh/log gốc đã ẩn thông tin nhạy cảm và chạy lại phép đo trong cùng khoảng thời gian.
- [ ] Kiểm tra các thành viên còn lại đã copy đúng bản group report và file validation notes vào repo cá nhân của họ.

### Self-check nộp phần 02 (nhóm)
- [x] Có nhật ký hội tụ 9-12 → 1 (cluster + shortlist + score) — bản nháp từ bảng candidate được cung cấp
- [x] Có validation (quote thật) + research (link kiểm được) — validation và baseline do nhóm cung cấp, cần lưu log lặp lại nếu pilot tiếp tục
- [x] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [x] Có PS v0 → v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [x] Có so sánh No AI/Rule/Workflow/Agent + Decision Go có giới hạn, chưa chọn Agent
