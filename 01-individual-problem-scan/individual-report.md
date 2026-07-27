# 01 — Individual Problem Scan

> **Học viên:** Chu Tâm Vũ  
> **Mã học viên:** 2A202601360  
> **Khóa học:** AI20K — VinUni  
> **Ngày cập nhật:** 27/07/2026  

---

## 1. Danh Sách Scan Rộng (10 Candidate Problems)

Nhằm mở rộng góc nhìn phân kỳ cá nhân và đạt mức tối đa tiêu chí đánh giá (scan rộng hơn 5 bài toán), danh sách bên dưới bao gồm 10 vấn đề được quan sát trực tiếp từ công việc học tập, nghiên cứu Deep Learning và vận hành dự án thực tế tại VinUni:

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? (Actor) | Dấu hiệu thật (Tần suất / Thời gian / Log) |
|---|---|---|---|---|
| 1 | **Tốn thời gian & AI Advantage** | Đọc hàng chục file PDF bài báo (arXiv), trích xuất bảng kết quả baseline và nhóm luận điểm để tổng hợp phần Related Work trong LaTeX. | Sinh viên / Researcher AI | Tốn 4–6 tiếng/bài báo; đọc 15–20 PDF dài 10–15 trang; trích xuất thủ công các chỉ số baseline (Accuracy, F1, Param size). |
| 2 | **Lặp lại & Tốn thời gian** | Tổng hợp chỉ số huấn luyện mô hình (Loss curve, WandB log, GPU usage) từ nhiều server để viết báo cáo tiến độ tuần gửi Giáo sư hướng dẫn. | Nghiên cứu sinh / Trợ lý nghiên cứu (RA) | 90 phút vào chiều Thứ Sáu hàng tuần; báo cáo trễ làm gián đoạn buổi sync tiến độ với Giáo sư. |
| 3 | **Pain từ người khác** | Khách hàng gửi email phản hồi lỗi ứng dụng bằng văn bản lan man, nhân viên Support phải đọc, tóm tắt và gõ lại ticket Jira chuẩn kèm các bước tái hiện lỗi cho Dev. | Support Specialist, Lead Dev | Tốn 90 phút/ngày (xử lý 40–50 ticket/ngày); Dev phải nhắn tin hỏi lại CS 3–4 lần/ngày do trích xuất thiếu context. |
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

## 3. Chi Tiết Top 3 Problem Cards & Draft Workflows (Phase 2)

---

### PROBLEM CARD #1 — Đọc & Trích xuất Baseline cho Bài báo LaTeX

#### Thẻ Thông Tin Tóm Tắt (Card #1)
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

#### Nội Dung Chi Tiết (Card #1)
- **Problem 1 câu:** Mỗi khi thực hiện đề tài hoặc viết bài báo khoa học, người nghiên cứu mất từ 3–5 tiếng đọc lướt hàng chục file PDF (arXiv), trích xuất các bảng kết quả baseline và nhóm luận điểm để viết phần Related Work / Literature Review bằng mã LaTeX.
- **Actor:** Sinh viên / Nghiên cứu sinh AI (chịu trách nhiệm tổng quan nghiên cứu và soạn thảo bài báo LaTeX).
- **Thời điểm / Bối cảnh:** Giai đoạn khảo sát tài liệu (Literature Review), chuẩn bị nộp bài báo khoa học (Submission deadline) hoặc khi cần tìm đối chứng baseline cho mô hình mới.
- **Current Workflow (6 bước):**  
  1. Tìm kiếm bài báo liên quan trên arXiv / Google Scholar theo từ khóa. *(20 phút)*  
  2. Tải 15–20 file PDF tài liệu về máy tính. *(10 phút)*  
  3. **[Bottleneck 1]** Đọc lướt từng file PDF để trích xuất thông tin: Tên mô hình, Tập dữ liệu, Chỉ số đánh giá (Accuracy, F1, Loss, Params) và Ưu/Nhược điểm. *(90 phút)*  
  4. Gõ lại bảng so sánh baseline vào Google Sheets / Excel. *(20 phút)*  
  5. **[Bottleneck 2]** Nhóm các phương pháp theo phân loại (CNN vs GNN vs Transformer) và soạn thảo văn bản so sánh trực tiếp vào file `.tex`. *(60 phút)*  
  6. Tra cứu mã BibTeX trên Google Scholar và chèn thủ công các thẻ `\cite{...}` cùng bảng `\begin{table}` vào mã nguồn LaTeX. *(40 phút)*  
