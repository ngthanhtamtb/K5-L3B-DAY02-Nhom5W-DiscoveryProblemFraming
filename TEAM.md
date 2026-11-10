# Team — Nhom5W (Lớp L3B)

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: **Nhom5W**
- Lớp: **K5 - Level 3 (L3B)**
- Tên repo: `K5-L3B-DAY02-Nhom5W-DiscoveryProblemFraming`
- Candidate problem nhóm chọn (1 câu): **Tối ưu hóa chu trình kiểm tra định kỳ và tự động hóa báo cáo tiến trình học tập cá nhân hóa gửi phụ huynh cho giáo viên THPT.**
- Quyết định cuối (Go / Not Yet / No-Go): **Go, phạm vi nhỏ (Pilot 4 tuần trên 1 lớp 35 học sinh).**

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | **Nguyễn Thành Tâm** | **2A202603933** | **Nhóm trưởng**, điều phối thời gian, xây dựng cây OST, phân tích AI Canvas & 4 mức AI | `ngthanhtamtb` |
| 2 | **Lê Tuấn Đạt** | **2A202603949** | Phụ trách Research giải pháp thị trường, thiết kế quy trình Trước/Sau, viết Problem Statement v0/v1 | `letuandat131` |
| 3 | **Nguyễn Huy Tấn** | **2A202603925** | Phụ trách Assumption Map, phỏng vấn The Mom Test, kiểm chứng dữ liệu thực tế & đánh giá 4 rủi ro | `Besoi2004` |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Nguyễn Thành Tâm | Lê Tuấn Đạt, Nguyễn Huy Tấn | 4 cluster từ 9 card của 3 người, cây OST rút gọn, bảng ma trận chấm điểm & xử lý bất đồng |
| CP4 — Kiểm chứng | Nguyễn Huy Tấn | Lê Tuấn Đạt | Assumption map, 3 biên bản phỏng vấn The Mom Test (`report/assets/`), tổng hợp tín hiệu phản bác |
| CP4 — Research | Lê Tuấn Đạt | Nguyễn Thành Tâm | Bảng phân tích 4 giải pháp (Azota, K12Online, Khan Academy, ChatGPT) có link kiểm tra & rà soát ảo giác của AI |
| CP5 — Quy trình trước/sau | Lê Tuấn Đạt | Nguyễn Huy Tấn | Sơ đồ Mermaid Before (315') và After (115'), phản biện 2 gợi ý lệch của AI, bảng so sánh chỉ số |
| CP5 — Problem Statement v0 | Lê Tuấn Đạt | Nguyễn Thành Tâm | Bản Problem Statement v0 kèm phản biện lỗ hổng metric & chặn phình phạm vi (scope creep) từ AI |
| CP6 — Mức can thiệp + Problem Statement v1 | Nguyễn Thành Tâm | Lê Tuấn Đạt | Ma trận độ mơ hồ × phức tạp, 4 mức can thiệp (bác bỏ Agent tự hành), AI Canvas, Google PAIR, Problem Statement v1, Bộ 10 test case eval |
| CP6 — Quyết định | Nguyễn Huy Tấn | Nguyễn Thành Tâm, Lê Tuấn Đạt | Bảng chấm 4 rủi ro (Value, Usability, Feasibility, Viability), quyết định Go Pilot 4 tuần và 3 ngưỡng dừng |
---
###phần của tâm
---

### LeTuanDat-2A202603949

**Phần việc phụ trách:**
- Research giải pháp đã có (CP4 Research).
- Vẽ quy trình trước/sau (CP5).
- Viết Problem Statement v0 và sửa lên v1 (CP5, CP6).

**Đóng góp cụ thể:**
- Đưa card #1 "Chu kỳ kiểm tra định kỳ và nhận xét tiến trình của GV-A" vào buổi pitch; card được nhóm chọn làm candidate chung (34/35).
- Tự mở trang chủ 4 công cụ (Azota, K12Online, Khan Academy, ChatGPT) ngày 09/11/2026 và làm bảng research: các công cụ có chấm điểm, thống kê, kênh phụ huynh, nhưng trang chủ không nêu bước soạn nhận xét tiến trình cá nhân hóa.
- Vẽ quy trình Before (315') và After (115'): Rule ở bước sinh mã đề và ánh xạ câu sai, AI chỉ ở bước soạn nháp nhận xét, giáo viên duyệt và tự gửi.
- Viết Problem Statement v0 → v1, thêm metric chất lượng và boundary "AI không nhận họ tên học sinh"; tham gia 4 tiêu chí đánh giá và bộ 10 test case (B3).

**Bằng chứng:**
- `report/team/group_report.md`: mục 3.3 (research), mục 4 (quy trình), mục 5 (v0), mục 7 (v1 + tiêu chí + test case).
- `report/individual/2A202603949_LeTuanDat.md`.
- Commit của tài khoản `letuandat131`.

**Điều mình học được từ phần nhóm:**
- Card đầu tiên của mình có cả OCR chấm bài; sau khi AI phản biện và GV-A nói chấm bài không phải chỗ nghẽn, mình bỏ OCR và chỉ giữ phần sau khi chấm. Bài học: tìm đúng bước nghẽn trước khi nghĩ công cụ.
- Không phải problem nào cũng cần AI: card thông báo của Tấn giải được bằng một kênh chính thức. AI chỉ nên ở đúng bước mà Rule không làm được, và con người vẫn duyệt cuối.

---

###phần của tấn
---
