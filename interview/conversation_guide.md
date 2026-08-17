# Chặng 2

## Vì sao phải sửa — điều ba interview đã bác và làm rõ

Giả thuyết gốc ban đầu xây dựng trên giả định: Learner ngại hỏi/không biết diễn đạt, còn Coach bị quá tải vì hàng loạt câu hỏi dồn dập cần AI sắp xếp thứ tự ưu tiên. Cả 3 cuộc phỏng vấn (2 Learner + 1 Coach) đã bộc lộ bản chất thực tế hoàn toàn khác.

| Đối tượng | Hành vi thật | Điểm gãy / Pain thật |
| :--- | :--- | :--- |
| **Learner 1** | "Mình sẽ hỏi" — lên Discord, nhắn thẳng Lab Coach: *"Anh ơi, em bị vướng phần này, phần này"* | Người tiếp nhận **không phụ trách đúng phần đó** → *"chưa trả lời cho mình thỏa đáng"* |
| **Learner 2** | Nhắn qua Discord, gọi Lab Coach ngay khi gặp lỗi code | Lab Coach bận/quên yêu cầu; phải **load lại bối cảnh** dự án/bài học nên khó hiểu ngay |
| **Lab Coach (LC-01)** | Không có cảnh báo tự động; phải **đi bộ dò từng bàn, nhìn lướt terminal**; dùng mic xử lý lỗi chung; nhắc đọc codelab; hỏi follow-up nhiều bước | Mù thông tin về tiến độ của nhóm im lặng; **Context Gap**: câu hỏi gửi đến quá dài lan man ("đại hải") khiến Coach tốn thời gian giải mã |

**Ba cơ chế hỏng thực tế trong quy trình hỗ trợ:**

1. **Detection & Visibility Gap** — Coach không có công cụ phát hiện tự động, phải đi đoán/dò thủ công quanh lớp; học viên không hiểu bài và không được can thiệp kịp thời dẫn đến hành vi tiêu cực (thả bot vào phá hệ thống).
2. **Context Gap & Routing** — Người hỗ trợ vào cuộc mà không có sẵn bối cảnh (slide nào, terminal lỗi gì, repo nào); học viên diễn đạt câu hỏi dài dòng ("đại hải") làm Coach mất nhiều thời gian hỏi follow-up để hiểu đúng vấn đề.
3. **Capacity & Ownership** — Số lượng Coach ít; phân công hỗ trợ chưa đúng chuyên môn từng phần bài học dẫn đến việc yêu cầu bị trôi hoặc trả lời không thỏa đáng.

**Hệ quả cần nhóm cân nhắc đối với Solution Directive:**
Directive ban đầu tập trung vào thành phần *(1) Danh sách xếp hàng ai cần hỗ trợ*. Tuy nhiên, evidence thực tế chứng minh giá trị cốt lõi nhất cần giải quyết nằm ở thành phần *(2) & (3) của Directive: Tự động trích xuất ngữ cảnh (Context Transfer)* và *Định vị chính xác điểm nghẽn (Pinpoint Bottleneck)* để giảm tải công sức đi dò bàn của Coach và xóa bỏ khoảng cách diễn đạt của Learner.

**Pain Hypothesis C — đề xuất cập nhật cho toàn nhóm:**

> Khi học viên gặp khó khăn trong buổi học (hoặc qua Discord), quy trình hỗ trợ bị tắc nghẽn vì Coach không có tín hiệu nhận diện sớm (phải đi dò từng bàn) và câu hỏi của học viên bị thiếu bối cảnh kỹ thuật (context gap), dẫn đến việc Coach mất nhiều thời gian làm rõ câu hỏi, hỗ trợ sai chuyên môn, hoặc học viên nản lòng sinh ra hành vi phá rối/bỏ dở bài học.

**Điều gì sẽ bác Pain C:** Learner và Coach khẳng định các buổi học đều nắm bắt bối cảnh của nhau ngay lập tức; không có câu hỏi nào bị hiểu sai ngữ cảnh; và Coach không tốn thời gian cho việc đi dò tìm người kẹt bài.

---