- **Bottleneck:** Bước 3 & Bước 5 tốn tổng cộng **150 phút**. Đọc quét hàng trăm trang PDF tiêu tốn năng lượng trí óc lớn; công đoạn viết lại bằng cú pháp LaTeX dễ gây xao lãng công việc nghiên cứu chính.
- **Impact:** Tiêu tốn **4–6 tiếng/tuần** cho các tác vụ tổng hợp tài liệu thụ động; nguy cơ bỏ sót các công trình baseline mới xuất bản; kéo dài thời gian hoàn thiện bản thảo (draft paper).
- **Success Metric:** Giảm tổng thời gian xử lý 10 bài báo từ **240 phút xuống dưới 45 phút**; mã LaTeX Table và BibTeX tạo tự động chuẩn xác 100%, biên dịch không lỗi syntax.
- **Non-AI Alternative:** Sử dụng Zotero / Mendeley kết hợp Google Sheets template. *(Hạn chế: Zotero chỉ lưu trữ file và xuất BibTeX, không có khả năng tự động đọc PDF trích xuất bảng số liệu hay tổng hợp luận điểm so sánh).*
- **AI Hypothesis:** AI Workflow (LLM + PDF Parser) tự động trích xuất các chỉ số baseline ra bảng LaTeX Table, đồng thời đề xuất dàn ý đoạn văn Related Work có gắn sẵn mã `\cite{}`. Người nghiên cứu giữ vai trò kiểm chứng (Human-in-the-loop).
- **Quick Gut:** `[x] Workflow`

#### Sơ Đồ Quy Trình (Draft Workflows Card #1)

##### 1. Current State (Hiện tại — 240 phút)
```text
[1. Tìm & Tải 15-20 PDF: 30']
  │
  ▼
[BOTTLENECK 1] [2. Đọc quét PDF trích xuất Baseline Metrics: 90']
  │
  ▼
[3. Gõ bảng số liệu vào Excel/Sheets: 20']
  │
  ▼
[BOTTLENECK 2] [4. Soạn thảo nội dung Related Work & phân loại: 60']
  │
  ▼
[5. Gõ mã LaTeX Table & chèn thẻ \cite{}: 40']
```

##### 2. Future State (Sau khi áp dụng AI Workflow — 43 phút)
```text
[1. Cung cấp danh sách link arXiv / file PDF: 3']
  │
  ▼
[AI STEP] [2. AI Parser: Trích xuất Baseline Table ra mã LaTeX: 5']
  │
  ▼
[AI STEP] [3. AI Synthesizer: Gợi ý khung Related Work kèm mã \cite{}: 5']
  │
  ▼
[HUMAN BOUNDARY] [4. Đối chiếu & Kiểm chứng số liệu gốc từ PDF: 25']
  │
  ▼
[5. Copy vào Editor (Overleaf/VSCode) & Biên dịch: 5']

Fallback Strategy: Nếu AI trích xuất sai chỉ số trong bảng -> Người dùng mở file PDF tương ứng và đè số liệu đúng trực tiếp trên bảng LaTeX.
```

---

### PROBLEM CARD #2 — Tổng hợp Weekly Research Progress Report từ Log Thử nghiệm

#### Thẻ Thông Tin Tóm Tắt (Card #2)
```text
┌────────────────────────────────────────────────────────────────────────────┐
│ PROBLEM CARD #2                                                            │
│                                                                            │
│ Problem 1 câu: Nghiên cứu sinh (RA) mất 90 phút thu thập log thí nghiệm    │
│ (WandB, TensorBoard, Git) để viết báo cáo tiến độ tuần gửi Giáo sư.        │
│                                                                            │
│ Ai chịu ảnh hưởng?: Nghiên cứu sinh / Trợ lý nghiên cứu AI (RA)            │
│                                                                            │
│ Current Workflow:                                                          │
│ 1. SSH Server log → 2. Export WandB → 3. Check Git Commits                 │
│ → 4. Mở Doc Template → 5. Viết nhận định kĩ thuật → 6. Send Mail           │
│                                                                            │
│ Điểm nghẽn nhất: Bước 5 (Tổng hợp số liệu & Viết nhận định narrative)      │
│                 Thời gian nghẽn: 35 phút/lần                               │
│                                                                            │
│ Success Metric: Giảm thời gian tổng hợp từ 90 phút xuống dưới 25 phút;     │
│                100% báo cáo nộp đúng hạn 18h Thứ Sáu.                      │
│                                                                            │
│ Quick Gut: [x] Workflow                                                    │
└────────────────────────────────────────────────────────────────────────────┘
```

