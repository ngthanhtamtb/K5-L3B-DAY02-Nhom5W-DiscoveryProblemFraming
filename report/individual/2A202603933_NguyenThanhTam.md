# Báo cáo cá nhân — 2A202603933_NguyenThanhTam

## 1. Thông tin học viên

- Họ tên: **Nguyễn Thành Tâm**
- MSSV: **2A202603933**
- Lớp: **K5 - Level 3 (L3B)**
- Tên nhóm: **Nhom5W**
- Link repo nhóm: https://github.com/ngthanhtamtb/K5-L3B-DAY02-Nhom5W-DiscoveryProblemFraming
- Vai trò trong nhóm: **Nhóm trưởng**, điều phối thời gian, dẫn dắt hội tụ nhóm & xây dựng cây OST (CP3), phân tích mức can thiệp AI, AI Canvas, Problem Statement v1 & bộ 10 test case đánh giá (CP6).

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

> ⚠️ Dữ liệu trong cột "Dấu hiệu thật" ở giai đoạn này là **ước lượng suy luận từ quan sát gián tiếp** (mô tả công việc, trao đổi không chính thức, bối cảnh chung). Chưa có phỏng vấn trực tiếp. Các con số được đánh dấu `[GT]` = Giả thuyết cần verify trước CP2.

**Actor tham chiếu:** Kỹ sư hiện trường / Chỉ huy công trường / Quản lý dự án xây dựng

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (nguồn & mức tin cậy) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi cuối mỗi ngày làm việc tại công trường, tôi muốn tổng hợp nhanh nhật ký thi công (khối lượng hoàn thành, nhân công, thiết bị, vật tư tiêu hao, sự cố) thành 1 báo cáo gửi về văn phòng, để chỉ huy trưởng và chủ đầu tư nắm tiến độ mà tôi không phải gõ lại dữ liệu từ sổ tay vào Excel mỗi tối. | Chỉ huy công trường, Kỹ sư hiện trường, Chỉ huy trưởng, Chủ đầu tư | **Quan sát thật:** Nhật ký công trường là yêu cầu pháp lý bắt buộc theo Nghị định 06/2021/NĐ-CP. **[GT]** ~45–60 phút/ngày gõ thủ công; mỗi dự án có 1–3 kỹ sư hiện trường chịu pain này đồng thời. **Rủi ro verify:** Hiện tại gõ thủ công hay đã có app? |
| 2 | Tốn thời gian | Khi cần quyết toán khối lượng với nhà thầu phụ vào cuối tháng, tôi muốn đối chiếu nhanh khối lượng nghiệm thu thực tế so với dự toán ban đầu và biên bản xác nhận hiện trường, để phê duyệt thanh toán đúng hạn mà không phải lật 3–4 file Excel và bản vẽ riêng lẻ. | Kỹ sư QS (định giá), Chỉ huy trưởng, Nhà thầu phụ, Kế toán dự án | **Quan sát thật:** Quyết toán theo tháng là chu kỳ cố định trong mọi dự án xây dựng. **[GT]** 2–3 ngày/tháng để đối chiếu thủ công; sai lệch khối lượng thường gây tranh chấp thanh toán. **Rủi ro verify:** Dữ liệu nghiệm thu có được lưu số không, hay vẫn là biên bản giấy ký tay? |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận được bộ hồ sơ thiết kế mới (bản vẽ thi công + thuyết minh kỹ thuật + danh mục vật liệu) từ tư vấn thiết kế, tôi muốn nhanh chóng xác định các điểm thay đổi so với phiên bản trước và những yêu cầu kỹ thuật đặc biệt cần lưu ý, để bàn giao đúng thông tin cho tổ trưởng thi công trước khi đổ bê tông. | Kỹ sư hiện trường, Tổ trưởng thi công, Giám sát tư vấn | **Quan sát thật:** Revision bản vẽ trong thi công là sự kiện thường xuyên, đặc biệt với dự án dân dụng phức tạp. **[GT]** Mỗi lần revision: 2–4 tiếng đọc và so sánh thủ công; nếu bỏ sót thay đổi → thi công sai → phá dỡ làm lại tốn kém. |
| 4 | Lặp lại | Khi cần đặt mua vật tư cho tuần thi công tiếp theo, tôi muốn tra nhanh tồn kho hiện tại tại công trường và đối chiếu với kế hoạch thi công, để lập phiếu yêu cầu mua hàng chính xác mà không thiếu hoặc thừa vật tư gây ứ đọng vốn. | Kỹ sư vật tư, Chỉ huy công trường, Phòng Mua hàng | **Quan sát thật:** Lập phiếu yêu cầu vật tư là công việc tuần/2 tuần. **[GT]** Tồn kho thường ghi sổ tay hoặc Excel riêng của từng thủ kho — không có hệ thống tập trung. **[GT]** Thiếu vật tư đột xuất khiến dừng thi công 0.5–1 ngày/sự cố. |
| 5 | Pain từ người khác | Khi giám sát của chủ đầu tư yêu cầu cung cấp hồ sơ nghiệm thu một hạng mục (biên bản kiểm tra vật liệu, biên bản nghiệm thu nội bộ, kết quả thí nghiệm, bản vẽ hoàn công), tôi muốn tập hợp và gửi đủ bộ hồ sơ trong ngày, để không làm chậm tiến độ nghiệm thu và thanh toán đợt. | Kỹ sư hiện trường, Kỹ sư hồ sơ, Chủ đầu tư / Giám sát | **Quan sát thật:** Hồ sơ nghiệm thu phân tán ở nhiều người, nhiều thời điểm — phổ biến trong ngành. **[GT]** Trung bình mất 0.5–1 ngày/hạng mục để gom hồ sơ; thiếu 1 biên bản → chủ đầu tư từ chối nghiệm thu → trễ thanh toán 15–30 ngày. |
| 6 | Tốn thời gian | Khi kỳ họp tiến độ định kỳ 2 tuần/lần với chủ đầu tư sắp diễn ra, tôi muốn so sánh nhanh tiến độ thực tế với đường cong S (kế hoạch) và xác định nguyên nhân lệch tiến độ, để trình bày được phương án xử lý thay vì chỉ báo cáo số liệu thiếu. | PM dự án, Chỉ huy trưởng, Chủ đầu tư | **Quan sát thật:** Họp tiến độ định kỳ là thông lệ tất cả dự án xây dựng. **[GT]** ~3–4 tiếng chuẩn bị slide + cập nhật đường cong S thủ công trên Excel. |
| 7 | Pain từ người khác | Khi xảy ra sự cố kỹ thuật tại công trường (nứt kết cấu, sập cốp pha, tai nạn lao động), tôi muốn lập nhanh báo cáo sự cố đúng mẫu quy định gửi chủ đầu tư và cơ quan quản lý nhà nước, để đáp ứng nghĩa vụ thông báo trong 24h theo quy định pháp luật mà không bỏ sót nội dung bắt buộc. | Chỉ huy trưởng, Ban ATLĐ, Chủ đầu tư, Sở Xây dựng | **Quan sát thật:** Nghị định 06/2021 yêu cầu báo cáo sự cố trong 24h — xác minh được từ văn bản pháp luật. **[GT]** Tần suất sự cố thực tế/dự án — cần số liệu từ người trong ngành. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý giữ lại:** Giữ lại ý #1 (Nhật ký thi công hằng ngày) và #5 (Gom hồ sơ nghiệm thu) vì impact rõ, actor cụ thể, có cơ sở pháp lý xác minh được. Giữ #3 (Đọc bản vẽ revision) vì hậu quả nặng nếu bỏ sót thay đổi kỹ thuật.
- **Ý loại bỏ:** AI từng gợi ý "Tự động hóa toàn bộ quy trình đấu thầu và lựa chọn nhà thầu". Loại bỏ vì phạm vi quá rộng, liên quan đến pháp lý đấu thầu phức tạp, không phù hợp với mục tiêu làm rõ quy trình trong một buổi lab 4 tiếng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | #1 — Nhật ký thi công hằng ngày | Lặp lại mỗi ngày → ROI cao nhất; actor cụ thể (kỹ sư hiện trường); bottleneck rõ (gõ lại sổ tay → Excel); yêu cầu pháp lý bắt buộc nên adoption không thể bỏ qua; dễ pilot trong 2 tuần | Kỹ sư hiện trường hiện ghi tay hay đã có app? Voice-to-text tiếng Việt kỹ thuật xây dựng có đủ chính xác không? |
| 2 | #5 — Gom hồ sơ nghiệm thu | Downstream impact rõ: thiếu 1 biên bản → trễ thanh toán 15–30 ngày; bottleneck là chờ hồ sơ từ nhiều người; checklist + folder Drive có thể giải một phần nhưng vẫn còn gap | Hồ sơ hiện đang lưu ở đâu (Drive, email, giấy)? Ai là người tổng hợp chính? |
| 3 | #3 — Đọc bản vẽ revision | Hậu quả nặng nếu bỏ sót (phá dỡ làm lại, chi phí cao); bài toán "so sánh 2 tài liệu" phù hợp với AI; không phụ thuộc vào hệ thống bên ngoài | Bản vẽ có ở dạng PDF có thể xử lý được không, hay là DWG/CAD? Revision cloud có được đánh dấu rõ trên bản vẽ không? |

