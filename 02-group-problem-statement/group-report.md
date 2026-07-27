# Group Report — Day 02

## Thành viên nhóm

| STT | Họ và tên     | Mã học viên | Vai trò trong nhóm |
|:---:|:--------------|:-----------:|:-------------------|
|  1  | Vũ Quốc Anh   | 2A202601080 | Research           |
|  2  | Trần Tuấn Anh | 2A202601804 | Research           |
|  3  | Hà Xuân Sơn   | 2A202601904 | Research           |
|  4  | Chu Tâm Vũ    | 2A202601360 | Research           |
|  5  | Lê Trung Kiên | 2A202601182 | Làm slide          |
|  6  | Bùi Tùng Lâm  | 2A202601676 | Làm slide          |
|  7  | Lê Nhật Minh  | 2A202602023 | FAQ                |
|  8  | Chu Tuấn Việt | 2A202601082 | FAQ                |
|  9  | Trần Anh Tú   | 2A202601674 | FAQ                |
| 10  | Đỗ Quý Đức    | 2A202601828 | FAQ                |
| 11  | Giáp Quốc Anh | 2A202601522 | Trưởng nhóm        |

# 02 — Group Problem Statement

## Group convergence

Nhóm 3-4 người, mỗi người share top 3. Tổng cộng khoảng 9-12 candidates xoay quanh vấn đề quá tải bệnh viện.

| *Cluster* | *Candidate examples* | *Pattern chung* |
| :--- | :--- | :--- |
| Thu thập thông tin ban đầu | Khai báo triệu chứng cấp cứu (Triage), Lịch sử bệnh nền, Khai báo y tế | Tốn nhiều thời gian điều dưỡng hỏi đi hỏi lại các câu hỏi lặp lại với từng bệnh nhân. |
| Phân bổ nguồn lực | Xếp giường bệnh, Phân luồng phòng khám | Mất thời gian tìm kiếm thông tin phòng/giường trống và ghép nối bệnh nhân. |
| Quản lý hồ sơ / Báo cáo | Tóm tắt bệnh án chuyển tuyến, Viết báo cáo ca trực | Gom thông tin từ nhiều nguồn (HIS, xét nghiệm) để viết báo cáo bàn giao. |
| Trả kết quả | Báo kết quả X-quang/Máu, Hướng dẫn dùng thuốc | Bác sĩ/Dược sĩ tốn thời gian giải thích các chỉ số cơ bản lặp đi lặp lại. |

## Shortlist và score

| *Candidate* | *Actor rõ* | *Workflow rõ* | *Pain có evidence* | *Impact đo được* | *Làm trong lab* | *So sánh R/W/A được* | *Nhóm hiểu domain* | *Tổng* |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Phân loại bệnh (Triage)** | 5 | 5 | 5 | 5 | 4 | 5 | 4 | 33 |
| Tóm tắt bệnh án | 4 | 4 | 4 | 4 | 5 | 4 | 4 | 29 |
| Xếp giường bệnh | 3 | 3 | 5 | 4 | 2 | 4 | 3 | 24 |

Nhóm chọn: **Phân loại bệnh nhân (Triage) ban đầu**.

**Vì sao chọn:**
* Có workflow rất rõ (Bệnh nhân đến → Khai báo → Đo sinh hiệu → Phân loại ưu tiên).
* Có baseline thời gian (trung bình 5-7 phút hỏi bệnh/người, tạo ra nút thắt cổ chai ở khu chờ).
* Có thể vẽ before/after rất rõ ràng.
* Rủi ro y tế có thể kiểm soát nếu đặt đúng "Human boundary" (Điều dưỡng vẫn là người quyết định cuối cùng).

**Vì sao không chọn các bài khác:**
* Xếp giường bệnh: Phụ thuộc quá nhiều vào hệ thống HIS lõi của bệnh viện, khó làm demo/pilot trong lab.
* Tóm tắt bệnh án: Hay, nhưng impact giảm tải thời gian chờ trực tiếp của bệnh nhân không lớn bằng quy trình Triage.