#### Nội Dung Chi Tiết (Card #2)
- **Problem 1 câu:** Mỗi chiều Thứ Sáu, Nghiên cứu sinh / RA mất 90 phút thu thập chỉ số thí nghiệm Deep Learning (loss curve, WandB log, GPU usage) từ nhiều server và repo để viết báo cáo tiến độ tuần gửi Giáo sư hướng dẫn.
- **Actor:** Nghiên cứu sinh / Trợ lý nghiên cứu AI (RA).
- **Thời điểm / Bối cảnh:** 16:00 – 17:30 Thứ Sáu hàng tuần, trước buổi họp sync tiến độ tuần với Giáo sư hướng dẫn.
- **Current Workflow (6 bước):**  
  1. Login SSH vào các server GPU chạy thử nghiệm, kiểm tra log terminal và trạng thái `nvidia-smi`. *(15 phút)*  
  2. Mở WandB / TensorBoard dashboard xuất biểu đồ Loss/Accuracy và các chỉ số evaluation. *(15 phút)*  
  3. Mở Git commit log xem tuần này đã điều chỉnh những module / siêu tham số (hyperparameters) nào. *(10 phút)*  
  4. Mở Google Docs / Word template báo cáo tiến độ tuần. *(5 phút)*  
  5. **[Bottleneck]** Tổng hợp các số liệu rải rác và viết phần nhận định (narrative): Phân tích nguyên nhân mô hình hội tụ chậm/lỗi OOM, đánh giá hiệu quả thay đổi kĩ thuật và đề xuất kế hoạch chạy tuần tới. *(35 phút)*  
  6. Self-review, căn chỉnh định dạng hình vẽ biểu đồ và xuất file PDF gửi email cho Giáo sư. *(10 phút)*  
- **Bottleneck:** Bước 5 tốn **35 phút**. Việc xâu chuỗi log thô từ terminal, biểu đồ WandB và mã nguồn Git để viết thành văn bản nhận định kĩ thuật mạch lạc rất dễ gây bí ý tưởng.
- **Impact:** Tốn 90 phút/tuần cho 1 RA (~7.5 tiếng/tuần nếu lab có 5 RA); báo cáo gửi chậm khiến Giáo sư không kịp đọc trước buổi họp sync.
- **Success Metric:** Giảm thời gian tổng hợp báo cáo từ **90 phút xuống dưới 25 phút/tuần**; 100% báo cáo được gửi đúng hạn trước 18:00 Thứ Sáu.
- **Non-AI Alternative:** Tạo template Notion/Google Form cố định tiêu đề. *(Hạn chế: Chỉ hỗ trợ khung cấu trúc, không giúp tự động đọc log thô để sinh câu chữ phân tích).*
- **AI Hypothesis:** AI Workflow đọc dữ liệu thô (WandB summary JSON + Git commit log) để tự động tạo nháp phần nhận định tiến độ & bảng tổng hợp kết quả chạy. RA kiểm tra và bổ sung phân tích chuyên sâu.
- **Quick Gut:** `[x] Workflow`

#### Sơ Đồ Quy Trình (Draft Workflows Card #2)

##### 1. Current State (Hiện tại — 90 phút)
```text
[1. SSH Server Check GPU Log: 15'] 
  │
  ▼
[2. Export WandB/TensorBoard: 15'] 
  │
  ▼
[3. Check Git Commits: 10'] 
  │
  ▼
[4. Mở Doc Template: 5'] 
  │
  ▼
[BOTTLENECK] [5. Viết Narrative & Nhận định kĩ thuật: 35'] 
  │
  ▼
[6. Format & Gửi Email PDF: 10']
```