---

### Problem Card #1 — Nhật ký thi công hằng ngày

| Trường | Nội dung |
|---|---|
| Job Story | Khi cuối mỗi ngày làm việc tại công trường, tôi muốn tổng hợp nhanh nhật ký thi công (khối lượng hoàn thành, nhân công, thiết bị, vật tư tiêu hao, sự cố) thành 1 báo cáo gửi về văn phòng, để chỉ huy trưởng và chủ đầu tư nắm tiến độ mà không phải gõ lại dữ liệu từ sổ tay vào Excel mỗi tối. |
| Actor | Kỹ sư hiện trường / Chỉ huy công trường (1–3 người/dự án) |
| Thời điểm / bối cảnh | Cuối mỗi ngày làm việc tại công trường (17:00–19:00), 5–6 ngày/tuần; thực hiện tại lán trại hoặc văn phòng công trường sau giờ thi công |
| Quy trình hiện tại (3–7 bước) | 1. Ghi chép sổ tay thực địa suốt ngày (nhân công từng tổ, thiết bị vận hành, khối lượng từng hạng mục, vật tư xuất kho, sự cố phát sinh) · 2. Về lán/văn phòng công trường, mở file Excel mẫu nhật ký · 3. Gõ lại từng mục từ sổ tay vào Excel (mất 30–40 phút) · 4. Chụp ảnh hiện trường để đính kèm · 5. Gửi file qua email hoặc Zalo về văn phòng chính |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 — gõ lại dữ liệu từ sổ tay vào Excel: **[GT]** ~30–40 phút/ngày; đây là công việc thuần nhập liệu, không tạo thêm giá trị, dễ xảy ra lỗi sót dòng hoặc sai số |
| Impact (nếu không giải thì sao) | **[GT]** ~45–60 phút/ngày/kỹ sư bị lãng phí; với 2 kỹ sư = 90–120 phút lãng phí/ngày/dự án; báo cáo hay bị trễ, thiếu chi tiết, hoặc bỏ sót sự cố nhỏ làm mất bằng chứng khi tranh chấp sau này; vi phạm Nghị định 06/2021 nếu nhật ký không đầy đủ |
| Success metric (baseline → target) | Baseline: **[GT]** 45–60 phút/ngày/kỹ sư (cần bấm giờ thực tế 1 tuần để xác nhận) → Target: < 15 phút/ngày · Đo bằng: kỹ sư tự bấm giờ trong 2 tuần pilot |
| Phương án không dùng AI | Template Excel chuẩn hóa + Google Form trên điện thoại nhập liệu tại chỗ → giảm bước gõ lại nhưng vẫn phải nhập từng trường thủ công |
| Giả thuyết về AI (nếu có) | Kỹ sư nói vào điện thoại (voice memo) tóm tắt ngày làm việc → AI transcribe + parse theo cấu trúc nhật ký (nhân công, thiết bị, khối lượng, sự cố) → điền vào template → kỹ sư review và xác nhận trước khi gửi |
| Cảm nhận nhanh | **Workflow** — các bước định sẵn rõ ràng; AI làm bước parse/điền; con người review trước khi gửi |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~50 phút/ngày

