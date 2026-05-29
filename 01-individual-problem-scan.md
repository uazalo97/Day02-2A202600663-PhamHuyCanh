# 01 — Individual Problem Scan

## Scan Rộng

| #  | Lăng kính | Problem quan sát được                                                     | Ai đang đau? | Dấu hiệu thật                                                                   |
| -- | ----------- | ----------------------------------------------------------------------------- | -------------- | ---------------------------------------------------------------------------------- |
| 1  | Công việc | Tìm đúng người có đúng thẩm quyền, vai trò để hỏi             | Team member    | Mỗi lần cần hỗ trợ đều phải hỏi vòng vòng người nọ người kia       |
| 2  | Công việc | Chọn món / địa điểm đi ăn chung cho team (team lunch)                 | Team member    | Mất thời gian nhất ở khâu quyết định, hay chốt muộn                      |
| 3  | Công việc | Hiểu task từ nhiều tin nhắn / thread (Slack, email, ticket)               | Team member    | Mất thời gian đọc nhiều thread, hay phải hỏi lại để hiểu rõ nhiệm vụ |
| 4  | Công việc | Ghi chép meeting notes thiếu chuẩn/không nhất quán                      | Team member    | Thông tin hay bị thiếu, phải hỏi lại hoặc tự dò lại sau họp             |
| 5  | Công việc | Phân công task không rõ ràng giữa các thành viên                     | Team member    | Task bị trùng hoặc không người nhận trách nhiệm rõ ràng                 |
| 6  | Công việc | Review code / pull request mất nhiều thời gian                             | Team member    | PR bị comment nhiều vòng, chậm merge, blocker cho người khác                |
| 7  | Công việc | Cập nhật trạng thái (status update) không đồng bộ                     | Team member    | Các bản cập nhật mâu thuẫn, cần sync thêm trong meeting                    |
| 8  | Công việc | Tìm lại quyết định / context cũ trong chat hoặc ticket                 | Team member    | Phải dò lại lịch sử chat nhiều lần, mất 10-20 phút                        |
| 9  | Công việc | Thiếu template / checklist chuẩn cho task lặp lại                         | Team member    | Mỗi người làm theo kiểu riêng, dẫn đến sai sót hoặc thiếu bước       |
| 10 | Công việc | Onboarding người mới: thiếu tài liệu ngắn gọn để bắt tay vào làm | Team member    | Người mới mất nhiều thời gian để hiểu workflow, phải hỏi nhiều         |

## Top 3

| Rank | Problem                                                         | Vì sao chọn                                                                                                                                | Điều còn chưa chắc                                                                                      |
| ---- | --------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| 1    | Tìm đúng người có đúng thẩm quyền, vai trò để hỏi | Workflow lặp lại trong công việc team; hay phải hỏi vòng vòng, mất thời gian và có thể đo được số lượt hỏi lại         | Có đủ thường xuyên để làm thành bài lab không, và phạm vi chỉ trong một team hay nhiều team |
| 2    | Chọn món / địa điểm đi ăn chung cho team (team lunch)   | Xảy ra lặp lại trong các hoạt động team, dễ quan sát, có pain rõ ở bước quyết định, phù hợp để vẽ workflow trước/sau | Impact có đủ lớn cho productivity của team không (hay chỉ là bất tiện nhỏ)?                       |
| 3    | Hiểu task từ nhiều tin nhắn / thread (Slack, email, ticket) | Pain rõ khi task lan truyền qua nhiều kênh; tốn thời gian tổng hợp ngữ cảnh và thường phải hỏi lại                           | Có đủ input (thread, ticket) để AI tổng hợp giúp không, và privacy/access có cho phép?           |

## Problem Card #1 — Tìm đúng người để hỏi

**Problem 1 câu:**
Mỗi khi cần hỗ trợ, tôi mất thời gian hỏi vòng vòng để tìm đúng người có đúng thẩm quyền hoặc đúng vai trò.

**Actor:**
Team member (nhân viên trong team).

**Thời điểm / bối cảnh:**
Khi cần hỏi về task nội bộ, quy trình team, quyền truy cập hoặc người phụ trách một công việc trong team.

**Current workflow:**

```text
1. Có câu hỏi hoặc vấn đề cần xử lý
2. Nghĩ xem ai có thể biết
3. Hỏi 1 người đầu tiên
4. Bị chuyển sang người khác hoặc được giới thiệu vòng vòng
5. Hỏi lại đúng người
6. Chờ phản hồi / xác nhận
```

