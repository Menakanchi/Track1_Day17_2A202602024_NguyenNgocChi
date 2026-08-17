# Chặng 1 – Đặt giả thuyết · 60 phút

**Mục tiêu:** Mở lại toàn bộ logic đang bị nén trong solution directive và biến nó thành một giả thuyết đủ cụ thể để evidence có thể làm thay đổi.

**Chuỗi logic:**
> Solution → Change → Actor → Situation & Job → Pain → Evidence

---

### 1. Solution – Gỡ solution khỏi hình thức cụ thể

* **Case đã chọn:** Case C – AI Support Radar
* **Solution directive:** 
  > Xây dựng tính năng AI Support Radar tự động giám sát và thu thập dữ liệu hành vi học tập của học viên sau mỗi phiên học (chuyển slide, dừng lâu, highlight, ghi chú, nhấn nút "Chưa hiểu", sửa đáp án trắc nghiệm, lịch sử chat với AI). Hệ thống dùng AI suy đoán nhu cầu trợ giúp và tạo bảng Support Queue đề xuất cho giảng viên/coach quyết định có can thiệp hỗ trợ học viên hay không.
* **Capability trung tính:** 
  > Khả năng tự động phát hiện và cảnh báo sớm các điểm tắc nghẽn kiến thức của từng cá nhân học viên dựa trên dữ liệu tương tác học tập thực tế, giúp người hỗ trợ chủ động can thiệp kịp thời.

---

### 2. Change – Làm lộ chuỗi thay đổi được kỳ vọng

$$\text{Solution} \rightarrow \text{Coach/Giảng viên nhận diện sớm học viên bị kẹt} \rightarrow \text{Coach chủ động mở lời hỗ trợ đúng chỗ} \rightarrow \text{Học viên vượt qua rào cản ngại hỏi để giải quyết khúc mắc} \rightarrow \text{Outcome}$$

* **Các thay đổi được kỳ vọng:**
  1. **Thay đổi về nhận thức (Awareness):** Coach/Giảng viên biết rõ danh tính học viên đang bị tụt lại và vị trí slide/bài tập cụ thể bị nghẽn ngay sau phiên học thay vì phải chờ học viên tự hỏi.
  2. **Thay đổi về hành vi (Behavior Change):** Coach chủ động nhắn tin can thiệp trúng đích; học viên chuyển từ việc âm thầm chịu đựng/bỏ dở sang tương tác tháo gỡ điểm nghẽn.
  3. **Thay đổi về kết quả (Outcome):** Giảm tỷ lệ học viên bỏ cuộc, giảm tỷ lệ trượt bài thực hành và nâng cao tỷ lệ hoàn thành khóa học.

---

### 3. Actor – Xác định các nhóm người có liên quan

| Nhóm người (Actor) | Họ đang làm gì? | Pain hoặc hậu quả có thể có | Họ hưởng lợi thế nào? |
| :--- | :--- | :--- | :--- |
| **Learner (Học viên)** | Tự xem lại bài học, thực hành, chat với AI khi chưa hiểu. | Gặp khó khăn nhưng ngại/sợ hỏi trên kênh chung Discord; dễ nản lòng và bỏ dở khóa học. | Được hỗ trợ đúng chỗ tắc nghẽn mà không phải chịu áp lực tâm lý hay mất công diễn đạt câu hỏi. |
| **Lab Coach / Instructor** | Giảng dạy, trực kênh Discord để giải đáp thắc mắc của học viên. | "Mù thông tin" về mức độ tiếp thu thực tế của lớp; chỉ hỗ trợ bị động khi có người kêu cứu; quá tải nếu rà soát thủ công. | Nắm bắt chính xác tình hình lớp, tiết kiệm thời gian lọc thông tin và can thiệp trúng đích. |
| **Platform / Vận hành** | Cung cấp nền tảng và quản lý chất lượng đào tạo tổng thể. | Tỷ lệ rớt môn cao, học viên drop giữa chừng làm giảm uy tín nền tảng. | Tăng tỷ lệ hoàn thành khóa học (Completion Rate), tối ưu hóa hiệu quả của đội ngũ coach. |

---

### 4. Situation & Job – User đang cố làm gì trong tình huống nào?

* **Mô tả Situation & Job:**
  > Khi **kết thúc một buổi học trực tuyến có nhiều kiến thức khó**, **Lab Coach/Giảng viên** đang cố **lọc ra danh sách những học viên đang bị đuối để chủ động hỗ trợ** bằng cách **đọc lướt qua tin nhắn trên kênh chung Discord và chờ xem có ai chủ động tag tên hỏi bài hay không**.

* **JTBD Hypothesis:**
  > Khi **vừa kết thúc phiên học trên lớp**, tôi muốn **nhận biết chính xác những học viên nào đang gặp khó khăn và họ kẹt ở nội dung nào**, để có thể **chủ động can thiệp và giải thích kịp thời trước khi học viên bị nản lòng hoặc rớt môn**.

---

### 5. Pain – Viết các cách giải thích cạnh tranh

* **Pain Hypothesis A (Thiếu khả năng quan sát / Mù thông tin):**
  > Khi **kết thúc một buổi học trực tuyến có nhiều kiến thức nặng**, **Lab Coach / Giảng viên** gặp khó khăn trong việc **xác định những học viên đang bị tụt lại để hỗ trợ kịp thời** vì **không có công cụ đo lường mức độ tiếp thu thời gian thực và học viên thường im lặng không chủ động hỏi**, dẫn đến **chỉ phát hiện ra học viên bị rỗng kiến thức khi bài tập bị điểm kém hoặc học viên đã nản lòng bỏ học**.

