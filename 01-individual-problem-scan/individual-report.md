# 01 — Individual Problem Scan (Bản Nộp Cá Nhân)

> **Học viên:** Chu Tâm Vũ  
> **Mã học viên:** 2A202601360  
> **Khóa học:** AI20K — VinUni  
> **Ngày cập nhật:** 27/07/2026  

---

## 1. Danh Sách Scan Rộng (10 Candidate Problems)

Nhằm mở rộng góc nhìn phân kỳ cá nhân và đạt mức tối đa tiêu chí đánh giá (scan rộng hơn 5 bài toán), danh sách bên dưới bao gồm 10 vấn đề được quan sát trực tiếp từ công việc học tập, nghiên cứu Deep Learning và vận hành dự án thực tế tại VinUni:

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? (Actor) | Dấu hiệu thật (Tần suất / Thời gian / Log) |
|---|---|---|---|---|
| 1 | **Tốn thời gian & AI Advantage** | Đọc hàng chục file PDF bài báo (arXiv), trích xuất bảng kết quả baseline và nhóm luận điểm để tổng hợp phần *Related Work* trong LaTeX. | Sinh viên / Researcher AI | Tốn 4–6 tiếng/bài báo; đọc 15–20 PDF dài 10–15 trang; trích xuất thủ công các chỉ số baseline (Accuracy, F1, Param size). |
| 2 | **Lặp lại & Tốn thời gian** | Tổng hợp chỉ số huấn luyện mô hình (Loss curve, WandB log, GPU usage) từ nhiều server để viết báo cáo tiến độ tuần gửi Giáo sư hướng dẫn. | Nghiên cứu sinh / Trợ lý nghiên cứu (RA) | 90 phút vào chiều Thứ Sáu hàng tuần; báo cáo trễ làm gián đoạn buổi sync tiến độ với Giáo sư. |
| 3 | **Pain từ người khác** | Khách hàng gửi email phản hồi lỗi ứng dụng bằng văn bản lan man, nhân nhân viên Support phải đọc, tóm tắt và gõ lại ticket Jira chuẩn kèm các bước tái hiện lỗi cho Dev. | Support Specialist, Lead Dev | Tốn 90 phút/ngày (xử lý 40–50 ticket/ngày); Dev phải nhắn tin hỏi lại CS 3–4 lần/ngày do trích xuất thiếu context. |
| 4 | **Tốn thời gian & AI Advantage** | Truy vết lại lý do thay đổi siêu tham số (hyperparameters), cấu hình mô hình hoặc quyết định kỹ thuật cũ bị trôi trong Slack thread / Git commit log. | AI Engineer, Dev Team | Tốn 15–20 phút/lần tra cứu; xuất hiện 3–4 lần/tuần; mất nhiều thời gian hỏi lại đồng đội. |
| 5 | **Lặp lại** | Chuyển đổi thủ công bảng số liệu từ Pandas/Excel sang cú pháp mã `\begin{table}` trong LaTeX và căn chỉnh định dạng lề. | Sinh viên soạn bài báo LaTeX | 30–45 phút/bảng phức tạp; hay bị lỗi biên dịch lề hoặc tràn bảng ra ngoài trang PDF. |
| 6 | **Lặp lại** | Soạn báo cáo công việc hàng ngày (Daily Standup Update) theo đúng định dạng `Done / Today / Blocker` để gửi vào kênh Slack dự án. | Thành viên team dev / Sinh viên | Tốn 10 phút/ngày (50 phút/tuần); công việc mang tính thủ công lặp lại nhưng hay bị quên. |
| 7 | **Pain từ người khác** | Review Pull Request (PR) code của bạn cùng nhóm nhưng code thiếu comment giải thích logic và thiếu mô tả kịch bản test thử nghiệm. | Code Reviewer / Team Lead | 45 phút/PR; phải comment qua lại 2-3 lượt trước khi có thể merge code. |
| 8 | **Lặp lại & Pain từ người khác** | Trợ giảng (TA) phải giải đáp lặp đi lặp lại các câu hỏi trùng lặp về deadline, quy chuẩn nộp bài và lỗi môi trường trong kênh Discord môn học. | Trợ giảng (TA), Sinh viên | Tốn 45 phút/ngày; các câu hỏi trùng lặp chiếm hơn 60% tổng lượng tin nhắn trong kênh thảo luận. |
| 9 | **Tốn thời gian** | Phân công và theo dõi tiến độ công việc tuần cho nhóm đồ án 4-5 người từ ghi chú cuộc họp (meeting notes) chưa hoàn chỉnh. | Nhóm trưởng đồ án (Group Lead) | Tốn 60 phút/tuần; một số công việc bị bỏ sót hoặc trùng lặp người thực hiện. |
| 10 | **Tốn thời gian** | Sàng lọc và tóm tắt 30+ hồ sơ ứng viên đăng ký tham gia Câu lạc bộ Tech / Dự án nghiên cứu để chọn shortlist phỏng vấn. | Trưởng ban nhân sự / Project Lead | Tốn 15 phút/CV (~7.5 tiếng/đợt tuyển); đánh giá kỹ năng cứng/mềm dễ bị mang tính chủ quan. |