## 1. Big 3 

| # | Điều cần học | Evidence cần tìm | Điều gì khiến nhóm xem lại giả thuyết? |
| :--- | :--- | :--- | :--- |
| **1** *(đáng sợ)* | **Context Gap & Trở ngại tiếp nhận:** Yếu tố nào làm lần hỗ trợ bị kéo dài — Coach không nắm bối cảnh, câu hỏi lan man, hay sai người phụ trách? | Lần gần nhất: Coach/Learner mất bao nhiêu phút và bao nhiêu lượt chat để làm rõ ngữ cảnh câu hỏi trước khi đi vào fix lỗi thực sự. | Câu hỏi gửi đi luôn được hiểu đúng ngay lập tức trong 30 giây đầu tiên, không cần hỏi follow-up. |
| **2** | **Hậu quả thật (Consequence):** Việc hỗ trợ chậm/không đúng bối cảnh gây ra hậu quả gì cho cả hai phía? | Hành động sau đó: Học viên thả bot phá, bỏ bài, nộp thiếu; Coach tốn thời gian đi lại từng bàn hoặc dồn ứ việc giải đáp lúc đêm muộn. | Học viên vẫn hoàn thành bài tập 100% đúng hạn; Coach không thấy việc đi dò từng bàn là phiền toái. |
| **3** | **Pattern & Cơ chế tự xử lý (Workarounds):** Tần suất xuất hiện lỗi chung và cách phân luồng hỗ trợ trong 7 ngày gần đây. | Số lần Coach phải cầm mic thông báo chung; số lần học viên ưu tiên hỏi AI/bạn cùng bàn trước khi tìm đến Coach. | Mọi câu hỏi đều là lỗi cá biệt chưa từng lặp lại; học viên không bao giờ dùng AI hay hỏi bạn xung quanh. |

---

## 2. Conversation Guide — bản v2

### Tiêu chí tuyển người

Chúng tôi cần nói chuyện với người đã **trực tiếp tham gia học/làm bài thực hành hoặc trực tiếp làm Lab Coach hỗ trợ** trong vòng **7** ngày gần đây.

Mục tiêu bao phủ: **2 Learner + 1 Lab Coach**.

### Recruitment check

* **Với Learner:** *"Trong 7 ngày gần đây, bạn có thể kể tên một buổi lab cụ thể mà bạn gặp lỗi kỹ thuật hoặc phải nhờ Coach trợ giúp không?"*
* **Với Coach:** *"Trong các buổi học tuần vừa rồi, anh/chị có trực tiếp đứng lớp hướng dẫn thực hành và giải đáp thắc mắc trên Discord không?"*

### Lời mở đầu

"Bọn mình đang tìm hiểu về trải nghiệm thực tế trong quá trình học thực hành và hỗ trợ giải đáp thắc mắc giữa học viên và đội ngũ Coach. Cuộc trò chuyện này hoàn toàn nhằm mục đích học hỏi quy trình thực tế, không có câu trả lời đúng hay sai và tụi em không đánh giá bất kỳ ai. Bọn mình sẽ chỉ hỏi về những sự kiện cụ thể đã diễn ra trong các buổi học vừa qua."

### Story opener

* **Dành cho Learner:** *"Kể mình nghe về lần gần nhất trong 7 ngày qua bạn bị mắc ở một đoạn code/slide và phải tìm sự trợ giúp. Hôm đó là bài nào và bạn đã xử lý thế nào?"*
* **Dành cho Coach:** *"Kể em nghe về lần gần nhất trong tuần qua anh/chị trực tiếp đứng lớp hỗ trợ bài lab và phát hiện học viên đang gặp sự cố?"*

---

### Big 3 Questions — Dành cho Learner