##### 2. Future State (Sau khi áp dụng AI Workflow — 22 phút)
```text
[1. Export WandB JSON Summary & Git Log: 5'] 
  │
  ▼
[AI STEP] [2. AI Prompting: Tự động tổng hợp Draft Narrative & Table: 2'] 
  │
  ▼
[HUMAN BOUNDARY] [3. RA Review & Bổ sung phân tích kĩ thuật chuyên sâu: 10'] 
  │
  ▼
[4. Export PDF & Gửi Mail cho Giáo sư: 5']

Fallback Strategy: Nếu AI phân tích sai nguyên nhân lỗi mô hình -> RA tự đè lại nhận định kĩ thuật theo log gốc.
```

---

### PROBLEM CARD #3 — Phân loại & Tóm tắt Ticket Hỗ trợ Kỹ thuật cho Team Dev

#### Thẻ Thông Tin Tóm Tắt (Card #3)
```text
┌────────────────────────────────────────────────────────────────────────────┐
│ PROBLEM CARD #3                                                            │
│                                                                            │
│ Problem 1 câu: Nhân viên Support mất 90 phút/ngày đọc email lan man của    │
│ khách hàng, tóm tắt và gõ lại ticket Jira chuẩn kèm các bước tái hiện lỗi. │
│                                                                            │
│ Ai chịu ảnh hưởng?: Support Specialist (CS) & Lead Developer               │
│                                                                            │
│ Current Workflow:                                                          │
│ 1. Mở Mailbox → 2. Đọc email → 3. Tóm tắt lỗi Jira → 4. Đánh Priority      │
│ → 5. Assign Dev → 6. Dev hỏi lại nếu thiếu context                         │
│                                                                            │
│ Điểm nghẽn nhất: Bước 3 & 4 (Trích context & Viết lại ticket chuẩn)        │
│                 Thời gian nghẽn: 45 phút/ngày                              │
│                                                                            │
│ Success Metric: Giảm thời gian xử lý ticket từ 4' xuống 1' (tổng 90' → 25')│
│                Tỉ lệ Dev phải hỏi lại thông tin < 5%.                      │
│                                                                            │
│ Quick Gut: [x] Rule / Workflow                                             │
└────────────────────────────────────────────────────────────────────────────┘
```

#### Nội Dung Chi Tiết (Card #3)
- **Problem 1 câu:** Mỗi ngày nhân viên Support (CS) mất 90 phút đọc từng email/ticket khiếu nại lan man của khách hàng, trích xuất thông tin kỹ thuật và gõ lại ticket Jira chuẩn kèm các bước tái hiện lỗi (Steps to reproduce) cho Dev team.
- **Actor:** Customer Support Specialist (người tiếp nhận) và Lead Developer (người nhận ticket).
- **Thời điểm / Bối cảnh:** Đầu ca làm việc mỗi sáng và rải rác trong ngày khi có ticket khiếu nại mới từ khách hàng gửi về Mailbox/Zendesk.
- **Current Workflow (6 bước):**  
  1. Mở Mailbox / hệ thống ticket nhận 40–50 email khiếu nại mỗi ngày. *(5 phút)*  
  2. Đọc từng email để hiểu vấn đề khách hàng đang gặp phải. *(20 phút)*  
  3. **[Bottleneck 1]** Trích xuất thông tin thiết bị/OS/tài khoản và gõ lại tóm tắt lỗi ngắn gọn kèm các bước tái hiện lỗi (Steps to reproduce) lên Jira. *(35 phút)*  
  4. **[Bottleneck 2]** Đánh giá mức độ ưu tiên (Low / Medium / High / Critical) theo cảm tính cá nhân. *(10 phút)*  
  5. Gán (Assign) ticket cho đúng team Dev phụ trách (Frontend / Backend / Payment). *(5 phút)*  
  6. Dev đọc ticket; nếu thông tin mập mờ, Dev phải nhắn tin phản hồi lại CS để xác minh. *(15 phút)*  