---

## 2. Đánh Giá & Phân Hạng Top 3 Candidate Problems

Tiêu chí lựa chọn Top 3 bao gồm: Actor rõ ràng, Workflow hiện tại mô tả chính xác được các bước, Bottleneck đo lường được bằng thời gian và có tính khả thi cao khi đánh giá các phương án No AI / Rule / Workflow / Agent trong bài lab:

| Rank | Candidate Problem | Lý do lựa chọn | Điều còn chưa chắc chắn |
|---|---|---|---|
| **#1** | **Đọc & Trích xuất Baseline cho Bài báo LaTeX (Literature Review)** | Workflow minh bạch, chiếm thời gian lớn nhất (~4 tiếng/bài báo), metric thời gian rõ ràng và AI có lợi thế vượt trội trong phân tích văn bản/PDF. | Khả năng kiểm soát hiện tượng hallucination (bịa số liệu) của AI khi đọc các bảng biểu PDF phức tạp. |
| **#2** | **Tổng hợp Weekly Research Progress Report từ Log Thử nghiệm** | Điểm đau thực tế hàng tuần của sinh viên nghiên cứu, workflow lặp lại cố định, chỉ số đầu ra đo bằng tỉ lệ gửi báo cáo đúng hạn. | Khó khăn trong việc tích hợp dữ liệu từ nhiều nguồn công cụ khác nhau (Git, WandB, TensorBoard). |
| **#3** | **Phân loại & Tóm tắt Ticket Hỗ trợ Kỹ thuật cho Team Dev** | Bài toán vận hành thực tế tại doanh nghiệp/dự án tech, dễ dàng so sánh hiệu quả giữa Rule (Form/Regex) và AI Workflow. | Giới hạn về dữ liệu ticket thực tế để thử nghiệm ngay trong phạm vi thời lượng bài lab. |

---

## 3. Problem Card #1 (Chi Tiết) — Đọc & Trích xuất Baseline cho Bài báo LaTeX

### Thẻ Thông Tin Tóm Tắt (Problem Card #1)
```text
┌────────────────────────────────────────────────────────────────────────────┐
│ PROBLEM CARD #1                                                            │
│                                                                            │
│ Problem 1 câu: Người nghiên cứu mất ~4 tiếng đọc lướt 15-20 file PDF       │
│ bài báo để trích xuất bảng số liệu baseline và tổng hợp luận điểm LaTeX.   │
│                                                                            │
│ Ai chịu ảnh hưởng?: Sinh viên / Researcher AI đang viết bài báo LaTeX      │
│                                                                            │
│ Current Workflow:                                                          │
│ 1. Tìm PDF → 2. Đọc lướt Baseline → 3. Gõ bảng số liệu → 4. Soạn Related   │
│ Work → 5. Gõ mã LaTeX & BibTeX → 6. Biên dịch & Kiểm tra                   │
│                                                                            │
│ Điểm nghẽn nhất: Bước 3 & 4 (Trích số liệu & Soạn văn bản so sánh)         │
│                 Thời gian nghẽn: 150 phút/bài báo                          │
│                                                                            │
│ Success Metric: Giảm tổng thời gian từ 240 phút xuống dưới 45 phút;        │
│                Đảm bảo mã LaTeX Table & BibTeX chính xác 100%.             │
│                                                                            │
│ Quick Gut: [x] Workflow                                                    │
└────────────────────────────────────────────────────────────────────────────┘
```

