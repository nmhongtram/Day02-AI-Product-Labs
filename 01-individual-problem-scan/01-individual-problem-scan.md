# 01 — Individual Problem Scan

## Scan rộng

| #  | Lăng kính          | Problem quan sát được                                                          | Ai đang đau?              | Dấu hiệu thật                          |
| -- | ------------------ | ------------------------------------------------------------------------------ | ------------------------- | -------------------------------------- |
| 1  | AI có thể tốt hơn  | Team meeting trao đổi nhiều topic liên tục nên dễ miss decision và action item | Team project AI, học viên | Sau meeting phải hỏi lại task/deadline |
| 2  | Lặp lại            | Review chat dài để tìm “quyết định cuối cùng” hoặc link quan trọng             | Học viên, team member     | Mất 10-30 phút/search                  |
| 3  | AI có thể tốt hơn  | Tài liệu, recording, assignment và lịch học nằm rải rác nhiều kênh             | Học viên khóa AI          | Thường hỏi lại “link ở đâu?”           |
| 4  | Pain từ người khác | Lịch học hoặc deadline cập nhật sát giờ nhưng notification phân tán            | Học viên                  | Miss class/link/deadline               |
| 5  | Tốn thời gian      | Customize CV/project description theo từng job AI/Data                         | Sinh viên mới tốt nghiệp  | 20-40 phút/job                         |
| 6  | Tốn thời gian      | Đọc research paper để hiểu methodology và contribution                         | Research student          | 1-2 giờ/paper                          |
| 7  | Lặp lại            | Viết weekly internship/project progress report từ task log                     | Intern, research student  | 45-60 phút/tuần                        |
| 8  | Pain từ người khác | Mentor/TA phải trả lời cùng một câu hỏi nhiều lần                              | Mentor, TA                | FAQ lặp đi lặp lại                     |
| 9  | Tốn thời gian      | Tìm trọ ngắn hạn phù hợp ngân sách và khoảng cách học                          | Học viên                  | Search nhiều nhóm/Facebook             |
| 10 | AI có thể tốt hơn  | Đọc và hiểu hợp đồng trọ ngắn hạn để tránh mất cọc hoặc phí ẩn                 | Học viên                  | Không chắc điều khoản/phạt             |



## Top 3

| Rank | Problem                                   | Vì sao chọn                                                             | Điều còn chưa chắc                    |
| ---- | ----------------------------------------- | ----------------------------------------------------------------------- | ------------------------------------- |
| 1    | Meeting/team discussion bị miss thông tin | Pain thật trong teamwork, AI phù hợp để summarize + extract action item | Accuracy khi nhiều người nói cùng lúc |
| 2    | Unified search cho tài liệu/lịch/link     | Workflow hằng ngày, impact rộng cho học viên/team                       | Data integration nhiều nguồn          |
| 3    | Customize CV cho từng job AI/Data         | Scope rõ, metric dễ đo, sát nhu cầu cá nhân                             | Quality/relevance với recruiter       |


## Problem Card #1 - Meeting/team discussion bị miss thông tin

**Problem 1 câu:**
Trong các buổi meeting hoặc thảo luận team dự án AI, nhiều vấn đề được trao đổi liên tục nên thành viên dễ bỏ sót decision, action item hoặc deadline quan trọng.

**Actor:**  
Sinh viên/học viên tham gia team project AI hoặc research project từ 3-6 người.

**Thời điểm / bối cảnh:**  
Trong meeting online/offline, đặc biệt khi team brainstorm technical issue, chia task hoặc update progress.

**Current workflow:**

1. Team họp qua Discord/Google Meet
2. Nhiều người trao đổi liên tục
3. Một người note thủ công
4. Sau meeting team đọc lại chat/note
5. Thành viên tự nhớ task của mình
6. Hỏi lại nếu quên decision/deadline

**Bottleneck:**
Bước 3-5 — note thủ công thường thiếu thông tin, không capture đầy đủ action item và decision cuối cùng.

**Impact:**

Miss task hoặc deadline.
Phải hỏi lại nhiều lần trong chat.
Tốn thời gian đọc lại conversation dài.
Team alignment kém hơn.

**Success metric:**

Giảm số lần hỏi lại task/deadline sau meeting.
Giảm thời gian đọc lại meeting/chat log.
Tăng tỷ lệ action item được follow đúng hạn.

**Non-AI alternative:**
Dùng template meeting note hoặc phân công một người làm thư ký.

**AI hypothesis:**
AI có thể transcribe/summarize meeting, extract decision/action item/deadline và gửi structured recap sau meeting.

**Quick gut:**
Agent.

### Draft current workflow

```text
CURRENT STATE — 45 phút + follow-up confusion

[1 Team discussion]
→ [2 Manual note-taking]
→ [3 Đọc lại chat/note]
→ [4 Tự nhớ task]
→ [5 Hỏi lại trong chat]  <-- bottleneck
→ [6 Re-align task/deadline]
```

### Draft future workflow

```text
FUTURE STATE — 10 phút review

[1 Record meeting/chat]
→ [2 AI summarize discussion]
→ [3 AI extract action item + owner + deadline]
→ [4 Team review/edit summary]  <-- human boundary
→ [5 Auto-share structured recap]

Fallback: AI hiểu sai speaker/task → team edit manually.
```

## Problem Cards #2 và #3 — tóm tắt

| Card                                  | Actor                    | Bottleneck                                        | Metric                       | Quick gut        | Vì sao chưa chọn làm #1            |
| ------------------------------------- | ------------------------ | ------------------------------------------------- | ---------------------------- | ---------------- | ---------------------------------- |
| Unified search cho tài liệu/lịch/link | Học viên, team member    | Search tài liệu/link/lịch từ nhiều nguồn phân tán | 15 phút → dưới 3 phút/search | Agent / Workflow | Scope và data integration khá rộng |
| Customize CV cho từng job AI/Data     | Sinh viên mới tốt nghiệp | Rewrite project description theo từng JD          | 30 phút → dưới 10 phút/job   | Workflow         | Impact hẹp hơn teamwork workflow   |
---
---