| STT | Điều cần học | Câu hỏi sẽ dùng |
| :--- | :--- | :--- |
| **1** | **Ngữ cảnh & Tiếp nhận hỗ trợ** | *"Sau khi bạn nhắn hỏi hoặc gọi Coach, bạn đã phải giải thích những gì để Coach hiểu được phần bạn đang làm? Coach có nắm được ngay bài bạn đang làm không?"* |
| **2** | **Hậu quả thật** | *"Sau lần hỗ trợ chưa thỏa đáng (hoặc phải chờ lâu) đó, bạn đã làm gì tiếp theo? Việc đó ảnh hưởng thế nào đến việc hoàn thành bài tập hôm đó?"* |
| **3** | **Pattern & Workaround** | *"Trong tuần qua, trước khi gọi Coach thì bạn đã thử những cách nào khác (hỏi bạn bên cạnh, hỏi AI ngoài)? Tỷ lệ tự gỡ được là bao nhiêu?"* |

---

### Big 3 Questions — Dành cho Lab Coach

| STT | Điều cần học | Câu hỏi sẽ dùng |
| :--- | :--- | :--- |
| **1** | **Cách phát hiện & Độ trễ nhận biết** | *"Trong buổi học gần nhất, từ lúc học viên gặp sự cố (terminal lỗi, đứng hình) đến khi anh/chị phát hiện ra là mất bao lâu? Anh/chị nhận biết bằng cách nào khi bạn ấy không giơ tay?"* |
| **2** | **Xử lý Context Gap (Câu hỏi lan man)** | *"Lần gần nhất nhận một câu hỏi dài dòng hoặc thiếu thông tin, anh/chị đã mất bao nhiêu thời gian và làm những bước nào để làm rõ bối cảnh câu hỏi trước khi trả lời?"* |
| **3** | **Hành vi khắc phục & Xử lý lỗi chung** | *"Kể lại lần gần nhất có nhiều bạn cùng vướng một lỗi: Anh/chị đã làm gì để giải quyết dứt điểm cho cả lớp mà không phải đi đến từng bàn?"* |


---

### Probe bank & Phản xạ khi Data lệch hướng

* **Probe bank (Đào sâu câu chuyện):**
* *"Lúc học viên không hiểu bài và bắt đầu có hành vi thả bot phá hệ thống, anh/chị đã xử lý tình huống đó thế nào?"*
* *"Khi học viên hỏi câu hỏi 'đại hải', anh/chị phải hỏi follow-up bao nhiêu câu thì mới chốt được vấn đề?"*
* *"Có bao giờ anh/chị đến hỗ trợ nhưng nhận ra nội dung bài đó không thuộc phần chuyên môn chính của mình không? Lúc đó anh/chị xử lý ra sao?"*

* **Ba phản xạ khi data bắt đầu lệch:**

| User đưa ra | Phản xạ | Cách quay lại evidence |
| :--- | :--- | :--- |
| **Lời khen** | **Deflect** | Cảm ơn ngắn rồi quay lại việc họ đang làm hiện tại: *"Dạ vâng, vậy trong buổi học gần nhất chuyện đó diễn ra cụ thể thế nào ạ?"* |
| **Câu chung chung hoặc lời hứa tương lai** | **Anchor** | Neo về quá khứ: *"Lần gần nhất chuyện đó xảy ra là khi nào ạ? Lúc đó anh/chị đã xử lý ra sao?"* |
| **Ý tưởng hoặc feature request** | **Dig** | Đào sâu pain gốc: *"Điều đó giúp anh/chị giải quyết được khó khăn gì cụ thể? Hiện tại khi chưa có nó thì anh/chị đang xử lý bằng cách nào?"* |

---

### Tự rà soát và phân công (Checkpoint 2 Checklist)

- [x] Không có câu nào làm lộ solution (không nhắc AI Support Radar, Support Queue, Dashboard).
- [x] Không có câu nào hỏi ý kiến tương lai hay giả định (*"anh/chị có muốn..."*).
- [x] Story opener đã neo chính xác vào *"lần gần nhất"*.
- [x] Ba câu hỏi chính nối trực tiếp với Big 3.
- [x] Câu hỏi số 2 là câu hỏi "đáng sợ" kiểm chứng xem có thực sự xảy ra tình trạng quá tải câu hỏi lẻ cần AI xếp hàng hay không.
- [x] Interviewee đáp ứng tiêu chí tuyển (Lab Coach thực tế đứng lớp).