## Quick validation

Nhóm hỏi nhanh 2 Điều dưỡng trưởng và 1 Bác sĩ trực cấp cứu.

| *Nguồn* | *Số người* | *Tín hiệu xác nhận* | *Tín hiệu phản bác* | *Nhóm sửa problem thế nào* |
| :--- | :--- | :--- | :--- | :--- |
| Phỏng vấn nhanh | 3 | 3/3 xác nhận khâu hỏi triệu chứng ban đầu lặp đi lặp lại tốn thời gian, bệnh nhân đông thường cáu gắt vì phải chờ lâu. | Bệnh nhân lớn tuổi không biết dùng smartphone/app để tự khai báo trước. | **Thu hẹp & Bổ sung:** AI bot có thể tương tác bằng **giọng nói** (Speech-to-text) tại Kiosk thay vì chỉ bắt nhập text. |
| Mini poll bệnh nhân | 10 | 8/10 phàn nàn vì phải chờ 30-45 phút chỉ để được lấy sinh hiệu và hỏi "đau ở đâu". | Khai báo máy sợ bác sĩ không đọc. | Cần đầu ra của AI là format chuẩn y khoa (SOAP) tích hợp sẵn vào màn hình của điều dưỡng. |

**Insight sau validation:**
Pain thật sự nằm ở việc *dịch ngôn ngữ đời thường của bệnh nhân* ("Tôi thấy nhói ở ngực từ tối qua") thành *ngôn ngữ y khoa có cấu trúc* để điều dưỡng đánh giá nhanh mức độ nguy hiểm, từ đó giảm thời gian kẹt ở quầy tiếp nhận.

## Research giải pháp

| *Nguồn / tool / case* | *Link* | *Họ giải quyết phần nào?* | *Điểm mạnh* | *Khoảng trống / rủi ro* | *Bài học cho nhóm* |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Symptomate / Ada Health | (Các app check triệu chứng) | Tự chẩn đoán và gợi ý có nên đi viện không. | AI logic tốt, có evidence y khoa. | Dùng ở nhà, không tích hợp vào quy trình tiếp nhận của bệnh viện; không có context bệnh án cũ. | Không làm "AI chẩn đoán", chỉ làm "AI thu thập và cấu trúc thông tin". |
| Kiosk khai báo y tế (Mùa Covid) | (Kiosk tại các bệnh viện) | Điền form (Rule-based) | Nhanh, auto-sync. | Form tĩnh (Checkbox) cứng nhắc, bệnh nhân không biết tick sao cho đúng bệnh phức tạp. | AI có thể chat linh hoạt để hỏi sâu hơn dựa trên câu trả lời trước, thay vì form tĩnh. |
| Ambient AI (Nuance DAX) | (Giải pháp y tế chuyên sâu) | Lắng nghe hội thoại và tự viết bệnh án. | Rất tự nhiên. | Chi phí quá đắt, cài đặt phức tạp. | Học pattern: AI lắng nghe/nhận text → cấu trúc lại → Người thật duyệt. |

**Research takeaway:**
Không nên build một Agent tự quyết định phân loại mức độ khẩn cấp (vì rủi ro y khoa/pháp lý). Hướng đi an toàn là dùng Workflow: Bệnh nhân tự khai báo (bằng text/voice qua AI Kiosk) → AI cấu trúc thành form chuẩn → Điều dưỡng xem, đo sinh hiệu, và chốt phân loại.

## Workflow before/after

**CURRENT STATE — Mất 10-15 phút / Bệnh nhân, kẹt ở quầy**

