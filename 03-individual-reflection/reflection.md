# 03 — Individual Reflection (Bài Thu Hoạch Cá Nhân)

> **Học viên:** Chu Tâm Vũ  
> **Mã học viên:** 2A202601360  
> **Khóa học:** AI20K — VinUni  
> **Ngày cập nhật:** 27/07/2026  

---

## 1. Mức Độ Tham Gia Và Đóng Góp Cá Nhân Trong Nhóm

Bảng tự đánh giá mức độ đóng góp cá nhân xuyên suốt 7 Phase hoạt động của buổi lab:

| Hoạt động | Tôi đã làm gì? | Kết quả / Ảnh hưởng tới sản phẩm nhóm |
|---|---|---|
| **Scan cá nhân** | Thực hiện scan rộng 10 bài toán thực tế dựa trên công việc nghiên cứu AI/Deep Learning và vận hành dự án tại VinUni. | Đưa vào ngân hàng bài toán nhóm 3 candidate sắc nét, giúp nhóm có thêm góc nhìn về bài toán trích xuất dữ liệu khoa học. |
| **Pitch Problem Card** | Pitch chi tiết Problem Card #1 (Đọc & Trích xuất Baseline cho Bài báo LaTeX) với workflow 6 bước và thời gian đo lường rõ ràng. | Bài pitch đạt điểm thuyết phục cao và được nhóm đưa vào shortlist top 2 candidate thảo luận cuối cùng. |
| **Challenge bài của bạn khác** | Đặt câu hỏi challenge cho bài toán Slack Search của bạn trong nhóm về rủi ro phân quyền dữ liệu (data access) và scope quá rộng. | Giúp nhóm loại bỏ bài toán Slack Search để tránh nguy cơ gián đoạn bài lab do phạm vi dữ liệu quá mơ hồ. |
| **Gom trùng / Cluster** | Phân loại 12 bài toán của 4 thành viên vào 4 cụm pattern: Báo cáo/Tổng hợp, Tìm kiếm tài liệu, Review/Feedback, và Planning. | Giúp nhóm nhìn ra bức tranh tổng thể, phát hiện pattern chung là hầu hết thành viên đều nghẽn ở khâu tổng hợp thông tin thô. |
| **Chọn candidate problem** | Cùng nhóm thảo luận và chấm điểm matrix 7 tiêu chí để thống nhất chọn bài toán Đọc & Trích xuất Baseline LaTeX làm candidate chính. | Đạt được đồng thuận 100% trong nhóm mà không cần phải bỏ phiếu cảm tính. |
| **Validation / Research** | Đảm nhận việc tra cứu các công cụ đã có trên thị trường như Zotero, Connected Papers, Elicit và ChatPDF. | Chỉ ra cho nhóm thấy các công cụ hiện tại chỉ dừng ở mức tìm file hoặc chat lẻ tẻ, chưa có workflow sinh trực tiếp mã LaTeX Table. |
| **Workflow nhóm** | Chủ trì vẽ sơ đồ Current State (240 phút) và Future State (43 phút) dạng ASCII kèm các điểm ranh giới người-máy (Human Boundary). | Sơ đồ thể hiện rõ bước Human Review bắt buộc để kiểm soát rủi ro hallucination của AI. |
| **Problem Statement** | Tham gia viết và tinh chỉnh Problem Statement v0 thành v1, làm sắc nét chỉ số Success Metric và phạm vi Boundary. | Đảm bảo metric không chỉ đo bằng thời gian (240 phút -> 45 phút) mà còn gắn với độ chính xác của mã LaTeX biên dịch. |
| **Rule / Workflow / Agent** | Lập luận phản đối việc xây dựng Autonomous Agent phức tạp, đề xuất chọn cấp độ AI Workflow kết hợp con người review. | Giúp nhóm hạ cấp độ từ Agent xuống Workflow, tiết kiệm thời gian và tăng tính khả thi cho mô hình triển khai. |
| **Final Decision** | Đóng góp vào bảng đánh giá 6 câu hỏi quyết định và xây dựng kịch bản thử nghiệm nhỏ nhất (Pilot Plan) cho nhóm. | Thống nhất quyết định Go với scope thử nghiệm trên 10 bài báo mẫu thuộc đề tài Deep Learning. |

---

## 2. Nhật Ký Sử Dụng AI Trong Quá Trình Làm Bài

