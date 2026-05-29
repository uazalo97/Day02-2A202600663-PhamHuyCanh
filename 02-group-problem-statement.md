# 02 — Group Problem Statement

**Nhóm:** Batch 02 — Nhóm 11 Zone B
**Thành viên:** Nguyễn Xuân Tới (2A202600810) · Quân · Tiến Huân · Thắng · Cảnh · Ngọc
**Case được chọn:** Tạo video bài giảng tự động từ tài liệu — EduVid AI
**Ngày hoàn thành:** 2026-05-29

---

## PHASE 3 — Group Convergence (Hội tụ nhóm)

### 3A. Tóm tắt quá trình chọn case

Nhóm thu thập 5 bài quét cá nhân, tổng cộng **30+ bài toán** được liệt kê. Sau vòng đọc nhanh (5 phút/người), nhóm shortlist xuống **5 bài toán ứng viên** đại diện cho các domain: HR, EdTech, trợ giảng, AI & automation consulting, và content marketing.

Nhóm đánh giá theo **4 tiêu chí cứng**:

| Tiêu chí                                                    | Trọng số  |
| ------------------------------------------------------------- | ----------- |
| Pain level — mức độ đau thật của người thật         | Cao         |
| AI-able — có thể giải bằng AI ở mức Workflow trở lên | Cao         |
| Measurable — có metric rõ ràng trước/sau                | Trung bình |
| Scope — làm được trong 4 tiếng demo                     | Trung bình |

Sau 20 phút thảo luận, nhóm thu hẹp xuống **2 ứng viên cuối**: bài của **Thắng** (EduVid) và bài của **Tiến Huân** (nhận xét bài tập học sinh tự động). Cả hai đều có pain rõ và actor cụ thể.

Lý do loại bài Tiến Huân: nhóm xác định bài toán nhận xét bài tập cần AI **tự phân loại loại bài, tự đánh giá độ khó, tự quyết định feedback phù hợp theo từng học sinh** — đây là mức **Agent**, không phải Workflow. Scope quá rộng để demo trong 4 tiếng, và rủi ro cao khi AI nhận xét sai ảnh hưởng trực tiếp đến học sinh.

Nhóm chọn **bài của Thắng** với lý do:

1. **Pain thật và có thể đo được ngay:** Giáo viên mất 2–4 giờ để sản xuất 1 video bài giảng, phải dùng 5–6 tool riêng lẻ. Con số xác nhận được ngay trong buổi học.
2. **Workflow rõ nhất trong nhóm:** Pipeline có điểm đầu (upload tài liệu) và điểm cuối (export video) rõ ràng. Mỗi bước bottleneck đều đo được thời gian.
3. **AI-able ở mức Workflow:** Generate Slides → Teacher Review → Generate Script → Teacher Review → Generate Audio → Teacher Review → Export. Không cần Agent tự quyết định động.
4. **Generalizable và có thị trường rõ:** Hàng triệu giáo viên đang gặp đúng bài toán này. Có tool tương tự để research gap ngay trong buổi.

---

### 3B. Shortlist và điểm số

| # | Bài toán                                | Người đề xuất | Pain (1–5) | AI-able (1–5) | Measurable (1–5) | Scope (1–5) | Tổng        | Ghi chú                                  |
| - | ----------------------------------------- | ------------------ | ----------- | -------------- | ----------------- | ------------ | ------------ | ----------------------------------------- |
| 1 | Tạo video bài giảng từ tài liệu     | Thắng             | 5           | 5              | 5                 | 5            | **20** | ✅ Chọn                                  |
| 2 | Nhận xét bài tập học sinh tự động | Tiến Huân        | 5           | 5              | 4                 | 4            | **18** | ⚠️ Agent-level — loại                 |
| 3 | Lên lịch 30 ngày content tự động    | Nguyễn Xuân Tới | 5           | 5              | 5                 | 4            | **19** | Actor = người đề xuất, khó validate |
| 4 | Sàng lọc CV tự động (HR)             | Quân              | 5           | 4              | 4                 | 4            | **17** | Cần data CV thật để demo              |
| 5 | Phân loại chi tiêu cá nhân           | Cảnh              | 4           | 4              | 4                 | 4            | **16** | Domain hẹp, khó generalize              |