[1 Bệnh nhân bốc số] 
→ [2 Ngồi chờ tới lượt: 15-30'] 
→ [3 Điều dưỡng hỏi triệu chứng & ghi chép: 5-7'] <-- Bottleneck (quá tải ở đây)
→ [4 Điều dưỡng đo sinh hiệu: 2'] 
→ [5 Điều dưỡng phân loại (Xanh/Vàng/Đỏ): 1'] 
→ [6 Chờ bác sĩ khám]

**FUTURE STATE — Mất 3 phút / Bệnh nhân tại quầy**

[1 Bệnh nhân bốc số & tương tác với AI Kiosk/QR: 3'] -- Chờ đợi được tối ưu hóa thành thời gian tự khai báo
→ [2 AI tóm tắt thành form y khoa (SOAP): 1s] -- Workflow step
→ [3 Điều dưỡng đọc tóm tắt trên màn hình: 30s] 
→ [4 Điều dưỡng đo sinh hiệu: 2'] <-- Human boundary (Kiểm tra thực tế)
→ [5 Điều dưỡng duyệt & phân loại: 30s] 
→ [6 Chờ bác sĩ khám]

**Fallback:** Bệnh nhân không dùng được AI (ngất xỉu, quá già) → Quay lại luồng điều dưỡng tự hỏi trực tiếp (CURRENT STATE).

**Before/after impact:**

| *Metric* | *Trước* | *Sau kỳ vọng* | *Ghi chú* |
| :--- | :--- | :--- | :--- |
| Thời gian tương tác tại quầy/BN | 7-10 phút | Dưới 3 phút | Target chính (giảm tải quầy) |
| Cảm giác chờ đợi của BN | Chờ không làm gì | Có việc để làm (khai báo) | Cải thiện CX (Patient Experience) |
| Bước thủ công của ĐD | Hỏi bệnh từ số 0 | Chỉ cần đọc & xác nhận | Giảm stress cho nhân viên y tế |
| Bottleneck chính | Điều dưỡng phải gõ phím | Bệnh nhân tự khai báo chậm | Chấp nhận được vì giải phóng Điều dưỡng |

## Problem Statement v0

| *Field* | *Nội dung* |
| :--- | :--- |
| *Actor* | Điều dưỡng trực phân loại (Triage Nurse) tại khoa Khám bệnh / Cấp cứu. |
| *Workflow* | Bệnh nhân lấy số → Chờ → Điều dưỡng hỏi bệnh sử & triệu chứng → Đo sinh hiệu → Đánh giá phân loại ưu tiên. |
| *Bottleneck* | Bước Điều dưỡng hỏi và ghi chép thủ công tốn 5-7 phút/người. Khi đông bệnh nhân (sáng sớm), tạo ra hàng đợi kéo dài hàng giờ. |
| *Impact* | Bệnh nhân cáu gắt, nguy cơ bỏ sót dấu hiệu chuyển nặng khi chờ đợi; Điều dưỡng stress, burnout. |
| *Success Metric* | Giảm thời gian thao tác tại quầy của điều dưỡng từ 7 phút xuống dưới 3 phút/bệnh nhân; Tăng thông lượng bệnh nhân tiếp nhận lên gấp đôi. |
| *Boundary* | AI không tự đưa ra chẩn đoán bệnh; Không tự quyết định phân loại cấp cứu (Xanh/Đỏ); Chỉ làm nhiệm vụ cấu trúc hóa thông tin đầu vào. |

## Rule / Workflow / Agent

| *Mức* | *Phương án* | *Khi nào đủ* | *Rủi ro* | *Chọn?* |
| :--- | :--- | :--- | :--- | :--- |
| *Rule* | App/Kiosk cho bệnh nhân check box (Có/Không) các triệu chứng có sẵn. | Đủ với các bệnh lý đơn giản, khám sức khỏe định kỳ. | Cứng nhắc, không khai thác được insight ("đau nén ở ngực trái lan ra tay"). | Không chọn làm core, nhưng có thể dùng kết hợp. |
| *Workflow* | Bệnh nhân chat/nói với AI tự nhiên → AI hỏi thêm 1-2 câu → AI summarize thành form chuẩn (SOAP) → Điều dưỡng review. | Rất hợp vì flow rõ ràng, giải phóng được sức người ở khâu nhập liệu thô. | Hallucination (AI tự bịa triệu chứng), hoặc bỏ sót ý. | **Chọn** |
| *Agent* | AI Kiosk tự thu thập, tự phân tích độ nguy hiểm, tự đưa ra quyết định nhập viện hay đuổi về. | Khi không có người thật ở đó (Remote clinic). | Vi phạm pháp luật y tế nghiêm trọng, nguy hiểm tính mạng. | Tuyệt đối không chọn. |

**Mức chọn: Workflow.**
*Vì sao:* 
- Lấy thông tin đầu vào là giao tiếp ngôn ngữ tự nhiên (cần LLM).
- Output trả ra cần định dạng cố định (Rule/JSON) để đẩy vào màn hình điều dưỡng.
- Con người (Điều dưỡng) là chốt chặn cuối cùng kiểm tra thông tin và ra quyết định y khoa.

## Problem Statement v1

| *Field* | *Nội dung* |
| :--- | :--- |
| *Actor* | Điều dưỡng trực phân loại (Triage Nurse). |
| *Workflow* | Khai báo triệu chứng bằng AI → ĐD review màn hình → ĐD đo sinh hiệu → ĐD chốt phân loại. |
| *Bottleneck* | Bước điều dưỡng dịch lời kể miên man của bệnh nhân thành hồ sơ y tế tốn 5-7 phút. |
| *Impact* | Gây ùn tắc cục bộ, nguy cơ bỏ sót bệnh nhân nặng, burnout cho nhân viên. |
| *Success Metric* | Giảm thời gian tương tác tại quầy xuống < 3 phút/người; 90% draft của AI được Điều dưỡng giữ lại mà không phải gõ lại toàn bộ. |
| *Boundary* | AI nghiêm cấm đưa ra bất kỳ lời khuyên y tế, chẩn đoán hay kê đơn nào cho bệnh nhân. |
| *AI intervention point* | Giữa lúc bệnh nhân bốc số chờ và trước khi bệnh nhân bước vào quầy điều dưỡng. |
| *Mức chọn* | Workflow: LLM extract entities (Triệu chứng, Thời gian, Mức độ đau) → Generate JSON → Hiển thị giao diện cho ĐD. |
| *Rủi ro & người thật* | Risk: Bỏ sót triệu chứng quan trọng. Human-in-the-loop: Điều dưỡng đọc tóm tắt, luôn hỏi xác nhận lại 1 câu: *"Bác có đau ngực hay khó thở không?"* trước khi chốt. |

## Final decision

**Decision:**
Chạy Pilot với scope an toàn nhất.

**Pilot nhỏ nhất:**
- Áp dụng ở quầy **Khám bệnh thông thường** (chưa đưa vào Cấp cứu khẩn cấp - Red Zone).
- Làm một Chatbot/Webform đơn giản để giả lập Kiosk: Bệnh nhân giả định nhập triệu chứng bằng giọng nói/text.
- AI chạy Prompt trích xuất ra format: `[Lý do chính] - [Thời gian khởi phát] - [Triệu chứng đi kèm] - [Bệnh nền]`.
- Mời 1-2 bạn có background y tế (hoặc đóng vai Điều dưỡng) đo thời gian đọc form này so với việc tự hỏi 5 câu hỏi.

**Exit / rollback:**
- Nếu AI liên tục bịa ra triệu chứng bệnh nhân không hề nói (Hallucination) > 10% số ca, ngừng dùng LLM và lùi về phương án Checkbox truyền thống (Rule-based).
- Nếu bệnh nhân mất quá 5 phút để xài bot vì prompt hỏi lại quá nhiều, giới hạn bot chỉ được hỏi tối đa 3 lượt.

**Decision rationale:**
- Giải quyết đúng điểm nghẽn (bottleneck) của sự quá tải: Thu thập thông tin rác.
- Có Human-in-the-loop cực kỳ chặt chẽ (Điều dưỡng).
- Phân định rõ ràng trách nhiệm: AI làm "Thư ký nhập liệu", Điều dưỡng làm "Người ra quyết định chuyên môn".