**Bottleneck:**
Bước tìm đúng người để hỏi, vì dễ bị hỏi sai người 1-2 lần trước khi tới đúng owner.

**Impact:**
Mất khoảng 10-15 phút cho mỗi lần hỏi trong trường hợp đơn giản; nếu gặp nhiều lần mỗi tuần thì rất tốn thời gian và làm chậm việc chính.

**Success metric:**
Giảm thời gian tìm đúng người từ 10-15 phút xuống dưới 3 phút, và giảm số lần hỏi vòng vòng.

**Non-AI alternative:**
Org chart, FAQ nội bộ, danh bạ team, hoặc quy ước rõ ai phụ trách việc gì.

**AI hypothesis:**
AI gợi ý đúng người nên hỏi dựa trên mô tả vấn đề, vai trò, hoặc ngữ cảnh task.

**Quick gut:**
Workflow.

## Problem Card #2 — Chọn món / địa điểm đi ăn chung

**Problem 1 câu:**
Mỗi lần đi ăn chung, cả nhóm mất nhiều thời gian để chốt món hoặc địa điểm phù hợp.

**Actor:**
Team member (nhân viên trong team).
Nhóm bạn / nhóm sinh viên.

**Thời điểm / bối cảnh:**
Trước khi đi ăn trưa/ăn trưa nhóm của team, hoặc tổ chức team lunch.

**Current workflow:**

```text
1. Gợi ý vài món hoặc vài quán
2. Mỗi người nêu sở thích riêng
3. So sánh khoảng cách, giá, khẩu vị, giờ mở cửa
4. Bỏ bớt lựa chọn không hợp
5. Vote hoặc chốt theo số đông
6. Nhắn địa điểm cuối cùng cho cả nhóm
```

**Bottleneck:**
Bước quyết định cuối cùng, vì mỗi người có một tiêu chí khác nhau nên hay chốt muộn.

**Impact:**
Mất khoảng 10-20 phút mỗi lần hẹn; nếu nhóm đi ăn thường xuyên thì đây là một pain lặp lại khá rõ.

**Success metric:**
Giảm thời gian chốt từ 10-20 phút xuống dưới 5 phút, và giảm số vòng nhắn qua lại.

**Non-AI alternative:**
Poll nhanh, checklist tiêu chí cố định, hoặc danh sách quán quen đã lọc sẵn.

**AI hypothesis:**
AI shortlist 2-3 lựa chọn phù hợp theo budget, vị trí, và khẩu vị.

**Quick gut:**
Rule / Workflow.

## Problem Card #3 — Hiểu task từ nhiều tin nhắn / thread

**Problem 1 câu:**
Khi task hoặc quyết định lan truyền qua Slack, email và ticket, tôi mất nhiều thời gian để tổng hợp ngữ cảnh và hiểu chính xác phải làm gì.

**Actor:**
Team member (nhân viên trong team).

**Thời điểm / bối cảnh:**
Khi nhận task mới hoặc khi cần hoàn thiện task dựa trên nhiều thread, log, hoặc ticket liên quan.

**Current workflow:**

```text
1. Đọc các message/thread liên quan (Slack, email, ticket)
2. Ghi chú các yêu cầu/ràng buộc rải rác
3. So sánh các thông tin xung đột hoặc thiếu
4. Hỏi lại chủ task/owner để làm rõ
5. Bắt tay vào làm khi rõ ràng
```

**Bottleneck:**
Bước tổng hợp ngữ cảnh từ nhiều nguồn và phát hiện chỗ mâu thuẫn/thiếu thông tin — thường phải hỏi lại chủ task.

**Impact:**
Mất 15–30 phút mỗi lần tổng hợp; chậm deliver hoặc làm sai nếu bỏ qua bước hỏi lại.

**Success metric:**
Giảm thời gian tổng hợp từ 15–30 phút xuống dưới 7 phút, và giảm số lần phải hỏi clarifying question xuống ít hơn 1 lần/một task.

**Non-AI alternative:**
Quy ước ghi chú rõ ràng trong ticket, checklist handoff, hoặc template mô tả task bắt buộc.

**AI hypothesis:**
AI đọc các thread/ticket, tóm tắt key decisions, highlight conflict/thiếu thông tin và trả về checklist rõ ràng để nhân viên hành động.

**Quick gut:**
Workflow.