> **Lý do chốt EduVid:** Huân điểm cao (18) nhưng bị loại vì cần Agent-level — quá rộng và rủi ro cao cho scope 4 tiếng. Tới điểm cao (19) nhưng actor là chính người đề xuất, dễ bị confirmation bias khi validate. EduVid của Thắng có workflow rõ nhất, actor là giáo viên (hỏi được ngay trong buổi), demo được bằng 1 file PDF thật.

---

## PHASE 4 — Quick Validation (Kiểm chứng nhanh)

### 4A. Phỏng vấn nhanh (3 người thật)

| Người          | Role                            | Câu hỏi hỏi                                                   | Câu trả lời tóm tắt                                                        |
| ---------------- | ------------------------------- | ---------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| Nguyễn Thị Mai | Giáo viên THPT — Hà Nội    | "Bạn mất bao lâu để làm 1 video bài giảng?"              | "2-3 tiếng, chủ yếu mất ở bước viết script và ghép video."            |
| Trần Văn Hùng | Quản lý trung tâm đào tạo | "Bạn có đang số hóa bài giảng không? Vướng ở đâu?"  | "Có, nhưng chậm vì giáo viên không có thời gian và không quen tool." |
| Lê Thị Hoa     | Giảng viên đại học         | "Nếu có tool tự tạo video từ slide/PDF, bạn dùng không?" | "Dùng ngay — bây giờ mất quá nhiều bước."                              |

**Kết luận validation:** Pain được xác nhận bởi **3/3 người** — đây là vấn đề thật, không phải vấn đề tưởng tượng.

### 4B. Research tool tương tự (Market Scan)

| Tool                   | Làm được gì                     | Không làm được gì                                        | Giá             |
| ---------------------- | ------------------------------------ | -------------------------------------------------------------- | ---------------- |
| **HeyGen**       | Tạo video với AI avatar từ script | Không tự tạo slide, không tự viết script từ tài liệu  | $24–$120/tháng |
| **Synthesia**    | AI avatar đọc script thành video  | Không xử lý tài liệu đầu vào, phải tự soạn script   | $22–$67/tháng  |
| **Descript**     | Edit video bằng text, transcript    | Không tự generate nội dung từ tài liệu                   | $12–$24/tháng  |
| **Gamma.app**    | Tạo slide từ prompt/tài liệu     | Không tạo audio, không xuất video bài giảng hoàn chỉnh | $8–$15/tháng   |
| **Beautiful.ai** | Tạo slide đẹp tự động          | Không có TTS, không có video export                        | $12/tháng       |

**Gap được xác nhận:**

> Chưa có tool nào kết hợp đầy đủ: **nhận tài liệu đầu vào (PDF/DOCX/PPTX) → tự tạo slide → tự viết script phù hợp nội dung → tự tạo audio → xuất video bài giảng hoàn chỉnh** trong một pipeline có điểm review của giáo viên ở từng bước. Các tool hiện tại đều chỉ giải 1–2 bước, không phải toàn bộ workflow.

---

## PHASE 5 — Problem Statement

### 5A. Workflow hiện tại (Before AI)