- **Bottleneck:** Bước 3 & 4 tốn **45 phút/ngày**. Email của khách thường gõ cảm tính, lan man ("App lỗi không ấn được"), CS mất nhiều thời gian đọc hiểu và thường trích xuất thiếu context làm Dev phải hỏi lại nhiều lần.
- **Impact:** Tốn 90 phút/ngày cho nhân viên CS; thời gian phản hồi ban đầu (First Response Time) bị trễ 2–4 tiếng; Dev tốn 30 phút/ngày nhắn tin trao đổi lại với CS.
- **Success Metric:** Giảm thời gian xử lý 1 ticket từ **4 phút xuống 1 phút** (tổng thời gian phân loại giảm từ 90 phút xuống dưới 25 phút/ngày); tỉ lệ Dev phải hỏi lại thông tin giảm từ 30% xuống dưới 5%.
- **Non-AI Alternative:** Yêu cầu khách hàng điền Form mẫu cố định (Dropdown loại lỗi). *(Hạn chế: Khách hàng thường chọn bừa mức ưu tiên hoặc vẫn mô tả lan man trong ô nhập tự do).*
- **AI Hypothesis:** AI đọc nội dung email, tự động trích xuất metadata (OS, thiết bị, mã lỗi), tạo nháp Jira Summary + Steps to reproduce và đề xuất mức độ ưu tiên. CS kiểm tra nhanh và chốt ticket.
- **Quick Gut:** `[x] Rule / Workflow`

#### Sơ Đồ Quy Trình (Draft Workflows Card #3)

##### 1. Current State (Hiện tại — 90 phút/ngày)
```text
[1. Mở Mailbox: 5'] 
  │
  ▼
[2. Đọc email khách hàng: 20'] 
  │
  ▼
[BOTTLENECK] [3 & 4. Tóm tắt lỗi + Trích context + Đánh priority lên Jira: 45'] 
  │
  ▼
[5. Gán cho team Dev: 5'] 
  │
  ▼
[BOTTLENECK] [6. Dev nhắn hỏi lại CS do thiếu thông tin: 15']
```

##### 2. Future State (Sau khi áp dụng AI Workflow — 23 phút/ngày)
```text
[1. Tiếp nhận Email/Ticket: 0'] 
  │
  ▼
[AI STEP] [2. AI Parser: Đọc email, trích metadata + Draft Jira Summary & Priority: 3'] 
  │
  ▼
[HUMAN BOUNDARY] [3. CS Review & Chỉnh sửa nhanh (1' / ticket): 17'] 
  │
  ▼
[4. Auto Sync sang Jira & Notify Dev: 3']

Fallback Strategy: Nếu AI phân loại sai loại lỗi -> CS bấm dropdown chỉnh lại tag trên giao diện review trước khi sync.
```

---

## 4. Chọn Candidate Ưu Tiên Để Pitch & Câu Hỏi Phản Biện

### Candidate Lựa Chọn Pitch
Problem Card #1: Đọc & Trích xuất Baseline cho Bài báo LaTeX (Literature Review).

### Lý Do Lựa Chọn
1. Tính cấp thiết & Đồng cảm cao: Đây là điểm đau trực tiếp và kéo dài của tất cả sinh viên/nghiên cứu sinh đang học tập và làm đồ án/bài báo khoa học tại VinUni.
2. Workflow minh bạch & Đo lường rõ: Quy trình 6 bước có điểm nghẽn tiêu tốn thời gian rất lớn (~240 phút/bài báo), dễ dàng thấy rõ hiệu quả cắt giảm sau khi tối ưu.
3. Mô hình AI phù hợp: Tận dụng đúng thế mạnh của AI trong xử lý ngôn ngữ tự nhiên và đọc trích xuất dữ liệu từ file PDF.

### Các Câu Hỏi Nhờ Nhóm Phản Biện (Challenge Questions)
1. "Hiện tượng AI hallucination (bịa số liệu) ở bài toán này sẽ gây hậu quả gì nghiêm trọng cho bài báo, và bước Human Review 25 phút đã đủ an toàn để kiểm soát rủi ro này chưa?"
2. "Nếu nhóm áp dụng giải pháp No-AI (Zotero + Excel Template chuẩn) thì có thể giải quyết được bao nhiêu % thời gian nghẽn so với việc xây dựng một AI Workflow?"
3. "Liệu bài toán này có khả thi để tạo một demo chạy thử ngay trong phạm vi thời lượng 4 tiếng của buổi lab hôm nay không?"