### Nội Dung Chi Tiết Problem Card #1

- **Problem 1 câu:**  
  Mỗi khi thực hiện đề tài hoặc viết bài báo khoa học, người nghiên cứu mất từ 3–5 tiếng đọc lướt hàng chục file PDF (arXiv), trích xuất các bảng kết quả baseline và nhóm luận điểm để viết phần *Related Work / Literature Review* bằng mã LaTeX.

- **Actor (Người gặp vấn đề):**  
  Sinh viên / Nghiên cứu sinh AI (chịu trách nhiệm thực hiện tổng quan nghiên cứu và soạn thảo bài báo LaTeX).

- **Thời điểm / Bối cảnh:**  
  Giai đoạn khảo sát tài liệu (Literature Review), chuẩn bị nộp bài báo khoa học (Submission deadline) hoặc khi cần tìm đối chứng baseline cho mô hình mới.

- **Current Workflow (Quy trình hiện tại — 6 bước):**  
  1. Tìm kiếm bài báo liên quan trên arXiv / Google Scholar theo từ khóa. *(20 phút)*  
  2. Tải 15–20 file PDF tài liệu về máy tính. *(10 phút)*  
  3. **[Bottleneck 1]** Đọc lướt từng file PDF để trích xuất thông tin: Tên mô hình, Tập dữ liệu, Chỉ số đánh giá (Accuracy, F1, Loss, Params) và Ưu/Nhược điểm. *(90 phút)*  
  4. Gõ lại bảng so sánh baseline vào Google Sheets / Excel. *(20 phút)*  
  5. **[Bottleneck 2]** Nhóm các phương pháp theo phân loại (CNN vs GNN vs Transformer) và soạn thảo văn bản so sánh trực tiếp vào file `.tex`. *(60 phút)*  
  6. Tra cứu mã BibTeX trên Google Scholar và chèn thủ công các thẻ `\cite{...}` cùng bảng `\begin{table}` vào mã nguồn LaTeX. *(40 phút)*  

- **Bottleneck (Điểm nghẽn chính):**  
  **Bước 3 & Bước 5** tốn tổng cộng **150 phút**. Việc đọc quét hàng trăm trang văn bản chỉ để rút ra một vài dòng chỉ số gây tiêu tốn năng lượng trí óc lớn; công đoạn viết lại bằng cú pháp LaTeX dễ gây xao lãng công việc nghiên cứu chính.

- **Impact (Tác động):**  
  - Tiêu tốn **4–6 tiếng/tuần** cho các tác vụ tổng hợp tài liệu thụ động.  
  - Nguy cơ bỏ sót các công trình baseline quan trọng mới xuất bản.  
  - Kéo dài thời gian hoàn thiện bản thảo (draft paper) gửi Giáo sư / Hội nghị.

- **Success Metric (Chỉ số thành công):**  
  - Giảm tổng thời gian xử lý 10 bài báo từ **240 phút xuống dưới 45 phút**.  
  - Mã LaTeX Table và BibTeX được tạo tự động chuẩn xác 100%, biên dịch không lỗi syntax.

- **Non-AI Alternative (Phương án không dùng AI):**  
  Sử dụng phần mềm quản lý trích dẫn Zotero / Mendeley kết hợp Google Sheets template.  
  *Đánh giá hạn chế:* Zotero chỉ hỗ trợ lưu trữ file và xuất BibTeX, không có khả năng tự động đọc nội dung PDF để trích xuất bảng số liệu baseline hoặc tự động nhóm luận điểm so sánh.