```
[Giáo viên]
     |
     ▼ Chuẩn bị tài liệu nguồn (PDF / DOCX / PPTX) — có sẵn
     |
     ▼ Dùng ChatGPT/Claude tóm tắt nội dung (15–30 phút)
         — Prompt thủ công từng lần
         — Output không đồng đều tùy cách hỏi
     |
     ▼ Tạo slide trên PowerPoint (30–60 phút)
         — Copy-paste từ output AI hoặc tự làm
         — Format, chọn layout, chọn màu
     |
     ▼ Viết lời giảng (script) cho từng slide (30–90 phút)  ← BOTTLENECK LỚN NHẤT
         — Phải đọc lại tài liệu gốc
         — Viết sao cho tự nhiên khi đọc lên
         — Thường phải viết lại nhiều lần
     |
     ▼ Thu âm hoặc dùng TTS (30–60 phút)
         — Nếu thu âm thật: thu nhiều lần vì nói vấp, tiếng ồn
         — Nếu TTS: phải chọn giọng, điều chỉnh tốc độ, kiểm tra từng đoạn
     |
     ▼ Ghép slide + audio trên Canva hoặc Camtasia (30–60 phút)
         — Sync từng slide với từng đoạn audio
         — Thêm transition, hiệu ứng
         — Export video (mất thêm 10–20 phút render)
     |
     ▼ Kiểm tra và upload lên LMS / YouTube (15–20 phút)

TỔNG THỜI GIAN: 2–4 giờ/video
SỐ TOOL SỬ DỤNG: 5–6 tool riêng lẻ, không kết nối với nhau
```

### 5B. Workflow kỳ vọng (After AI — Workflow Level)

```
[Giáo viên]
     |
     ▼ Upload tài liệu (PDF / DOCX / PPTX) — 2 phút
     |
     ▼ [AI] Generate Script (lời giảng toàn bộ) — auto  ← chốt text TRƯỚC
         — Tự đọc và phân tích nội dung tài liệu
         — Tự viết lời giảng theo cấu trúc logic
         — Tối ưu token: xử lý text một lần thay vì nhiều bước riêng lẻ
     |
     ▼ [Giáo viên] Review Script — 5 phút  ← human boundary #1
         — Chỉnh sửa câu chữ, bổ sung ý nếu cần
         — Approve để tiếp tục
         — Gợi ý: nên có người hỗ trợ bên cạnh ở bước này (đồng nghiệp / trợ giảng)
           để review nhanh hơn và tránh bỏ sót nội dung chuyên môn
     |
     ▼ [AI] Generate Slides từ Script đã duyệt — auto  ← slide sinh SAU text
         — Tự tạo slide dựa trên script đã approve
         — Đảm bảo nội dung slide khớp 100% với lời giảng
         — Tiết kiệm token đáng kể so với generate đồng thời slide + script
     |
     ▼ [Giáo viên] Review Slides — 3 phút  ← human boundary #2
         — Kiểm tra layout, chỉnh sửa nếu cần
         — Approve để tiếp tục
     |
     ▼ [AI] Generate Audio (TTS) — auto
         — Đọc script bằng giọng đã chọn, sync với slide
     |
     ▼ [Giáo viên] Review Audio — 3 phút  ← human boundary #3
         — Nghe nhanh, kiểm tra sync
         — Approve để export
     |
     ▼ [AI] Export Video hoàn chỉnh — auto

TỔNG THỜI GIAN: < 20 phút (3 lần review + wait time AI)
SỐ TOOL: 1 platform duy nhất
LƯU Ý TOKEN: Pipeline "text trước → slide sau" giảm chi phí AI ~40% so với
              generate song song, đồng thời đảm bảo nội dung nhất quán
```

---

### 5C. Problem Statement v0 (Draft ban đầu)

> *Giáo viên mất quá nhiều thời gian làm video bài giảng vì phải dùng nhiều tool khác nhau, cần AI làm thay.*

### 5D. Problem Statement v1 (Final — 7 fields)

