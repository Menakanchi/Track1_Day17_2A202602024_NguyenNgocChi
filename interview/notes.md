# Interview Script — Case C: AI Support Radar (Lab Coach)

## Thông tin interview

- **Interviewer:** Thành viên nhóm
- **Interviewer:** Lab Coach (Hỗ trợ kỹ thuật / Vận hành lớp học)
- **Kênh hỗ trợ được nhắc đến:** Trực tiếp tại phòng lab & Kênh Discord
- **Case:** Case C — AI Support Radar
- **Mục đích:** Tìm hiểu cách Lab Coach phát hiện học viên bị kẹt, cách sắp xếp thứ tự ưu tiên xử lý và cách khai thác ngữ cảnh (context) của câu hỏi trong thực tế.
- **Ghi âm:** Chỉ thực hiện sau khi interviewer đồng ý.

> **Lưu ý:** Giữ nguyên tắc The Mom Test, không giới thiệu trước về tính năng AI Support Radar hay bảng Support Queue tự động để tránh nhận về các câu trả lời mang tính phỏng đoán tương lai.

---

## Transcript

### Mở đầu

**Interviewer:**

Chào chị, nhóm em đang tìm hiểu về cách đội ngũ Lab Coach theo dõi và hỗ trợ học viên trong quá trình học và làm bài lab thực tế. Tụi em muốn lắng nghe những trải nghiệm, tình huống cụ thể đã diễn ra trong các buổi học vừa qua. Không có câu trả lời đúng hay sai và tụi em cũng không đánh giá quy trình làm việc; chị cứ chia sẻ thật những gì diễn ra nhé.

---

### Câu hỏi 1 — Nhận diện điểm kẹt & Thời gian phát hiện (Detection & Time-to-detect)

**Interviewer:**

Trong buổi học gần nhất, chị có thể kể lại trường hợp một bạn học viên gặp lỗi hoặc bị kẹt bài mà chị đã hỗ trợ? Lúc đó từ đâu mà chị biết bạn ấy đang gặp khó khăn, và từ thời điểm bạn ấy bị tắc đến khi chị nhận ra là mất khoảng bao lâu?

**Interviewee — Lab Coach:**

Nếu học viên không có dấu hiệu gì để nhận ra thì phần lớn bọn mình phải đoán thôi bạn ạ. Một là đoán, hai là trực tiếp đi lại quanh lớp. Ví dụ đến đoạn đáng lẽ phải cài đặt xong môi trường rồi, bọn mình đi qua nhìn lướt vào terminal thấy bạn ấy vẫn đang kẹt, màn hình đang dừng lại là bọn mình sẽ chủ động hỏi luôn. Còn nếu các bạn không tự giác hỏi thì bọn mình phải lại từng bàn để hỏi xem có ai đang gặp vấn đề gì không. 

Nhiều bạn có tâm lý ngại giơ tay hoặc do tính cách không muốn chủ động reach out đến Lab Coach, mà hay quay sang hỏi AI hoặc hỏi bạn bè xung quanh trước.

---

### Câu hỏi 2 — Phân loại & Ưu tiên hỗ trợ (Prioritization / Triage)

**Interviewer:**

Kể lại lần gần nhất có nhiều bạn học viên cùng giơ tay hoặc gửi câu hỏi dồn dập cùng lúc, chị đã sắp xếp thứ tự xử lý các ca đó như thế nào? Dựa vào dấu hiệu cụ thể nào mà chị quyết định hỗ trợ bạn này trước bạn kia?

**Interviewee — Lab Coach:**

Thực ra ít khi gặp tình trạng quá nhiều câu hỏi riêng lẻ dồn dập cùng lúc khiến bọn mình quá tải. Thường bọn mình phải tự đi tìm hỏi từng người. Tình huống dồn dập chỉ xảy ra khi mọi người cùng dính một lỗi chung. Khi hỗ trợ đến bạn thứ hai, thứ ba mà gặp đúng một lỗi (thường là lỗi cài đặt môi trường, cấu hình file readme hoặc codelab), bọn mình sẽ cầm mic thông báo chung cho cả lớp luôn để giải quyết dứt điểm rất nhanh. 