[Ghi chép sổ tay thực địa (cả ngày)]
→ [Mở Excel mẫu nhật ký: 5']
→ [Gõ lại từng mục từ sổ tay: 30–40'] ← BOTTLENECK
→ [Chụp ảnh đính kèm: 5']
→ [Gửi email/Zalo về văn phòng: 5']

TƯƠNG LAI — ~15 phút/ngày

[Ghi chép sổ tay thực địa (cả ngày)]
→ [Nói voice memo tóm tắt cuối ngày: 3–5'] ← Thay thế bước gõ lại
→ [AI transcribe + parse → điền vào template: 1–2'] ← AI
→ [Kỹ sư review, bổ sung nếu thiếu: 5–7']  ← CON NGƯỜI (boundary: AI không tự gửi)
→ [Xác nhận và gửi: 2']

Phương án quay về: AI parse sai → kỹ sư tự điền theo template Excel cũ
```

---

### Problem Card #2 — Gom hồ sơ nghiệm thu theo yêu cầu

| Trường | Nội dung |
|---|---|
| Job Story | Khi giám sát của chủ đầu tư yêu cầu cung cấp hồ sơ nghiệm thu một hạng mục (biên bản kiểm tra vật liệu, biên bản nghiệm thu nội bộ, kết quả thí nghiệm, bản vẽ hoàn công), tôi muốn tập hợp và gửi đủ bộ hồ sơ trong ngày, để không làm chậm tiến độ nghiệm thu và thanh toán đợt. |
| Actor | Kỹ sư hiện trường / Kỹ sư hồ sơ (người tổng hợp); liên quan đến kỹ sư thí nghiệm, kỹ sư vật liệu, cán bộ kỹ thuật từng hạng mục |
| Thời điểm / bối cảnh | Khi có yêu cầu nghiệm thu hạng mục (không định kỳ, đột xuất); thường có áp lực thời gian vì liên quan trực tiếp đến thanh toán đợt |
| Quy trình hiện tại (3–7 bước) | 1. Nhận yêu cầu từ giám sát (danh sách hồ sơ cần nộp) · 2. Xác định từng loại biên bản cần có theo checklist nghiệm thu · 3. Liên hệ từng người giữ từng loại hồ sơ qua Zalo/điện thoại · 4. Chờ nhận file scan hoặc bản cứng từ từng người (thường mất nửa ngày vì người bận thi công) · 5. Kiểm tra đủ bộ, đúng nội dung, đúng mốc thời gian · 6. Đóng gói và gửi (email + hard copy) |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3+4 — chờ hồ sơ từ nhiều người: **[GT]** ~4–6 tiếng; người giữ hồ sơ không ưu tiên vì đang bận việc thi công; hồ sơ phân tán nhiều nơi (email cũ, folder máy tính cá nhân, bản cứng trong tủ) |
| Impact (nếu không giải thì sao) | Thiếu 1 biên bản → chủ đầu tư từ chối nghiệm thu → trễ thanh toán đợt 15–30 ngày → ảnh hưởng dòng tiền dự án; kỹ sư mất thời gian chạy theo đốc thúc từng người |
| Success metric (baseline → target) | Baseline: **[GT]** 0.5–1 ngày làm việc/hạng mục để gom đủ hồ sơ → Target: < 2 tiếng · Tỷ lệ nghiệm thu passed lần đầu (không bị yêu cầu bổ sung): đo theo số lần nghiệm thu/quý |
| Phương án không dùng AI | Checklist chuẩn hóa theo loại hạng mục + folder Drive chia sẻ theo hạng mục → giảm quên sót nhưng vẫn phải gom thủ công |
| Giả thuyết về AI (nếu có) | AI scan yêu cầu từ giám sát → đối chiếu với kho hồ sơ Drive → báo thiếu tài liệu nào, cần lấy từ ai → tự động gửi nhắc nhở đến người phụ trách → kỹ sư review bộ hồ sơ hoàn chỉnh trước khi gửi |
| Cảm nhận nhanh | **Workflow** — các bước định sẵn; AI làm bước đối chiếu và nhắc nhở; con người kiểm tra và gửi |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~0.5–1 ngày/hạng mục

[Nhận yêu cầu từ giám sát: 15']
→ [Xác định checklist cần nộp: 15']
→ [Liên hệ từng người qua Zalo/điện thoại: 30']
→ [Chờ nhận file từ từng người: 3–5h] ← BOTTLENECK
→ [Kiểm tra đủ bộ, đúng nội dung: 30']
→ [Đóng gói + gửi: 30']

TƯƠNG LAI — ~2 tiếng/hạng mục

[Nhận yêu cầu từ giám sát: 15']
→ [AI đối chiếu với kho Drive → báo thiếu gì: 5'] ← AI
→ [AI tự gửi nhắc nhở đến người phụ trách: 5'] ← AI
→ [Người phụ trách upload hồ sơ: 60'] ← CON NGƯỜI (vẫn cần người upload)
→ [Kỹ sư review đủ bộ: 20']             ← CON NGƯỜI (boundary: AI không tự gửi cho CĐT)
→ [Gửi cho giám sát: 15']

Phương án quay về: AI miss hồ sơ → kỹ sư dùng checklist Excel thủ công
```

---

### Problem Card #3 — Đọc bản vẽ revision, xác định thay đổi kỹ thuật

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận được bộ hồ sơ thiết kế mới (bản vẽ thi công + thuyết minh kỹ thuật + danh mục vật liệu) từ tư vấn thiết kế, tôi muốn nhanh chóng xác định các điểm thay đổi so với phiên bản trước và những yêu cầu kỹ thuật đặc biệt cần lưu ý, để bàn giao đúng thông tin cho tổ trưởng thi công trước khi đổ bê tông. |
| Actor | Kỹ sư hiện trường (người nhận và đọc bản vẽ); Tổ trưởng thi công (người nhận thông tin); Giám sát tư vấn (người phát hành revision) |
| Thời điểm / bối cảnh | Mỗi khi tư vấn phát hành revision bản vẽ (không định kỳ, có thể 1–3 lần/tháng/dự án); thường có áp lực thời gian vì tổ thi công đang chờ để triển khai |
| Quy trình hiện tại (3–7 bước) | 1. Nhận bộ bản vẽ mới qua email (PDF hoặc DWG) · 2. Tìm phiên bản cũ tương ứng trong máy hoặc server · 3. So sánh thủ công từng trang, từng sheet (đọc revision cloud nếu có, hoặc so sánh mắt) · 4. Ghi chép danh sách thay đổi vào sổ hoặc email nội bộ · 5. Họp brief với tổ trưởng thi công · 6. Lưu trữ version mới, đánh dấu version cũ obsolete |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 — so sánh thủ công từng trang: **[GT]** 2–4 tiếng/lần revision; bản vẽ dân dụng thường 30–80+ sheet; không phải sheet nào cũng có revision cloud rõ ràng |
| Impact (nếu không giải thì sao) | Bỏ sót thay đổi kỹ thuật → thi công sai spec → phá dỡ làm lại (chi phí có thể lên đến hàng chục triệu đồng/sự cố) + trễ tiến độ + tranh chấp trách nhiệm với tư vấn |
| Success metric (baseline → target) | Baseline: **[GT]** 2–4 tiếng/lần revision → Target: < 30 phút/lần · Tỷ lệ sự cố thi công sai do missed revision: từ X → 0 (đo theo số sự cố/quý) |
| Phương án không dùng AI | Hệ thống document control (Procore, Autodesk Construction Cloud) có tính năng revision tracking tự động → highlight delta giữa 2 version; nhưng cần đầu tư phần mềm và onboarding |
| Giả thuyết về AI (nếu có) | AI so sánh 2 file PDF bản vẽ → liệt kê danh sách thay đổi theo sheet (kích thước, cao độ, vật liệu, ghi chú) → kỹ sư review danh sách và xác nhận trước khi brief tổ thi công |
| Cảm nhận nhanh | **Workflow** — bước AI là bước so sánh document; con người review và xác nhận (vì AI có thể miss thay đổi tinh vi về ký hiệu kỹ thuật) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~3 tiếng/lần revision

[Nhận bản vẽ mới qua email: 5']
→ [Tìm phiên bản cũ tương ứng: 10–15']
→ [So sánh thủ công từng sheet: 90–180'] ← BOTTLENECK
→ [Ghi chép danh sách thay đổi: 20']
→ [Brief tổ trưởng thi công: 20']
→ [Lưu trữ + đánh dấu obsolete: 10']

TƯƠNG LAI — ~30 phút/lần revision

[Nhận bản vẽ mới qua email: 5']
→ [Upload 2 version vào tool: 2']
→ [AI so sánh → xuất danh sách thay đổi theo sheet: 3–5'] ← AI
→ [Kỹ sư review danh sách, check thay đổi tinh vi: 15'] ← CON NGƯỜI
   (boundary: AI không tự thông báo cho tổ thi công)
→ [Brief tổ trưởng thi công dựa trên danh sách: 10']
→ [Lưu trữ + đánh dấu obsolete: 5']

Phương án quay về: AI so sánh sai/miss → kỹ sư đọc thủ công theo quy trình cũ
```

---

### Card muốn pitch nhất

- **Card số:** #1 — Nhật ký thi công hằng ngày
- **Vì sao:** Lặp lại mỗi ngày làm việc (5–6 ngày/tuần) → ROI cao nhất nếu giải được; bottleneck gõ lại dữ liệu rõ ràng, dễ đo; bắt buộc pháp lý (Nghị định 06/2021) nên người dùng không thể bỏ bước này; giải pháp voice-to-text + AI parse có thể pilot nhanh chỉ cần điện thoại, không cần đầu tư hệ thống.
- **Câu hỏi muốn nhóm phản biện:** (1) Kỹ sư hiện trường có chịu bỏ thói quen ghi sổ tay không? (2) Nếu số liệu khối lượng bị parse sai mà kỹ sư không phát hiện → ai chịu trách nhiệm?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 50 phút chỉ là ước lượng, chưa có bấm giờ thực tế | Đồng ý | Đánh dấu `[GT]`, thêm cách đo vào Success metric (bấm giờ 1 tuần trước pilot) |
| Voice-to-text dễ sai tên hạng mục kỹ thuật tiếng Việt | Đồng ý một phần | Thêm bước "kỹ sư review" bắt buộc trước khi gửi; AI không tự động gửi |
| Chưa rõ ai sở hữu template nhật ký — kỹ sư tự làm hay do CĐT áp mẫu | Đồng ý | Thêm vào "Điều còn chưa chắc" ở bảng chọn top 3 |
| Gợi ý làm Agent tự gửi báo cáo về văn phòng mỗi tối | Không đồng ý | Giữ boundary rõ: AI không tự gửi; kỹ sư phải xác nhận trước |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| **Pitch Problem Card** | Trình bày 3 Problem Cards ngành xây dựng (#4 Nhật ký thi công hằng ngày, #5 Gom hồ sơ nghiệm thu, #6 Đọc bản vẽ revision), trọng tâm pitch Card #1 (ứng với candidate #4 trong bảng nhóm). | Candidate #4 lọt vào shortlist 3 bài toán đại diện 3 bối cảnh để chấm điểm (đạt 23/35 điểm); nhóm thống nhất giữ làm hướng mở rộng về sau vì trong thời gian lab chưa tiếp cận được kỹ sư hiện trường để kiểm chứng số liệu `[GT]`. |
| **Phản biện bài của bạn khác** | **Câu hỏi tôi đã đặt:**<br>1. Hỏi Lê Tuấn Đạt (candidate #1 — Nhận xét 70 em): *"Giáo viên duyệt 70 bản nháp trong 35 phút có thực tế không, hay sẽ đọc lướt rồi bấm gửi?"*<br>2. Hỏi Nguyễn Huy Tấn (candidate #8 — Đối chiếu bài lab với rubric): *"RUBRIC.md đã như một checklist, tự tick theo đó có đủ không?"*<br>3. Hỏi Nguyễn Huy Tấn (candidate #9 — Tìm tin nhắn cũ trên Discord): *"Discord đã có ô tìm kiếm, vậy mất 10 phút là do tìm kiếm kém hay do không nhớ từ khóa?"* | - Câu hỏi 1 trở thành **Giả định #4 (Usability Risk)** trong Assumption Map (mục 3.1) và mục 8.1 của `group_report.md`, buộc nhóm thiết kế giao diện duyệt dạng thẻ, đo thực tế thời gian duyệt trong pilot và đặt ngưỡng dừng nếu phải viết lại > 35%.<br>- Câu hỏi 2 & 3 giúp nhóm loại sớm candidate #8 (No AI checklist đã đủ) và #9 (Discord đã có tìm kiếm, pain thực tế nhỏ) ở mục 2.4. |
| **Nhận phản biện** | **Câu hỏi tôi nhận được:**<br>1. Lê Tuấn Đạt hỏi (#4 Nhật ký thi công): *"Con số 45–60 phút/ngày lấy từ đâu, đã hỏi kỹ sư hiện trường nào chưa?"*<br>2. Nguyễn Huy Tấn hỏi (#5 Hồ sơ nghiệm thu): *"Nghẽn là do chờ người khác gửi hồ sơ; có nhắc nhở thì họ có gửi nhanh hơn không, hay checklist + thư mục chung là đủ?"*<br>3. Lê Tuấn Đạt hỏi (#6 Bản vẽ revision): *"Bản vẽ đang ở dạng PDF hay DWG? Nếu là DWG thì phần mềm CAD có sẵn chức năng so revision chưa?"* | **Tôi đã sửa gì:** Thừa nhận minh bạch cả 3 card xây dựng mới dừng ở mức giả thuyết `[GT]`, trong đó card #5 có thể giải phần lớn bằng No AI (checklist + folder Drive chung) và card #6 phụ thuộc định dạng CAD/PDF. Tôi chủ động chấm bài mình 2/5 ở tiêu chí "Pain có bằng chứng" & "Nhóm hiểu domain", đồng thuận nhường quyền ưu tiên cho candidate #1 (GV-A) có người thật kiểm chứng ngay ở CP4. |
| **Gom cluster / cây OST** | Phụ trách chính CP3: Điều phối nhóm gom 9 candidate từ 3 bối cảnh theo **pattern công việc** thành 4 cluster (A, B, C, D); trực tiếp vẽ sơ đồ Mermaid cây Opportunity Solution Tree rút gọn (mục 2.3). | Giúp nhóm tìm ra điểm hội tụ chung ở Cluster A (*chép dữ liệu có sẵn sau mỗi chu kỳ thành báo cáo cá nhân hóa*) và lọc bỏ dứt điểm 4 "solution đội lốt opportunity" (OCR chấm bài giấy, agent tự gửi báo cáo công trường, app gom 4 kênh, chatbot trả lời phụ huynh). |
| **Chọn candidate problem** | Thiết lập bảng chấm điểm shortlist 7 tiêu chí (mục 2.4), điều phối xử lý bất đồng về phạm vi đề tài #1. | Chốt chọn candidate #1 (34/35 điểm) có lập luận loại trừ rõ cho cả 8 bài còn lại; thống nhất cắt bỏ hoàn toàn tính năng OCR chấm bài giấy khỏi đề tài chung. |
| **Kiểm chứng / research** | Hỗ trợ Lê Tuấn Đạt thực hiện CP4 Research (mục 3.3): Cùng mở và đối chiếu trực tiếp trang chủ 4 công cụ (Azota, K12Online, Khan Academy, ChatGPT) ngày 09/11/2026. | Xác nhận khoảng trống thực tế: các nền tảng Việt Nam mạnh về chấm điểm/thống kê nhưng trang chủ không nêu bước chuyển danh sách câu sai thành nhận xét tiến trình 3 phần; giúp nhóm chốt hướng không xây lại app chấm thi mà chỉ làm Workflow nối sau bước chấm. |
| **Quy trình nhóm** | Cùng Đạt và Tấn rà soát quy trình Before (315') và After (115', tiết kiệm 200' ~ 63%), phân định rạch ròi vai trò Rule — AI Workflow — Con người (mục 4). | Giữ nguyên 65 phút cho bước giáo viên chấm bài + nhập mã câu sai (không ép tự động hóa chỗ không nghẽn) và thiết lập chốt chặn HITL 35 phút ở Bước 5 kèm phương án Fallback về mẫu nhận xét cũ. |
| **Problem Statement** | Hỗ trợ Đạt rà soát Problem Statement v0 (CP5) và phụ trách chính nâng cấp lên **Problem Statement v1 + Bộ tiêu chí đánh giá & 10 Test Case Eval** (CP6, mục 7). | Bổ sung 2 metric chất lượng vào v1 (tỉ lệ viết lại < 15%, > 80% phụ huynh thấy rõ phần cần ôn), siết Boundary bảo mật (chỉ truyền mã học sinh cho AI, họ tên thật do Rule chèn sau), hoàn thiện 4 tiêu chí đánh giá và bộ 10 test case Ground Truth (TC01–TC10) đạt chuẩn 40–90 từ. |
| **Mức can thiệp AI** | Phụ trách chính CP6 (mục 6): Xây dựng ma trận Độ mơ hồ × Độ phức tạp, bảng so sánh 4 mức (No AI / Rule / Workflow / Agent), AI Canvas rút gọn và trả lời 2 câu hỏi Google PAIR. | Chứng minh rõ vì sao dùng Rule cho Bước 1 & 3, chỉ dùng AI Workflow ở Bước 4; chốt nguyên tắc **Augment** và thiết kế chống lỗi **Báo nhầm (False Positive)** vì bịa lỗi sai của học sinh gây hậu quả sư phạm nghiêm trọng hơn bỏ sót. |
| **Quyết định** | Hỗ trợ Nguyễn Huy Tấn rà soát bảng đánh giá 4 rủi ro (Value, Usability, Feasibility, Viability) và thiết kế kế hoạch Pilot + ngưỡng dừng (mục 8). | Thống nhất quyết định **Go phạm vi nhỏ** (Pilot 4 tuần / 2 chu kỳ trên 1 lớp 35 học sinh bằng Google Sheets + Prompt chuẩn), chốt 2 điều kiện tiên quyết trước pilot và 3 ngưỡng dừng định lượng (Stop Conditions). |

---

## 5. Dùng AI

*(Lưu ý: Ở CP3 Pitch & phản biện và CP4 Phỏng vấn người thật, nhóm tuân thủ quy định không sử dụng AI).*

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| **CP1 Scan** | Dùng AI gợi ý mở rộng góc nhìn theo 4 lăng kính cho bối cảnh công trường Xây dựng và đóng vai kỹ sư giải pháp để rà soát rủi ro giả định cho 7 job stories. | Giúp hệ thống hóa Assumption Risk Map, nhắc tách bạch giữa quan sát thực tế (quy định Nghị định 06/2021/NĐ-CP) với các con số ước lượng chưa có log bấm giờ thực địa. | Gợi ý bài toán phạm vi quá rộng không vừa sức lab 4 tiếng (*"Tự động hóa toàn bộ quy trình đấu thầu và lựa chọn nhà thầu"*) và có xu hướng đưa ra con số ước lượng nghe rất chắc chắn dù chưa phỏng vấn thực tế. | Loại bỏ ý tự động hóa đấu thầu; giữ lại 7 job stories sát nghiệp vụ công trường và chủ động gắn nhãn `[GT]` minh bạch kèm rủi ro cần verify cho mọi con số ước lượng. |
| **CP2 Problem Card** | Hỗ trợ chuẩn hóa cấu trúc 3 Problem Cards xây dựng và đóng vai PM hoài nghi để phản biện Card #1 (Nhật ký thi công). | Chỉ đúng điểm yếu: baseline 50 phút mới dựa trên ước lượng và rủi ro voice-to-text tiếng Việt nhận diện sai thuật ngữ kỹ thuật xây dựng, tên hạng mục. | Đề xuất hướng làm Agent tự động gửi báo cáo nhật ký về văn phòng mỗi tối và mặc định kỹ sư được tự đổi mẫu biểu báo cáo. | Bác bỏ hướng Agent tự gửi, giữ Boundary bắt buộc kỹ sư review trước khi gửi; bổ sung phương án quay về Excel mẫu cũ và đưa câu hỏi về quyền sở hữu biểu mẫu của CĐT vào mục "Điều còn chưa chắc". |
| **CP4 Research** | Tìm kiếm và đối chiếu các công cụ EdTech tương đương cho bài toán của GV-A (Azota, K12Online, Khan Academy, ChatGPT). | Gợi ý nhanh danh sách các nền tảng sát bối cảnh trường phổ thông Việt Nam và mô hình gắn thẻ kỹ năng (Competency Tagging) của Khan Academy. | Bị **ảo giác (hallucination)** nói quá rằng *"Azota và K12Online hiện đã có sẵn AI tự động phân tích lỗ hổng kiến thức và viết nhận xét cá nhân hóa gửi phụ huynh"*. | Không tin ngay câu trả lời của AI: cùng Đạt trực tiếp mở `azota.vn` và `k12online.vn` (ngày 09/11/2026) để kiểm tra, gạch bỏ nhận định ảo giác của AI và ghi đúng thực tế là trang chủ chỉ nêu chấm trắc nghiệm/thống kê điểm, chưa nêu tính năng soạn nhận xét tiến trình dài hạn. |
| **CP5 Quy trình** | Hỗ trợ vẽ sơ đồ Mermaid Before (315') / After (115') và dùng prompt phản biện tìm lỗ hổng quy trình tương lai. | Tạo nhanh bố cục sơ đồ trực quan, phân biệt màu sắc rõ giữa các bước Rule, AI Workflow và Con người (HITL). | Đưa ra 2 gợi ý quá đà theo hướng "ham tự động hóa": (1) đòi dùng LLM tự sinh 3 bộ câu hỏi mới ở Bước 1 thay vì Rule, và (2) đòi gộp Bước 4 + Bước 5 cho AI tự gửi thẳng tin nhắn phụ huynh qua API để ép thời gian từ 115' xuống 60'. | Bác bỏ cả 2 đề xuất của AI: giữ Bước 1 là **Rule** (vì đề định kỳ bắt buộc lấy từ ngân hàng đã thẩm định của trường) và giữ chặt Bước 5 là con người duyệt 35' (tổng 115') theo lệnh cấm máy tự gửi của Tổ trưởng chuyên môn. |
| **CP5–6 Problem Statement** | Dùng prompt *"Chỉ ra lỗ hổng trong Problem Statement v0, không viết lại thay tôi"* trước khi nâng cấp lên bản v1. | Chỉ ra hợp lý việc bản v0 chỉ đo tốc độ thời gian (315' → < 120'), thiếu thước đo chất lượng bản nháp và sự đón nhận của phụ huynh. | Gợi ý bị lệch gây phình phạm vi (scope creep): khuyên mở rộng cho *"toàn bộ các môn học THPT (cả tự luận Văn, Sử, Địa) và tích hợp chatbot AI giải đáp phụ huynh 24/7"*; đồng thời chưa tính đến rủi ro lộ tên thật học sinh (PII). | Đồng ý bổ sung 2 metric chất lượng vào v1 (tỉ lệ viết lại < 15%, phụ huynh thấy rõ phần cần ôn > 80%) và ẩn danh họ tên học sinh ở Boundary; bác bỏ hoàn toàn việc mở rộng sang môn xã hội tự luận và chatbot 24/7, khóa chặt ở Toán/KHTN có ma trận K1–K3. |
| **CP6 Mức can thiệp / quyết định** | Phản biện lựa chọn mức can thiệp AI và hỗ trợ nháp khung tình huống cho bộ 10 Test Case đánh giá (Eval Set TC01–TC10). | Giúp bao phủ nhanh nhiều trường hợp biên cho bộ test case (học sinh đạt 10/10, tụt điểm khi sang hình học không gian mới, hết giờ bỏ trống câu cuối, sai câu dễ do tính nhẩm). | Ban đầu gợi ý chọn mô hình **Autonomous Agent** tự hành từ khâu lấy ngân hàng đề đến gửi tin cho phụ huynh; ở TC04 (học sinh 10/10, không sai câu nào) AI áp máy móc khung 3 phần dễ gượng ép tìm "lỗ hổng" và đếm lệch số từ tiếng Việt. | Kiên quyết bác bỏ Agent tự hành để kéo mức can thiệp về **Workflow (HITL)** an toàn sư phạm; thêm ngoại lệ vào Tiêu chí 2 (*"Học sinh không sai câu nào thì phần (2) được bỏ"*) và tự đếm tay chuẩn hóa toàn bộ 10 test case trong khoảng 47–68 từ (chuẩn 40–90 từ). |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi nghe Đạt trình bày các bài toán của giáo viên THPT và Tấn chia sẻ vấn đề trôi thông báo, tôi thấy là dù 3 thành viên xuất phát từ 3 lĩnh vực hoàn toàn khác nhau (trường phổ thông, khóa học công nghệ, công trường xây dựng), bản chất nỗi đau lại hội tụ về cùng một vài pattern công việc lặp lại — điển hình là việc phải tra cứu dữ liệu có sẵn sau mỗi chu kỳ rồi gõ tay thành báo cáo cho từng người nhận. Tôi cũng học được từ bài của Đạt tầm quan trọng của việc chọn bài toán tiếp cận được người thật ngay trong thời gian ngắn, còn bài của Tấn cho tôi thấy một góc nhìn rất thực tế: có những vấn đề gây phiền toái cho cả trăm người mỗi ngày nhưng cách giải đúng đắn nhất lại là quy chuẩn hóa quy trình (No AI — thống nhất một nguồn thông báo chính thức) chứ không phải cố xây thêm công cụ AI.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Nhóm đã vấp vào bẫy "solution-first" ngay ở giai đoạn đầu: bản phác thảo đầu tiên cho bài toán giáo viên từng ôm đồm cả ý tưởng dùng OCR nhận diện chữ viết tay để chấm bài tự động, hay ở bài thông báo của Tấn ban đầu cũng dễ nghĩ ngay tới việc làm một app gom tin từ 4 kênh. Nhóm nhận ra điều này ở hai thời điểm: lần một là khi tôi điều phối vẽ cây OST ở CP3, cả nhóm rà soát và phải gạch bỏ 4 ý tưởng thực chất là tính năng đội lốt cơ hội; lần hai quyết định nhất là khi Tấn và Đạt mang kết quả phỏng vấn GV-A về ở CP4 — cô giáo nói rõ việc chấm 70 bài theo barem chỉ mất 45 phút và không hề làm cô mệt, thứ làm cô "sợ phát khóc" tối Chủ nhật là ngồi nhớ lỗi cũ từng học sinh để gõ nhận xét. Ngay lúc đó, nhóm thống nhất cắt bỏ hoàn toàn OCR, giữ nguyên bước chấm bài cho giáo viên và thu hẹp phạm vi chỉ từ sau khi đã có điểm và mã câu sai.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Tôi đã thay đổi quyết định rất lớn ở CP3. Trước buổi họp nhóm, tôi đã đầu tư xây dựng kỹ bộ 7 job stories và 3 Problem Cards trong lĩnh vực xây dựng, tâm đắc nhất là Card Nhật ký thi công hằng ngày vì có căn cứ pháp lý Nghị định 06/2021 rõ ràng và tần suất lặp lại mỗi tối. Tuy nhiên khi pitch, Đạt hỏi thẳng: *"Con số 45–60 phút/ngày lấy từ đâu, đã hỏi kỹ sư hiện trường nào chưa?"*, còn Tấn chất vấn ở card hồ sơ nghiệm thu rằng nếu nghẽn do chờ người khác gửi file thì liệu một checklist kèm thư mục chung đã đủ chưa. Những câu hỏi đó chạm đúng điểm yếu cốt tử: toàn bộ số phút trong bài xây dựng của tôi đều đang gắn nhãn giả thuyết `[GT]` và trong vài tiếng làm lab, cả nhóm không thể tìm đâu ra kỹ sư công trường để phỏng vấn theo The Mom Test. Với vai trò nhóm trưởng, thay vì cố bảo vệ bài mình, tôi chủ động chấm card của mình 2/5 ở cột bằng chứng và đồng thuận cùng nhóm chọn đề tài GV-A của Đạt để đào sâu.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Kết quả kiểm chứng làm tôi bất ngờ. Qua biên bản phỏng vấn, tôi không ngờ giáo viên chỉ gõ nhận xét thật được cho khoảng 25–30 em đầu tiên rồi kiệt sức phải copy câu mẫu từ file Word, dẫn đến ước tính của tổ trưởng là khoảng 70% sổ liên lạc bị rập khuôn, kéo theo cảnh phụ huynh nhận điểm 7.5 của con vẫn phải chụp màn hình nhắn Zalo hỏi cô giáo vào tối muộn — tức là cách làm đối phó hiện tại vô tình đẻ thêm việc ngược lại cho chính giáo viên. 
Ở bước Research, khi trực tiếp mở kiểm tra Azota và K12Online, tôi thấy các nền tảng nội địa đã giải quyết rất tốt khâu chấm thi và lên bảng điểm, nhưng lại bỏ ngỏ đúng "dặm cuối" là chuyển hóa mã câu sai thành lời nhận xét sư phạm 3 phần. Nhờ phát hiện này, nhóm hoàn toàn bỏ ý định xây hệ thống lớn mà chỉ thiết kế một Workflow gọn nhẹ chạy trên Google Sheets.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Phần khó nhất với tôi là cân bằng giữa tốc độ và chất lượng trong **Success Metric**, đồng thời thiết lập **Boundary** sao cho an toàn tuyệt đối với môi trường học đường. Ở bản v0, nhóm chỉ đưa vào mục tiêu giảm thời gian từ 315 phút xuống dưới 120 phút. Khi rà soát lại để lên bản v1, tôi nhận ra nếu chỉ tối ưu số phút thì AI có thể phóng bút rất nhanh nhưng sinh ra nhận xét vô hồn hoặc nhầm dữ liệu, khiến giáo viên phải xóa đi gõ lại còn cực hơn cũ. Việc thiết kế thêm hai thước đo kiểm chứng được — tỉ lệ bản nháp phải viết lại từ đầu dưới 15% và khảo sát 1 câu với phụ huynh đạt trên 80% thấy rõ phần con cần ôn — kèm theo quy tắc tách họ tên thật của học sinh ra khỏi dữ liệu gửi cho AI là bước đòi hỏi nhóm phải tranh luận kỹ lưỡng nhất.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại từ đầu, ở phần cá nhân CP1–CP2 tôi sẽ chọn quét vấn đề ngay trong quy trình làm việc/học tập hằng ngày mà tôi có sẵn lịch sử bấm giờ hoặc hỏi được người trong cuộc ngay lập tức, tránh chọn domain xây dựng gián tiếp khiến mọi chỉ số dừng ở mức giả thuyết. Ở phần nhóm, tôi sẽ phản biện gắt gao hơn ở hai điểm: một là yêu cầu đo bấm giờ thực tế ít nhất 5–10 học sinh mẫu để kiểm chứng con số ước lượng 170 phút viết nhận xét và 35 phút đọc duyệt (vì 30 giây đọc và sửa một nhận xét cho 70 em liên tục vẫn có nguy cơ gây mỏi mắt, đọc lướt); hai là rà soát kỹ kịch bản câu hỏi phỏng vấn trước khi đi hỏi để tránh lọt câu hỏi giả định *"Nếu có tiện ích... nhà trường có cho phép không?"* trong buổi gặp tổ trưởng chuyên môn, giúp bằng chứng Viability vững chắc hơn ngay từ CP4.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Bài toán của nhóm tập trung vào nỗi đau của giáo viên Toán THPT (đại diện là GV-A phụ trách 2 lớp, 70 học sinh) khi mỗi chu kỳ kiểm tra 2 tuần phải mất 315 phút, trong đó nghẽn nặng nhất ở khâu cân bằng 3 mã đề (45 phút) và tra lịch sử lỗi sai để gõ nhận xét cá nhân hóa cho 70 em (170 phút), khiến giáo viên kiệt sức phải copy câu mẫu còn phụ huynh không biết con hổng phần nào để kèm cặp. Trong quy trình tương lai 6 bước (kỳ vọng còn 115 phút), giáo viên vẫn trực tiếp chấm bài và nhập mã câu sai (65 phút), hệ thống dùng Rule tự động sinh 3 mã đề chuẩn hóa (5 phút) và ánh xạ câu sai sang mã kỹ năng kèm điểm kỳ trước (2 phút), tiếp đó AI soạn nháp 70 nhận xét theo cấu trúc 3 phần (3 phút) để giáo viên rà soát chỉnh sửa (35 phút) rồi tự bấm gửi (5 phút). Hiệu quả được đo lường bằng 3 chỉ số: giảm tổng thời gian từ 315 phút xuống dưới 120 phút/chu kỳ, tỉ lệ bản nháp giáo viên phải viết lại dưới 15%, và trên 80% phụ huynh lớp pilot xác nhận nhận xét chỉ rõ nội dung con cần ôn. Về ranh giới an toàn (Boundary), AI chỉ được nhận mã học sinh cùng mã câu sai (tên thật do Rule ghép sau), tuyệt đối không tự sửa điểm, không bịa lỗi ngoài danh sách câu sai, không dùng từ ngữ phán xét nhân cách và không được tự động gửi tin cho phụ huynh. Nhóm chọn mức can thiệp **Workflow** có con người kiểm duyệt (Rule ở Bước 1, 3 và AI ở duy nhất Bước 4) vì câu mẫu No AI hay ghép chuỗi Rule đơn thuần đều khô cứng không nối được sự tiến bộ giữa hai kỳ, trong khi Agent tự hành lại quá rủi ro về phát ngôn sư phạm trên một quy trình vốn đã cố định. Do cả 4 rủi ro (Value, Usability, Feasibility, Viability) đều ở mức Trung bình và kiểm chứng nhanh được, nhóm quyết định **Go phạm vi nhỏ**: chạy pilot 4 tuần (2 đợt kiểm tra) trên 1 lớp 35 học sinh bằng Google Sheets và prompt chuẩn sau khi có xác nhận của nhà trường, kèm ngưỡng dừng tức khắc nếu tỉ lệ viết lại vượt 35% hoặc xảy ra dù chỉ 1 lỗi ảo giác sai điểm số/kiến thức.

---

## 7. Tài liệu tham khảo

1. Chính phủ (2021) — *Nghị định 06/2021/NĐ-CP quy định chi tiết một số nội dung về quản lý chất lượng, thi công xây dựng và bảo trì công trình xây dựng* (cơ sở pháp lý cho CP1 & CP2 phần cá nhân).
2. Báo cáo nhóm Nhom5W: [group_report.md](../team/group_report.md), hồ sơ phân công [TEAM.md](../../TEAM.md) và 3 biên bản phỏng vấn CP4 ([snapshot 1](../assets/cp4-interview-snapshot-1.md), [snapshot 2](../assets/cp4-interview-snapshot-2.md), [snapshot 3](../assets/cp4-interview-snapshot-3.md)).
3. Rob Fitzpatrick — *The Mom Test*: https://www.momtestbook.com/
4. Teresa Torres — *Opportunity Solution Trees*: https://www.producttalk.org/opportunity-solution-trees/
5. Google PAIR — *People + AI Guidebook (User Needs & Mental Models)*: https://pair.withgoogle.com/chapter/user-needs/
6. Anthropic — *Building Effective Agents*: https://www.anthropic.com/research/building-effective-agents
7. Marty Cagan (SVPG) — *The Four Big Risks*: https://www.svpg.com/four-big-risks/
8. Các nền tảng đối chiếu trong phần Research nhóm (kiểm tra ngày 09/11/2026): https://azota.vn/, https://k12online.vn/, https://www.khanacademy.org/, https://chatgpt.com/