Bảng tổng hợp chi tiết việc ứng dụng AI, điểm hữu ích, điểm AI sai/hời hợt và các điều chỉnh bằng nhận định cá nhân:

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định cá nhân? |
|---|---|---|---|---|
| **Scan cá nhân** | Đặt prompt gợi ý thêm bài toán từ góc nhìn lăng kính AI Advantage. | Gợi ý thêm ý tưởng về việc tìm kiếm câu trả lời cũ trong kênh Discord môn học. | Đề xuất một số ý tưởng chung chung mang tính giải pháp như "Xây trợ lý AI học tập toàn năng". | Loại bỏ toàn bộ các ý tưởng mang tính giải pháp, chỉ giữ lại các vấn đề có actor và điểm nghẽn đo lường được. |
| **Problem Card** | Đóng vai Skeptical PM để phản biện tính khả thi của Problem Card #1. | Chỉ ra điểm yếu trong việc đo lường chất lượng đoạn văn Related Work (khó định lượng). | AI đề xuất chuyển bài toán sang dạng Agent tự động nộp bài báo không cần người duyệt. | Sửa lại Quick Gut về mức Workflow, bổ sung bước Human Review bắt buộc để kiểm tra số liệu gốc. |
| **Workflow** | Nhờ AI chuyển đổi mô tả các bước thành cú pháp sơ đồ ASCII / Mermaid. | Giúp định dạng sơ đồ nhanh chóng, tiết kiệm thời gian vẽ tay. | AI tự ý gộp bước trích xuất số liệu và bước soạn văn bản Related Work làm một. | Tách độc lập thành 2 bước vì đây là 2 điểm nghẽn có bản chất khác nhau (trích xuất chỉ số vs tổng hợp văn phong). |
| **Research** | Tìm kiếm danh sách các sản phẩm thương mại hiện có giải quyết bài toán đọc PDF nghiên cứu. | Liệt kê nhanh các công cụ như Elicit, Consensus, ChatPDF, Zotero. | AI đưa ra một số tuyên bố hời hợt như "tiết kiệm 90% thời gian" mà không có nguồn kiểm chứng. | Loại bỏ các số liệu tiếp thị không căn cứ, chỉ giữ lại tính năng cốt lõi của công cụ để làm baseline so sánh. |
| **Problem Statement** | Kiểm tra độ chặt chẽ của các trường thông tin trong Problem Statement v1. | Nhắc nhở bổ sung trường ranh giới (Boundary) để AI không tự ý sửa các phần khác trong bài báo. | AI gợi ý đưa thêm các metric phức tạp khó đo lường như "độ sáng tạo của bài báo". | Giữ nguyên metric thực tế: thời gian xử lý và tính chính xác của cú pháp biên dịch LaTeX. |
| **Rule / Workflow / Agent** | Hỏi phản biện lý do vì sao không nên chọn cấp độ Agent cho bài toán này. | Đưa ra các lập luận tốt về rủi ro hallucination và chi phí vận hành agent cao. | AI vẫn cố gắng gợi ý tích hợp thêm tính năng tự động tìm bài báo mới trên arXiv hàng ngày. | Cắt bỏ tính năng tự động tìm kiếm, thu hẹp scope đúng vào khâu xử lý danh sách PDF người dùng cung cấp. |
| **Decision** | Gợi ý tiêu chí Exit / Rollback cho kịch bản thử nghiệm Pilot. | Gợi ý ngưỡng thất bại nếu tỉ lệ sửa đổi thủ công vượt quá 50%. | AI đề xuất kịch bản thử nghiệm quá rộng kéo dài nhiều tháng với nhiều team. | Thu hẹp kịch bản Pilot xuống thử nghiệm trên 10 bài báo mẫu trong 2 tuần cho 1 cá nhân. |

---

## 3. Phản Tư Cá Nhân Và Bài Học Rút Ra

### Điều học được khi lắng nghe bài toán từ các thành viên khác
Khi nghe 3 thành viên khác trình bày Top 3 candidate problems của họ, tôi nhận ra rằng những điểm đau trong vận hành (như phân loại ticket support hay tổng hợp báo cáo tiến độ) có cấu trúc điểm nghẽn rất tương đồng với bài toán nghiên cứu của tôi. Tất cả đều gặp khó khăn ở bước chuyển đổi dữ liệu thô (raw data/log/PDF) thành văn bản nhận định có cấu trúc. Việc lắng nghe giúp tôi hiểu rằng một bài toán tốt không nhất thiết phải là một ý tưởng độc lạ, mà là bài toán có workflow hiện tại được mô tả cực kỳ rõ ràng.