- **AI Hypothesis (Giả thuyết ứng dụng AI):**  
  Sử dụng AI Workflow (LLM + PDF Parser) tự động trích xuất các chỉ số baseline ra bảng LaTeX Table, đồng thời đề xuất dàn ý đoạn văn Related Work có gắn sẵn mã `\cite{}`. Người nghiên cứu giữ vai trò kiểm chứng (Human-in-the-loop).

- **Quick Gut:**  
  `[x] Workflow` (Quy trình phối hợp nhiều bước: Parse PDF → Extract Table → Generate Draft → Human Review).

---

### Sơ Đồ Quy Trình (Draft Workflows)

#### 1. Current State (Hiện tại — 240 phút)
```text
[1. Tìm & Tải 15-20 PDF: 30']
  │
  ▼
🔴 [2. NGHẼN 1: Đọc quét PDF trích xuất Baseline Metrics: 90']
  │
  ▼
[3. Gõ bảng số liệu vào Excel/Sheets: 20']
  │
  ▼
🔴 [4. NGHẼN 2: Soạn thảo nội dung Related Work & phân loại: 60']
  │
  ▼
[5. Gõ mã LaTeX Table & chèn thẻ \cite{}: 40']
```

#### 2. Future State (Sau khi áp dụng AI Workflow — 43 phút)
```text
[1. Cung cấp danh sách link arXiv / file PDF: 3']
  │
  ▼
🟢 [2. AI Parser: Trích xuất Baseline Table ra mã LaTeX: 5']
  │
  ▼
🟢 [3. AI Synthesizer: Gợi ý khung Related Work kèm mã \cite{}: 5']
  │
  ▼
👤 [4. Human Boundary: Đối chiếu & Kiểm chứng số liệu gốc từ PDF: 25']
  │
  ▼
[5. Copy vào Editor (Overleaf/VSCode) & Biên dịch: 5']

Fallback Strategy: Nếu AI trích xuất sai chỉ số trong bảng → Người dùng mở file PDF tương ứng và đè số liệu đúng trực tiếp trên bảng LaTeX.
```

---

## 4. Tóm Tắt Problem Cards #2 & #3

| Card | Actor | Bottleneck | Metric | Quick gut | Lý do chưa chọn làm Candidate #1 |
|---|---|---|---|---|---|
| **#2 — Weekly Research Progress Report** | Sinh viên / RA nghiên cứu AI | Viết đoạn văn nhận định (narrative) từ log thô (WandB/Git) mất 35 phút. | 90 phút → 25 phút/tuần; 100% nộp đúng hạn. | Workflow | Dữ liệu nguồn (WandB, TensorBoard, Git) có cấu trúc phức tạp và phân tán hơn. |
| **#3 — Support Ticket Triage cho Dev** | Customer Support Specialist | Đọc email lan man và tóm tắt thành ticket Jira chuẩn mất 45 phút. | 90 phút → 25 phút/ngày; giảm tỉ lệ hỏi lại < 5%. | Rule / Workflow | Hạn chế về nguồn dữ liệu ticket thực tế để thử nghiệm trực tiếp trong thời lượng lab. |

---

## 5. Đề Xuất Candidate Để Pitch Với Nhóm

- **Candidate lựa chọn pitch:** **Problem Card #1 — Đọc & Trích xuất Baseline cho Bài báo LaTeX**.
- **Lý do lựa chọn:**  
  1. Đây là điểm đau phổ biến và cấp thiết đối với tất cả thành viên trong nhóm làm nghiên cứu / đồ án AI.  
  2. Workflow hiện tại phân định rõ ràng các bước và có chỉ số đo lường thời gian thực tế (240 phút).  
  3. Tính khả thi cao khi kiểm chứng giải pháp AI Workflow ngay trong thời lượng bài lab.  

- **Các câu hỏi chuẩn bị để nhóm Challenge:**  
  1. *"Làm thế nào để thiết kế bước Human Review tối ưu nhất nhằm phát hiện nhanh hiện tượng hallucination (bịa số liệu) của AI khi đọc bảng PDF?"*  
  2. *"Nếu kết hợp Zotero với một Notion Template chuẩn hóa (No-AI), chúng ta đã giải quyết được bao nhiêu % điểm nghẽn này so với việc dùng AI?"*  