* **Pain Hypothesis B – cách giải thích cạnh tranh (Quá tải vận hành & Kênh trao đổi phân mảnh):**
  > Khi **vừa kết thúc phiên học trên lớp**, **Lab Coach / Giảng viên** gặp khó khăn trong việc **rà soát và giải đáp thắc mắc cho từng cá nhân** vì **số lượng học viên quá đông trong khi kênh trao đổi (Discord) bị phân mảnh, tốn quá nhiều thời gian để nhắn tin hỏi han từng người**, dẫn đến **coach bị quá tải, việc hỗ trợ chỉ mang tính thụ động ai kêu thì giúp, bỏ sót nhóm học viên im lặng (silent strugglers)**.

* **Giả thuyết nhóm chọn để điều tra trước:** `A`
* **Lý do chọn:**
  > Giả thuyết A tập trung vào điểm mù thông tin cốt lõi (Lack of visibility). Nếu Coach hoàn toàn không biết học viên nào đang kẹt ở slide nào thì việc có thêm thời gian cũng không thể can thiệp đúng người, đúng chỗ.

---

### 6. Evidence – Xác định điều cần tìm trước khi viết câu hỏi

| Cần kiểm tra | Evidence làm nhóm tin hơn | Evidence làm nhóm nghi ngờ hoặc bác bỏ |
| :--- | :--- | :--- |
| **Situation có thật** | Coach/Giảng viên kể được trường hợp cụ thể tuần trước lớp có nhiều bạn im lặng không hỏi bài trên Discord sau buổi học. | Buổi nào học viên cũng chủ động hỏi liên tục trên Discord, Coach không cần phải đi tìm ai kẹt. |
| **Pain có ý nghĩa** | Coach cảm thấy bế tắc vì không nắm được độ hiểu bài; học viên thừa nhận việc kẹt bài khiến họ chán nản muốn bỏ dở. | Coach thấy việc học viên im lặng là bình thường; học viên tự tin tự xử lý được mà không cần trợ giúp. |
| **Workaround tồn tại** | Coach phải mở database/log làm bài tập thủ công, hoặc nhắn tin ngẫu nhiên từng bạn để hỏi thăm. | Coach hoàn toàn không làm gì thêm sau giờ dạy, chỉ ngồi chờ ai nhắn trên Discord thì trả lời. |
| **Consequence tồn tại** | Có học viên nộp bài trắng hoặc bỏ học ở các bài sau mà Coach không kịp trở tay; dồn ứ khối lượng hỗ trợ. | Học viên dù không hỏi vẫn làm bài tập 100% đạt yêu cầu, không có ai rớt môn vì thiếu hỗ trợ. |
| **Pattern có lặp** | Hiện tượng "học viên im lặng nhưng thực ra không hiểu" xảy ra đều đặn ở hầu hết các buổi học có bài khó. | Hiện tượng này chỉ là cá biệt ở 1–2 cá nhân, không mang tính đại diện cho cả lớp. |

---

### Chốt Problem Hypothesis và park solution

* **Problem Hypothesis nhóm mang sang Chặng 2:**
  > Khi kết thúc phiên học trực tuyến, Lab Coach/Giảng viên gặp khó khăn trong việc phát hiện những học viên đang gặp khúc mắc kiến thức do thiếu tín hiệu quan sát thời gian thực và học viên có tâm lý e ngại không dám hỏi trên kênh chung Discord, dẫn đến việc bỏ lỡ thời điểm can thiệp khiến học viên bị hổng kiến thức và rớt lại phía sau.

* **Điều gì phải đúng để giả thuyết đứng vững:**
  > Học viên thực sự có hành vi "bị kẹt nhưng im lặng", và Coach thực sự quan tâm/muốn chủ động can thiệp nhưng hiện tại đang bị thiếu thông tin định hướng.

* **Điều gì có thể khiến nhóm sửa hoặc bác bỏ giả thuyết:**
  > Học viên khẳng định họ luôn chủ động hỏi khi không hiểu, hoặc Coach cho rằng việc học viên tự học/tự xoay xở là bắt buộc và Coach không có nhu cầu chủ động can thiệp trước.

---

### Solution Parking Lot

| Hướng giải quyết có thể có | AI / Không sử dụng AI |
| :--- | :--- |
| **1. AI Support Radar Dashboard:** Phân tích telemetry (thời gian dừng slide, highlight, chat với AI) để xếp thứ tự ưu tiên học viên cần can thiệp. | **AI** |
| **2. AI Auto-Intervention Bot:** Tự động phát hiện học viên dừng lâu ở 1 slide trên 3 phút và gửi tin nhắn gợi ý tóm tắt ngay trên màn hình học. | **AI** |
| **3. Checkpoint Poll 1-chạm sau mỗi phần:** Nút đánh giá mức độ hiểu bài cuối mỗi slide (*"Hiểu rõ / Còn mơ hồ / Chưa hiểu"*) để tạo Heatmap cho Coach. | **Không sử dụng AI** |
| **4. Hộp câu hỏi ẩn danh (Anonymous Q&A Box):** Cho phép học viên gửi thắc mắc ẩn danh lên Discord/Web kèm ảnh chụp slide tự động. | **Không sử dụng AI** |
| **5. Daily Standup Form sau buổi học:** Form khảo sát 2 câu ngắn bắt buộc: *"Hôm nay bạn tự tin nhất phần nào?"* và *"Phần nào bạn muốn Coach giảng lại?"*. | **Không sử dụng AI** |