Sau khi giải quyết xong lỗi chung đó thì câu hỏi cá nhân giảm lại rất nhiều. Còn nếu có câu hỏi lẻ thì bọn mình cứ ưu tiên theo thứ tự bạn nào giơ tay trước thì hỗ trợ trước.

---

### Câu hỏi 3 — Trích xuất ngữ cảnh câu hỏi (Context Extraction)

**Interviewer:**

Lần gần nhất chị nhận được một câu hỏi quá ngắn hoặc diễn đạt lan man khiến chị chưa hiểu ngay bối cảnh, chị đã phải làm những bước gì để nắm được bạn ấy đang làm đến bước nào và gặp lỗi ở đâu?

**Interviewee — Lab Coach:**

Có chứ, nhiều khi câu hỏi rất "đại hải", bọn mình đọc mà hai ba đứa nhìn nhau nhăn mặt vì không hiểu bạn ấy đang muốn hỏi cái gì. Những lúc như thế, bọn mình phải ngồi đọc phân tích một hồi, rồi hỏi follow-up lại: *"Ý bạn là thế này đúng không? Bạn đang gặp lỗi ở bước này đúng không?"*. Phải làm rõ lại câu hỏi và bối cảnh thì mới đưa ra hướng giải quyết chính xác được.

---

### Kết thúc

**Interviewer:**

Những chia sẻ thực tế này giúp nhóm nắm rất rõ quy trình và các trở ngại khi hỗ trợ học viên. Cảm ơn chị rất nhiều!

---

## Evidence sơ bộ cần giữ lại

| Nhóm evidence | Ghi nhận thực tế từ Interview |
|---|---|
| **Situation (Bối cảnh)** | Coach hỗ trợ trực tiếp tại phòng lab và qua Discord buổi tối. |
| **Detection (Cách phát hiện)** | Không có công cụ đo lường tự động; Coach phải **đoán** hoặc **đi bộ rà soát từng bàn**, nhìn trộm màn hình/terminal để phát hiện điểm kẹt. |
| **Prioritization (Sắp xếp ưu tiên)** | Xử lý theo quy tắc *"đến trước phục vụ trước"* (FIFO); nếu phát hiện từ 2–3 người cùng dính một lỗi chung thì chuyển sang **cầm mic thông báo toàn lớp**. |
| **Context Gap (Ngữ cảnh câu hỏi)** | Câu hỏi của học viên thường dài dòng hoặc thiếu thông tin; Coach phải tốn thời gian trao đổi qua lại (follow-up) để gạn lọc ngữ cảnh. |
| **Hành vi học viên (Learner Behavior)** | Có xu hướng ngại giơ tay hỏi Coach; ưu tiên hỏi bạn cùng bàn hoặc dùng AI trước; ban đêm trên Discord chủ yếu hỏi về thủ tục nộp bài/lỗi build. |
| **Challenger Evidence (Điểm cần lưu ý)** | Coach không thường xuyên bị quá tải bởi số lượng câu hỏi dồn dập, trừ các lỗi hệ thống/môi trường chung. |

---

## Tự kiểm Interview (Checkpoint Checklist)

- [x] Câu hỏi 1, 2, 3 đã được neo hoàn toàn vào sự kiện quá khứ cụ thể (*"buổi học gần nhất"*, *"lần gần nhất"*).
- [x] Không để lộ solution directive hay hỏi ý kiến tương lai (*"chị có muốn..."*, *"nếu có AI..."*).
- [x] Khai thác đủ 3 khía cạnh: Phát hiện điểm nghẽn (Detection) — Sắp xếp ưu tiên (Prioritization) — Bóc tách ngữ cảnh (Context Extraction).
- [x] Đã ghi nhận đầy đủ các workaround thực tế của Coach: đi từng bàn, cầm mic giải thích chung, hỏi follow-up nhiều bước.