| Field                           | Nội dung                                                                                                                                                                                                                              |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Actor**                 | Giáo viên phổ thông, giảng viên đại học, và trung tâm đào tạo muốn số hóa bài giảng thành video để dạy online hoặc lưu trữ                                                                                   |
| **Workflow**              | Chuẩn bị tài liệu → dùng AI tóm tắt thủ công → tạo slide trên PowerPoint → viết script → thu âm hoặc TTS → ghép video trên Canva/Camtasia → upload LMS                                                           |
| **Bottleneck**            | Ba bước đều là bottleneck: tạo slide (30–60'), viết script (30–90'), ghép video (30–60') — tổng 2–4 giờ/video với 5–6 tool không kết nối nhau                                                                      |
| **Impact**                | Giáo viên không có thời gian số hóa bài giảng → khóa học online không được xây dựng → trường/trung tâm thiếu nguồn lực số hóa → cơ hội dạy online bị bỏ lỡ                                           |
| **Success Metric**        | Thời gian/video: 2–4 giờ → dưới 20 phút; Completion Rate: >80% giáo viên hoàn thành video sau khi bắt đầu; Export Success: >95% video export thành công                                                                |
| **Boundary**              | AI không tự publish lên LMS khi chưa được giáo viên approve; không tự thay đổi nội dung chuyên môn; không tự chọn giọng đọc mà không có lựa chọn của giáo viên; giáo viên review ở 3 điểm kiểm tra |
| **AI Intervention Point** | Sau khi giáo viên upload tài liệu → AI xử lý 3 bước nặng (Generate Slides, Generate Script, Generate Audio) → giáo viên review và approve sau mỗi bước trước khi AI tiếp tục                                      |

---

## PHASE 6 — AI Level Selection

### So sánh 3 mức độ AI

| Mức                  | Mô tả                                                                                                   | Áp dụng cho bài toán này                                                                 | Phù hợp?                        |
| --------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------- |
| **Rule-based**  | IF/THEN cứng nhắc. Template slide cố định, giáo viên tự điền nội dung                          | Giảm bước format nhưng không giải quyết việc tạo nội dung                           | ❌ Không giải quyết bottleneck |
| **Workflow AI** | Pipeline tuyến tính: Upload → AI Generate → Teacher Review → AI Generate → Teacher Review → Export | Đúng với cấu trúc bài toán — mỗi bước AI rõ ràng, có điểm review của người | ✅**Phù hợp nhất**       |
| **Agent AI**    | Tự phân tích tài liệu, tự điều chỉnh style, tự quyết định cách trình bày, tự publish     | Quá phức tạp — nội dung giáo dục cần giáo viên kiểm soát chất lượng            | ❌ Rủi ro cao, chưa cần        |

**Kết luận:** Chọn **Workflow AI** vì:

- Pipeline tuyến tính, không cần AI tự quyết định động
- Giáo viên kiểm soát ở 3 điểm (Slides / Script / Audio) — đảm bảo chất lượng chuyên môn
- Có thể demo được trong 4 tiếng với 1 file PDF thật
- Stack khả thi: OpenAI API (text) + TTS API (audio) + pipeline export video

---

## PHASE 7 — Go / Not Yet / No-Go Decision

### Checklist đánh giá

| Câu hỏi                                                           | Trả lời                                                                                                | Kết luận                             |
| ------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------- |
| Có người thật đang gặp bài toán này không?                | ✅ Có — 3/3 người phỏng vấn xác nhận mất 2–3 giờ/video                                        | Go                                     |
| AI có thể làm tốt hơn con người ở bước bottleneck không? | ✅ Có — LLM generate slide/script nhanh hơn và nhất quán hơn                                      | Go                                     |
| Có thể đo được kết quả trước/sau không?                  | ✅ Có — thời gian/video, completion rate, export success                                              | Go                                     |
| Có tool tương tự chứng minh thị trường không?              | ✅ Có — HeyGen, Synthesia, Gamma. Gap ở tích hợp end-to-end                                         | Go                                     |
| Scope có fit 4 tiếng không?                                      | ✅ Có — prototype với 1 tài liệu thật, 1 pipeline, bỏ qua polish UI                               | Go                                     |
| Rủi ro nào cần chú ý?                                          | ⚠️ Chất lượng script AI có thể không đúng ngữ điệu giảng dạy → xử lý bằng review step | Not Yet → đã xử lý bằng boundary |

### Quyết định: ✅ **GO — với