### Nhận diện xu hướng Solution-First trong thảo luận nhóm
Nhóm tôi có thời điểm rơi vào bẫy Solution-First ở Phase 3. Ngay khi thành viên trình bày bài toán tìm kiếm quyết định cũ trong Slack, cả nhóm đã hào hứng bàn về việc dùng mô hình RAG hay Fine-tune LLM nào. Nhờ bám sát tiêu chí checklist trong worksheet, tôi đã kéo nhóm quay lại câu hỏi: "Actor thực sự ở đây là ai, họ mất bao nhiêu phút mỗi lần tìm và data access có bị vướng phân quyền không?". Việc quay lại bản chất problem đã giúp nhóm nhận ra bài toán Slack Search có phạm vi rủi ro quá lớn về mặt dữ liệu và quyết định không chọn.

### Thay đổi nhận thức sau khi bị phản biện (Challenge)
Ban đầu, tôi khá tự tin rằng bài toán trích xuất Baseline LaTeX của mình có thể xử lý hoàn toàn tự động bằng AI. Tuy nhiên, khi bạn trong nhóm đặt câu hỏi challenge: "Nếu AI trích xuất sai một chỉ số F1-score trong bảng baseline mà người nghiên cứu đưa thẳng vào bài báo nộp hội nghị thì hậu quả ra sao?", tôi đã nhận ra lỗ hổng lớn trong giả định của mình. Tôi đã thay đổi quan điểm, đồng ý hạ cấp độ giải pháp từ tự động hóa toàn phần xuống cấp độ AI Workflow với ranh giới bắt buộc là con người phải mở PDF đối chiếu số liệu trước khi biên dịch.

### Đóng góp thực sự vào sản phẩm cuối cùng của nhóm
Đóng góp lớn nhất của tôi cho sản phẩm nhóm là việc giữ kỷ luật về mặt logic và con số. Tôi đã trực tiếp xây dựng sơ đồ workflow trước/sau với định lượng thời gian chính xác cho từng bước, đồng thời lập luận giữ vững ranh giới người-máy (Human Boundary). Tôi cũng là người trực tiếp tổng hợp bảng so sánh các giải pháp thương mại để nhóm chứng minh được tính cần thiết của việc xây dựng một giải pháp riêng.

### Điều khó nhất khi hoàn thiện Problem Statement
Ranh giới giữa Success Metric và Boundary là phần khó viết nhất. Ban đầu nhóm tôi thường viết metric rất chung chung như "viết bài báo nhanh hơn và tốt hơn". Phải mất nhiều lần tinh chỉnh, nhóm mới tách bạch được: Metric phải là con số đo lường được (giảm từ 240 phút xuống 45 phút, mã LaTeX biên dịch không lỗi 100%), còn Boundary phải là ranh giới nghiêm ngặt về quyền hạn (AI chỉ sinh nháp văn bản và mã bảng, không được tự động phê duyệt hay nộp file).

### Kế hoạch điều chỉnh nếu thực hiện lại bài lab
Nếu được làm lại từ đầu, tôi sẽ challenge nhóm mạnh mẽ hơn ngay từ Phase 1 về việc thu thập minh chứng thực tế (evidence). Trong bài làm hôm nay, các con số thời gian baseline (như 240 phút hay 90 phút) chủ yếu dựa trên ước tính cá nhân và phỏng vấn nhanh trong nhóm. Nếu có thêm thời gian, tôi sẽ yêu cầu các thành viên ghi lại log thời gian thực tế của 2-3 lần làm việc gần nhất để số liệu đầu vào có độ tin cậy tuyệt đối trước khi xây dựng Problem Statement.

---

## 4. Tự Kiểm Tra Tiêu Chí Hoàn Thành (Checklist)

- [x] [12đ cá nhân] Cá nhân có danh sách scan 10 problems và Top 3 Problem Cards chi tiết.
- [x] [12đ cá nhân] Đã pitch bài toán cá nhân rõ ràng và đặt câu hỏi challenge đúng trọng tâm cho nhóm.
- [x] Nhóm có nhật ký hội tụ từ 12 candidates về 1 candidate problem duy nhất.
- [x] [15đ nhóm] Nhóm có sơ đồ workflow trước/sau thể hiện rõ các điểm nghẽn và ranh giới kiểm soát.
- [x] [20đ nhóm] Nhóm có Problem Statement v0/v1 với chỉ số metric định lượng và boundary cụ thể.
- [x] [15đ nhóm] Nhóm có bảng so sánh chi tiết giữa No AI / Rule / Workflow / Agent.
- [x] [10đ nhóm] Nhóm có quyết định Go / Not Yet / No-Go đi kèm lý do và kịch bản Pilot rõ ràng.
- [x] [10đ cá nhân] Bài reflection cá nhân trình bày rõ vai trò trong nhóm, nhật ký dùng AI, bài học rút ra và kế hoạch cải thiện.
- [x] [6đ cá nhân] Tự giải thích thành thạo mạch logic: Problem -> Workflow -> Metric -> Boundary -> Độ phù hợp AI.
