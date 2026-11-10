# Báo cáo cá nhân — 2A202603925_NguyenHuyTan

## 1. Thông tin học viên

- Họ tên: **Nguyễn Huy Tấn**
- MSSV: **2A202603925**
- Lớp: **K5 - Level 3 (L3B)**
- Tên nhóm: **Nhom5W**
- Link repo nhóm: `https://github.com/ngthanhtamtb/K5-L3B-DAY02-Nhom5W-DiscoveryProblemFraming`
- Vai trò trong nhóm: Phụ trách xây dựng Assumption Map, tổng hợp tín hiệu xác nhận & phản bác từ phỏng vấn The Mom Test ở CP4, hỗ trợ rà soát quy trình Before/After ở CP5, và phụ trách chính bảng đánh giá 4 rủi ro + ngưỡng dừng ở CP6.

**Chủ đề cá nhân:** Thông báo, deadline và lịch học của khóa học nằm rải rác ở nhiều kênh.

**Bối cảnh cá nhân:** Tấn là học viên khóa AI20K Cohort V của VinUni. Sau mỗi buổi học, Tấn phải kiểm tra 4 nguồn khác nhau để tìm thông báo, deadline và thay đổi lịch học: Outlook (email của ban tổ chức và coach), Discord (kênh thông báo và kênh lớp), trang Thời khóa biểu AI20K – Cohort V, và portal-cohort5.edufun.ai (bài lab và hạn nộp).

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi kết thúc buổi học, tôi muốn biết có thông báo, deadline hay thay đổi lịch nào mới trên các kênh, để sắp xếp việc cho ngày mai. | Tấn; có thể gồm học viên khác nếu họ cũng theo dõi các kênh này. | Có **4 nguồn** cần kiểm tra mỗi tối. Ước lượng mỗi lần rà đủ 4 nguồn và ghi lịch mất khoảng **~20 phút** (Outlook ~4', Discord ~8', Thời khóa biểu ~3', portal ~3', ghi lịch ~2') `(ước lượng; sẽ bấm giờ thật trong 5 ngày học tới)`. |
| 2 | Pain từ người khác | Khi lịch học hoặc deadline thay đổi, tôi muốn biết thay đổi nào là bản mới nhất, để không học hoặc nộp theo thông tin cũ. | Học viên chịu ảnh hưởng bởi thay đổi lịch hoặc hạn nộp. | Ước lượng trên Discord lớp trong một tuần gần đây: thấy khoảng **5–7 tin** hỏi lặp lại kiểu *"mấy giờ học / hạn nộp bài khi nào?"* do tin thông báo bị trôi `(ước lượng)`. |
| 3 | Tốn thời gian | Khi chuẩn bị nộp bài lab, tôi muốn đối chiếu bài làm với rubric, để không thiếu mục bắt buộc. | Học viên nộp bài lab. | Khi tự kiểm tra bài lab Day 01 trước đó theo cấu trúc rubric, mất khoảng **~20 phút** `(ước lượng)` đối chiếu từng mục để tránh nộp thiếu. |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi email của khóa học chứa nhiều việc cần làm, tôi muốn tách được từng việc và hạn tương ứng, để không bỏ sót mục nằm cuối email. | Người nhận email thông báo. | Xem qua các email thông báo gần nhất của khóa `(~4–5 email, ước lượng)`: thường có từ 8–12 đầu việc nhỏ và nhiều mốc hạn rải rác ở các đoạn khác nhau. |
| 5 | Lặp lại | Khi làm bài nhóm, tôi muốn biết ai phụ trách phần nào, để không làm trùng. | Nhóm **3 người** (Nhom5W). | Ở bài lab trước có tình trạng **2 người cùng viết một mục** do chưa chốt checklist phân công ngay từ đầu. |
| 6 | Tốn thời gian | Khi gặp lại một lỗi đã được coach giải đáp trên Discord, tôi muốn tìm được câu trả lời cũ, để không hỏi lại. | Học viên và coach. | Thử tìm lại các lỗi kỹ thuật cũ trên Discord mất khoảng **~10 phút/lần** `(ước lượng)` do tin nhắn thảo luận nhiều, khó nhớ chính xác từ khóa ban đầu. |

**AI đã hỗ trợ ở bước rà soát:**
- Sau khi tự scan 6 vấn đề từ việc học hằng ngày, tôi có dùng AI rà lại bảng. AI đề xuất tách vấn đề *"thông tin rải rác"* khỏi giả định *"cần xây bot AI"*, và nhắc phải đo thời gian, đếm số lần bỏ sót trước khi khẳng định mức độ nghiêm trọng. Tôi giữ 2 gợi ý này vì giúp bài scan bám sát dữ kiện hơn.
- Tôi không đưa ý tưởng *"trợ lý AI tự đọc toàn bộ kênh"* vào bảng problem vì đó là giải pháp, còn quyền truy cập API và quy định về kênh chính thức chưa được kiểm chứng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| **1** | **Thông báo, deadline rải rác bốn kênh (#1)** | Quy trình lặp lại hằng ngày và gồm 4 nguồn có thể quan sát trực tiếp. | Các học viên khác có kiểm tra đủ 4 nguồn giống mình không? Số lần biết tin muộn thực tế là bao nhiêu? |
| 2 | Đối chiếu rubric trước khi nộp bài lab (#3) | Đầu vào rõ ràng (file rubric và bài làm); đo được số mục bỏ sót trước khi nộp. | Một bảng checklist tick tay có thể đã giải quyết đủ tốt. |
| 3 | Tìm lại câu trả lời cũ trên Discord (#6) | Có thể kiểm thử ngay trên một số câu hỏi kỹ thuật đã từng có lời giải. | Thanh tìm kiếm sẵn có của Discord kết hợp tin ghim có thể đã đủ nhanh. |

---

### Problem Card #1 — Thông báo, deadline rải rác bốn kênh

| Trường | Nội dung |
|---|---|
| **Job Story** | **Khi** kết thúc buổi học, **tôi muốn** biết có thông báo, deadline hay thay đổi lịch nào mới trên các kênh, **để** sắp xếp việc cho ngày mai mà không bị lỡ lịch. |
| **Actor** | Trước mắt là Tấn, học viên AI20K Cohort V. Chỉ mở rộng sang học viên khác sau khi phỏng vấn xác nhận họ có cùng quy trình. |
| **Thời điểm / bối cảnh** | Cuối mỗi buổi học; hoặc ngay sau khi có thông báo đổi lịch hay dời deadline. |
| **Quy trình hiện tại (3–7 bước)** | 1. Mở Outlook xem email mới (~4' ước lượng)<br>2. Kiểm tra kênh thông báo và kênh lớp trên Discord (~8' ước lượng)<br>3. Xem trang Thời khóa biểu (~3' ước lượng)<br>4. Xem portal kiểm tra bài và hạn nộp (~3' ước lượng)<br>5. Ghi các việc cần làm vào lịch cá nhân (~2' ước lượng) |
| **Bottleneck (bước nào, mất bao nhiêu phút)** | **Bước 2 — Kiểm tra Discord (~8' ước lượng)**: bước mất nhiều thời gian nhất do tin nhắn thông báo dễ bị trôi giữa nhiều tin nhắn thảo luận. |
| **Impact (nếu không giải thì sao)** | Mất khoảng 20 phút mỗi tối `(ước lượng)` để đảo qua lại 4 nguồn; có nguy cơ xem thiếu một cập nhật hoặc dùng thông tin cũ. |
| **Success metric (baseline → target)** | **Baseline:** ~20 phút/lần kiểm tra đủ 4 nguồn `(ước lượng; kế hoạch bấm giờ thực tế trong 5 ngày học tới để chốt baseline)`.<br>**Target:** giảm ít nhất 50% thời gian kiểm tra; không bỏ sót thay đổi đã đăng ở nguồn chính thức trong 2 tuần thử nghiệm. |
| **Phương án không dùng AI** | Ban tổ chức xác định 1 nơi duy nhất là nguồn lịch/deadline chính thức; mọi thay đổi cập nhật tại đó, các kênh khác chỉ gửi đường dẫn điều hướng. Học viên bật thông báo riêng cho kênh chính thức. |
| **Giả thuyết về AI (nếu có)** | Nếu bắt buộc vẫn duy trì 4 kênh song song, AI có thể đọc tóm tắt các việc cần làm và hạn nộp từ nguồn được cấp quyền. Cần kiểm tra độ chính xác và quyền truy cập trước. |
| **Cảm nhận nhanh** | **Workflow / Rule** là hướng thử đầu tiên; chưa đủ bằng chứng để chọn Agent. |

#### Quy trình nháp hiện tại (Problem Card #1) — Tổng thời gian: ~20 phút (ước lượng)

```text
Outlook (~4') → Discord (~8') ⚠️ BOTTLENECK → Thời khóa biểu (~3') → Portal (~3') → Ghi lịch cá nhân (~2')
```

---

### Problem Card #2 — Đối chiếu rubric trước khi nộp bài lab

| Trường | Nội dung |
|---|---|
| **Job Story** | **Khi** chuẩn bị nộp bài lab trên portal, **tôi muốn** biết bài còn thiếu mục nào theo rubric, **để** không bị trừ điểm vì thiếu cấu trúc. |
| **Actor** | Học viên AI20K Cohort V, nộp bài lab sau mỗi buổi học. |
| **Thời điểm / bối cảnh** | Trước mỗi lần nộp bài lab, thường là buổi tối sát hạn nộp. |
| **Quy trình hiện tại (3–7 bước)** | 1. Mở `RUBRIC.md` và `CHECKPOINTS.md` (~2' ước lượng)<br>2. Đọc từng tiêu chí, đối chiếu với từng mục trong bài (~13' ước lượng)<br>3. Ghi lại mục thiếu và rà soát bổ sung (~4' ước lượng)<br>4. Nộp link trên LMS (~1' ước lượng) |
| **Bottleneck (bước nào, mất bao nhiêu phút)** | **Bước 2 — Đọc từng tiêu chí rồi tìm minh chứng tương ứng trong bài**, khoảng ~13'/bài `(ước lượng)`. |
| **Impact (nếu không giải thì sao)** | Mất khoảng ~20'/bài `(ước lượng)`; nếu sót một mục bắt buộc thì bị trừ điểm cấu trúc dù nội dung đã làm. |
| **Success metric (baseline → target)** | Thời gian tự kiểm: từ ~20' `(ước lượng)` $\to$ dưới 5'/bài (tự bấm giờ trong các bài lab tới). Số mục bị trừ vì thiếu: đếm ở bài đã chấm $\to$ 0. |
| **Phương án không dùng AI** | Gom các dòng tự kiểm tra trong `CHECKPOINTS.md` và `SUBMISSION.md` thành 1 checklist tick sẵn, mở cạnh bài khi làm. |
| **Giả thuyết về AI (nếu có)** | AI đọc bài làm và file rubric để liệt kê mục còn thiếu kèm trích dẫn; nhưng checklist có sẵn có thể đã đủ. |
| **Cảm nhận nhanh** | **No AI / Rule** trước; chỉ xét AI nếu checklist vẫn làm mất thời gian hoặc bỏ sót. |

#### Quy trình nháp hiện tại (Problem Card #2)

```text
1. Mở RUBRIC + CHECKPOINTS (~2') → 2. Đối chiếu tiêu chí với bài (~13') ⚠️ BOTTLENECK → 3. Ghi & bổ sung mục thiếu (~4') → 4. Nộp LMS (~1')
```

---

### Problem Card #3 — Tìm lại câu trả lời cũ trên Discord

| Trường | Nội dung |
|---|---|
| **Job Story** | **Khi** gặp lại một lỗi đã được coach giải đáp trên Discord, **tôi muốn** tìm lại được tin nhắn cũ, **để** không phải hỏi lại. |
| **Actor** | Học viên AI20K Cohort V (~100 người); coach là người phải trả lời lặp lại. |
| **Thời điểm / bối cảnh** | Khi làm lab gặp lỗi mà nhớ đã từng thấy ai hỏi trước đó, khoảng ~3 lần/tuần `(ước lượng)`. |
| **Quy trình hiện tại (3–7 bước)** | 1. Nhớ lại câu trả lời ở kênh nào (~2' ước lượng)<br>2. Gõ từ khóa tìm trên Discord, thử vài từ khóa khác nhau (~6' ước lượng)<br>3. Mở từng kết quả, đọc ngữ cảnh trong thread (~2' ước lượng)<br>4. Không thấy thì hỏi lại trên kênh và chờ coach trả lời |
| **Bottleneck (bước nào, mất bao nhiêu phút)** | **Bước 2 — Thử nhiều từ khóa tìm kiếm trên Discord**, khoảng ~6'/lần `(ước lượng)` do không nhớ đúng từ người hỏi trước đã dùng. |
| **Impact (nếu không giải thì sao)** | Mất ~10'/lần × ~3 lần/tuần ≈ 30'/tuần `(ước lượng)`; coach phải trả lời lại các câu hỏi trùng lặp. |
| **Success metric (baseline → target)** | Thời gian tìm: từ ~10' `(ước lượng)` $\to$ dưới 3'/lần (tự bấm giờ trong 1 tuần). Số câu hỏi trùng trên kênh: đếm 1 tuần làm baseline $\to$ giảm một nửa. |
| **Phương án không dùng AI** | Coach hoặc lớp trưởng ghim một tin "Câu hỏi thường gặp (FAQ)" theo từng lab, cập nhật cuối mỗi buổi. |
| **Giả thuyết về AI (nếu có)** | Tìm kiếm theo ngữ nghĩa câu hỏi kèm dẫn link tin nhắn gốc thay vì tìm khớp chính xác từng từ khóa. |
| **Cảm nhận nhanh** | **No AI / Rule** trước; tìm kiếm có dẫn nguồn chỉ là ứng viên nếu FAQ ghim không đạt. |

#### Quy trình nháp hiện tại (Problem Card #3)

```text
1. Nhớ kênh (~2') → 2. Thử từ khóa tìm kiếm (~6') ⚠️ BOTTLENECK → 3. Đọc thread (~2') → 4. Không thấy thì hỏi lại, chờ coach
```

---

### Card muốn pitch nhất

- **Card số:** **1**.
- **Vì sao chọn:** Đây là quy trình có 4 nguồn và lặp lại sau buổi học, có thể kiểm chứng bằng nhật ký thao tác; chưa khẳng định toàn bộ học viên có cùng pain.
- **Câu hỏi muốn nhóm phản biện:** *"Nếu trang Thời khóa biểu và portal được xác định là nguồn chính thức cho mọi thay đổi, còn Discord chỉ dẫn link, vấn đề này có còn đủ lớn để cần giải pháp mới không?"*

---

### AI đã phản biện card thế nào

Đã dùng prompt *"product manager hoài nghi"* trong `docs/01-worksheet.md` để xem lại actor, quy trình, bottleneck, metric và phương án không dùng AI:

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|:---:|---|
| Gán pain cho mọi học viên khi mới mô tả trải nghiệm của một người. | **Có** | Thu hẹp actor ban đầu thành Tấn; chỉ mở rộng sau khi phỏng vấn học viên khác. |
| Thời gian từng bước và số lần biết tin muộn trong bản nháp là ước lượng, chưa có nhật ký. | **Có** | Giữ rõ nhãn `(ước lượng)` trên toàn bộ số phút; lên kế hoạch bấm giờ thật để có baseline chuẩn. |
| Discord được gọi là bottleneck nhưng chưa chứng minh chậm nhất. | **Có** | Tách thời gian từng nguồn ra riêng, chỉ ra Discord chậm nhất do tin bị trôi, cần bấm giờ để kiểm chứng thêm. |
| Mục tiêu "không bỏ sót" cần có định nghĩa và nguồn kiểm chứng. | **Có** | Chỉ tính các thay đổi đã đăng ở nguồn chính thức và kiểm tra trong 2 tuần thử nghiệm. |
| Có thể xử lý bằng nguồn thông tin chính thức và quy tắc thông báo, chưa cần AI. | **Có** | Đưa Workflow/Rule thành lựa chọn thử trước; AI chỉ là giả thuyết nếu cách đơn giản không đủ. |
| Gợi ý AI tự động quét mọi tin nhắn Discord và email để gom thành bản tin. | **Không** | Bác bỏ vì nhảy sang giải pháp quá sớm (solution-first) và chưa có quyền truy cập API từ ban tổ chức. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| **Pitch Problem Card** | Pitch 3 card về việc học ở khóa AI20K, trọng tâm là card #1 của tôi (#7 trong bảng nhóm): thông báo, deadline rải rác ở 4 kênh | Card vào shortlist (27 điểm) nhưng bị loại: một nguồn thông báo chính thức (Rule/No AI) giải được phần lớn, người quyết định là ban tổ chức, và số liệu mới là ước lượng |
| **Phản biện bài của bạn khác** | Câu hỏi tôi đã đặt: (1) Hỏi Đạt, card #2: *"Việc này chỉ 1–2 lần/học kỳ, có đủ lặp lại để đáng làm không?"* (2) Hỏi Đạt, card #3: *"Đo thế nào thì một ví dụ được coi là đủ hay?"* (3) Hỏi Tâm, card #5: *"Nghẽn là do chờ người khác gửi hồ sơ; có nhắc nhở thì họ có gửi nhanh hơn không, hay checklist + thư mục chung là đủ?"* | Card #2 và #3 của Đạt không vào shortlist vì tần suất thấp và metric khó đo. Tâm đồng ý card #5 chưa đủ dữ liệu |
| **Nhận phản biện** | Câu hỏi tôi nhận được: (1) Đạt hỏi card #7: *"Nếu ban tổ chức chỉ cập nhật thay đổi ở một kênh chính thức thì problem này còn không?"* (2) Tâm hỏi card #8: *"RUBRIC.md đã như một checklist, tự tick theo đó có đủ không?"* (3) Tâm hỏi card #9 về việc Discord đã có ô tìm kiếm | Tôi đã sửa gì: card #1 để Workflow/Rule là hướng thử đầu tiên, phương án không dùng AI là một nguồn chính thức. Card #2 ghi No AI/Rule (checklist) trước. Card #3 ghi dùng tìm kiếm sẵn + FAQ ghim trước |
| **Gom cluster / cây OST** | Cùng nhóm gom 9 card thành 4 cluster; card #7 và #9 của tôi vào cụm B "Gom thông tin rải rác" | Cây OST có nhánh "thông báo đổi lịch bị trôi giữa nhiều tin chat"; ý "app gom thông báo 4 kênh" bị gạch vì là solution |
| **Chọn candidate problem** | Cùng chấm 7 tiêu chí cho 3 card shortlist | Nhóm chọn card #1 của Đạt về GV-A (34 điểm) |
| **Kiểm chứng / research** | Đẩy 3 biên bản phỏng vấn vào `report/assets/cp4-interview-snapshot-1..3.md`; phụ trách Assumption Map: chọn 3 giả định kiểm trước (#1, #2 Value và #5 Viability); tổng hợp tín hiệu xác nhận và phản bác | Nhờ tín hiệu phản bác, nhóm giữ việc cắt OCR và thêm yêu cầu giáo viên duyệt trước khi gửi (group report mục 3.1, 3.2) |
| **Quy trình nhóm** | Hỗ trợ Đạt rà quy trình Before/After | Quy trình After có bước người duyệt và phương án quay về |
| **Problem Statement** | Góp ý cho v0 | v1 có thêm metric chất lượng |
| **Mức can thiệp AI** | Tham gia thảo luận vì sao chọn Workflow | AI chỉ can thiệp ở bước 4 |
| **Quyết định** | Phụ trách chính bảng 4 rủi ro và ngưỡng dừng | Cả 4 rủi ro ở mức Trung bình kèm lý do; quyết định Go phạm vi nhỏ, 3 ngưỡng dừng đo được (group report mục 8) |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| **CP1 Scan** | Rà lại bảng scan sau khi tự viết 6 dòng | Tách "thông tin rải rác" khỏi giả định "cần bot AI"; nhắc phải đo trước khi khẳng định mức nghiêm trọng | Gợi ý "trợ lý AI tự đọc toàn bộ kênh", là giải pháp chứ không phải problem | Không đưa ý đó vào bảng; đánh dấu `(ước lượng)` và ghi rõ kế hoạch bấm giờ cho từng dòng |
| **CP2 Problem Card** | Cho AI đóng vai PM hoài nghi phản biện card #1 | Chỉ ra actor quá rộng, số phút là ước lượng, Discord chưa chứng minh là bước chậm nhất, Rule có thể đã đủ | Đề xuất viết bot tự động thu thập tin nhắn qua API mà bỏ qua vấn đề phân quyền và bảo mật của BTC | Thu hẹp actor, giữ nhãn ước lượng, bác bỏ ý tưởng bot và để Workflow/Rule là hướng thử đầu |
| **CP4 Assumption Map** | Hỏi gợi ý cách phân loại rủi ro theo khung 4 rủi ro của Marty Cagan | Gợi ý cách sắp xếp các giả định vào 2 trục Quan trọng / Đã có bằng chứng khá trực quan | Đánh giá rủi ro Viability (trường cho phép dùng AI) là thấp vì nghĩ việc dùng AI soạn nháp rất bình thường | Chỉnh lại mức Quan trọng = 5, Bằng chứng = 1 (cần kiểm trước) vì phản hồi của trường với phụ huynh chịu ràng buộc rất chặt |
| **CP5 Quy trình** | Hỗ trợ rà lại luồng 6 bước Before/After | Nhắc cân đối thời gian tổng thể và kiểm tra tính liên tục giữa đầu vào/đầu ra từng bước | Gợi ý gộp luôn khâu soạn nháp và khâu gửi để rút ngắn thời gian quy trình xuống tối đa | Bác bỏ ngay, tách riêng Bước 5 là con người duyệt 100% (HITL) theo đúng yêu cầu của Thầy Tổ trưởng trong phỏng vấn |
| **CP5–6 Problem Statement** | Dùng prompt *"Chỉ ra lỗ hổng, đừng viết lại thay tôi"* để soát bản nháp | Chỉ ra bản v0 thiếu tiêu chí đánh giá chất lượng nhận xét bên cạnh thời gian | Gợi ý dùng các từ ngữ kỹ thuật nặng tính hệ thống trong Problem Statement | Giữ văn phong nghiệp vụ giảng dạy dễ hiểu cho GV-A, bổ sung 2 metric chất lượng rõ ràng ở v1 |
| **CP6 Mức can thiệp / quyết định** | Rà soát bảng 4 rủi ro và 3 ngưỡng dừng | Gợi ý các con số định lượng cho ngưỡng dừng (ví dụ tỉ lệ phải viết lại) | Cho rằng công nghệ tạo văn bản đã ổn định nên rủi ro sai sót dữ liệu thấp, có thể áp dụng rộng | Hạ quyết định về pilot quy mô nhỏ nhất (1 lớp 35 em trong 4 tuần) và đặt ngưỡng dừng ngay nếu sai 01 dữ liệu |

---

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi nghe Đạt trình bày chuyện của GV-A và Tâm trình bày chuyện nhật ký thi công ở công trường, tôi thấy cả ba bài toán (việc học của tôi, giảng dạy của GV-A, làm hồ sơ của Tâm) tuy khác ngành nhưng đều chung một kiểu nghẽn: con người phải tự đọc, gom và chép lại thông tin từ nhiều nguồn rời rạc. Điều tôi học được rõ nhất là không phải việc nào mất thời gian cũng cần mang AI vào giải. Bài toán 4 kênh thông báo của tôi nghe thì bực thật, nhưng nguyên nhân gốc là do cách truyền thông chưa gom về một mối; chỉ cần ban tổ chức quy định 1 kênh chính thức (No AI / Rule) là giải quyết được phần lớn. Còn bài của Đạt về GV-A mới thực sự cần AI, vì khâu khó không nằm ở gom số liệu mà nằm ở việc viết lời nhận xét riêng cho từng học sinh theo tiến độ 2 tuần trước đó.

**6.2. Nhóm có lúc nào bị "solution-first" không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có, nhóm tôi bị nhảy vào giải pháp ngay từ đầu ở cả bài của tôi lẫn bài của Đạt. Về phía tôi, lúc mới nêu vấn đề thông báo rải rác 4 kênh, trong đầu tôi đã nghĩ ngay tới việc làm một cái "app gom thông báo 4 kênh". Nhưng khi cả nhóm ngồi vẽ cây OST, ý tưởng này bị gạch ngay lập tức vì nó là giải pháp chứ không phải nỗi đau; nhánh vấn đề thật được giữ lại trên cây là "thông báo đổi lịch bị trôi giữa nhiều tin chat". Còn về bài toán của GV-A, ở bản nháp card #1 đầu tiên, Đạt cũng tính cho AI dùng OCR đọc bài giấy để tự chấm điểm. Nhờ ở CP2 dùng AI đóng vai PM hoài nghi phản biện, rồi sang CP4 phỏng vấn GV-A xác nhận chấm bài bằng barem đã nhanh rồi, nhóm mới cắt hẳn phần OCR để tập trung đúng vào khâu gõ nhận xét. Bài học lớn của cả nhóm là phải bóc tách đúng chỗ nghẽn thật rồi mới tính đến công nghệ.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có, và lần đổi ý rõ nhất là ngay lúc pitch card ở CP3. Lúc đầu tôi khá bảo vệ card #7 của mình (thông báo rải rác 4 kênh) vì đó là chuyện tôi gặp hằng ngày khi học khóa AI20K. Tuy nhiên, Đạt đặt cho tôi một câu hỏi rất thẳng: *"Nếu ban tổ chức chỉ cập nhật thay đổi ở một kênh chính thức thì problem này còn không?"*. Nghe xong câu đó tôi khựng lại và nhận ra đúng thật: nếu ban tổ chức chốt một kênh chính thức còn các kênh khác chỉ dẫn link, vấn đề sẽ biến mất hoàn toàn mà chẳng cần viết thêm phần mềm hay AI nào cả. Tôi nhận ra bài của mình phụ thuộc vào quy định của ban tổ chức chứ không phải bài toán phù hợp để so sánh 4 mức can thiệp AI, nên tôi đồng ý hạ card xuống mức Rule / No AI và quay sang ủng hộ card #1 của Đạt.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Vì tôi trực tiếp phụ trách tổng hợp tín hiệu xác nhận và phản bác ở CP4, kết quả phỏng vấn The Mom Test khiến tôi bất ngờ ở hai chỗ lớn. Bất ngờ đầu tiên là ở phỏng vấn GV-A (biên bản 1): tôi cứ nghĩ chấm bài là khâu mệt nhất của giáo viên, nhưng cô nói rõ: *"Chấm bài thì tôi chấm theo barem, khoảng 45 phút là xong 2 lớp (hơn 70 bài). Nhưng cực hình nhất là sau đó: nhà trường yêu cầu mỗi bài kiểm tra định kỳ 2 tuần phải có báo cáo tiến trình cá nhân hóa gửi phụ huynh trên app của trường... Cứ 2 đến 3 phút một em, 70 em là mất đứt gần 3 tiếng đồng hồ buổi tối Chủ nhật!"*. Nhờ đó nhóm mới chắc chắn 100% quyết định bỏ OCR là hoàn toàn đúng. Bất ngờ thứ hai là khi tôi trực tiếp phỏng vấn Thầy T. — Tổ trưởng chuyên môn (biên bản 2). Thầy ủng hộ công cụ soạn nháp, nhưng đặt ranh giới cứng: *"Tuyệt đối không được để phần mềm tự động bắn tin nhắn cho phụ huynh. Nhận xét gửi đi đại diện cho uy tín sư phạm của nhà trường. Giáo viên phải là người đọc duyệt, chỉnh sửa từng câu chữ trước khi bấm nút gửi."* Yêu cầu này chốt luôn việc nhóm không thể chọn mức Agent tự động mà phải chọn Workflow có con người duyệt cuối.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất với tôi là đặt Success Metric cho những phần chưa từng có số đo trước đó, đặc biệt là phía phụ huynh học sinh. Ở bản v0, nhóm chỉ đặt mục tiêu thời gian từ 315 phút xuống dưới 120 phút cho GV-A. Nhưng làm nhanh hơn mà câu chữ AI viết ra cứng nhắc, giáo viên phải xóa đi viết lại hết, hoặc phụ huynh đọc xong vẫn không biết con yếu phần nào thì coi như thất bại. Cuối cùng nhóm phải tách thêm 2 chỉ số chất lượng ở bản v1: tỉ lệ bản nháp phải viết lại dưới 15% và khảo sát phụ huynh lớp pilot bằng một câu hỏi Có/Không trước và sau khi thử nghiệm (mục tiêu trên 80% chọn Có). Ngoài ra, viết phần Boundary sao cho chặt — nhất là quy định AI chỉ nhận mã học sinh và mã câu sai, không nhận họ tên thật — cũng khiến nhóm phải rà đi rà lại nhiều lần để tránh rủi ro lộ thông tin học sinh.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại từ đầu, việc đầu tiên tôi sửa ở phần cá nhân là phải tự bấm giờ thật quá trình kiểm tra 4 kênh trong vài ngày liên tiếp thay vì để số liệu dạng ước lượng rồi mới điền vào card. Không có số bấm giờ thật thì lúc pitch rất khó chứng minh độ lớn của vấn đề. Về phía bài nhóm, tôi nghĩ mình cần phản biện mạnh hơn nữa vào con số baseline 315 phút của GV-A. Con số này hiện nay mới chỉ là lời kể ước chừng của cô giáo trong buổi phỏng vấn (gần 1 tiếng soạn đề, gần 3 tiếng gõ nhận xét) chứ nhóm chưa có số bấm giờ thực tế. Nếu làm lại, tôi sẽ đề nghị nhóm yêu cầu GV-A bấm giờ kỹ 1 chu kỳ làm thật theo cách cũ ngay trước khi chạy pilot, để khi đánh giá kết quả giảm xuống dưới 120 phút sẽ có cơ sở so sánh chắc chắn nhất.

**6.7. Hiểu bài:**

1. **Problem:** GV-A (giáo viên Toán/KHTN THPT dạy 2 lớp, 70 học sinh) mất khoảng 315 phút (theo lời kể) cho mỗi đợt kiểm tra định kỳ 2 tuần, trong đó khâu nặng nhất là tự nhớ lại lỗi cũ và gõ nhận xét cá nhân hóa cho từng em (170 phút), khiến giáo viên quá tải phải dùng câu mẫu rập khuôn và phụ huynh không biết con đang hổng kỹ năng nào.
2. **Quy trình:** Chuyển sang luồng 6 bước (kỳ vọng 115 phút): Bước 1 Rule tự trộn câu hỏi từ ngân hàng đề gắn mã kỹ năng để xuất 3 mã đề $\to$ Bước 2 giáo viên tự chấm bài và nhập điểm kèm mã câu sai $\to$ Bước 3 Rule tự đối chiếu mã câu sai sang chuẩn kỹ năng và kéo lịch sử bài trước $\to$ Bước 4 AI soạn nháp nhận xét 3 phần $\to$ Bước 5 giáo viên đọc rà soát, chỉnh sửa $\to$ Bước 6 giáo viên tự bấm nút gửi cho phụ huynh.
3. **Metric:** Tổng thời gian từ baseline 315 phút (cần bấm giờ 1 chu kỳ trước pilot) giảm xuống dưới 120 phút; dưới 15% bản nháp AI phải xóa viết lại từ đầu; và trên 80% phụ huynh lớp pilot trả lời "Có" khi được khảo sát xem nhận xét có chỉ rõ phần con cần ôn luyện hay không.
4. **Boundary:** AI tuyệt đối không tự gửi tin nhắn cho phụ huynh, không tự sửa điểm số, không dùng từ ngữ phán xét tiêu cực về học sinh, và chỉ nhận mã học sinh, điểm số, mã câu sai chứ không nhận họ tên thật (tên học sinh do Rule ghép vào ở bước cuối).
5. **Mức can thiệp AI:** Chọn **Workflow** có AI ở duy nhất Bước 4 (soạn nháp nhận xét), vì quy trình gồm các bước cố định; No AI chính là file câu mẫu bị phụ huynh chê, Rule chỉ ghép câu thô không nối được tiến trình hai đợt, còn Agent tự trị không cần thiết và bị cấm vì rủi ro phát ngôn sai.
6. **Quyết định:** Chọn **GO ở phạm vi nhỏ** (pilot 4 tuần trên 1 lớp 35 học sinh của GV-A bằng Google Sheets và một prompt chuẩn hóa), kèm 3 ngưỡng dừng rõ ràng: dừng nếu giáo viên phải viết lại trên 35% bản nháp, dừng ngay lập tức nếu xuất hiện 01 lỗi sai kiến thức ở đề thi hoặc nhận xét sai dữ liệu suýt gửi phụ huynh, hoặc No-Go nếu ban giám hiệu không đồng ý bằng văn bản.

---

## 7. Tài liệu tham khảo

- `RUBRIC.md`, `CHECKPOINTS.md`, `SUBMISSION.md` của repo lab (căn cứ cho card #2).
- `docs/01-worksheet.md` — prompt "product manager hoài nghi" dùng ở CP2.
- Biên bản phỏng vấn CP4 của nhóm: `report/assets/cp4-interview-snapshot-1.md` đến `-3.md`.
- Marty Cagan — *The Four Big Risks*: https://www.svpg.com/four-big-risks/
