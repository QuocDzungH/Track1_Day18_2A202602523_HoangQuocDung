# Group Feedback Synthesis

> Bản tổng hợp kế thừa từ thành viên trong nhóm. Cần đối chiếu hai Feedback Notes của Quyền/Hinh và những quan sát chưa xác nhận của Trang. Các câu trong ngoặc kép dưới đây chưa có bản ghi nguồn kèm theo để xác nhận nguyên văn.

## 1. So sánh phản hồi

| Nội dung | Feedback 1 (Quyền test) | Feedback 2 (Dũng test) | Feedback 3 (Hinh test) |
| :--- | :--- | :--- | :--- |
| **Tester & Bối cảnh** | Đỗ Trường Thành Ân (2A202602899) - Người học gặp khó khi xem video | Trần Thị Thu Trang (2A202602581) - Sinh viên xem bài giảng lập trình gặp khó khăn | Dương Hải Minh (2A202602680) - Sinh viên IT tự học video bài giảng |
| **First action** | Thử bấm chuyển đổi các nút Option trước tiên để quan sát toàn bộ luồng. | Bấm *"Tôi không hiểu đoạn này!"* ở A & C; ở B thì đọc sơ đồ và chờ gợi ý. | Bấm ngay nút đỏ *"Tôi không hiểu đoạn này!"* ở A, lướt nhanh sơ đồ các node kiến thức. |
| **Breakdown chính (Chỗ gãy)** | Khó chịu với điều kiện kích hoạt của Option B (tự nhảy khi dừng video), chần chừ nút bỏ qua. | Ở A do dự vì không biết mình hổng chỗ nào; ở C dừng lại ở popup *"Bắt đúng bệnh!"* vì chưa rõ căn cứ. | Ở B chờ 3s tưởng lag; ở C khựng lại khi thấy quiz vì cảm giác bị ngắt mạch học. |
| **Cách lấy lại control** | Góp ý đổi điều kiện kích hoạt của B (người dùng có thể chỉ dừng để xem kỹ chứ không phải kẹt). | Ở B thử *"Không phải, bỏ qua"*; ở C bấm *"Đã hiểu, quay lại học tiếp"*. | Ở A xem xong bấm *"Quay lại video"*; ở C thích tự chọn lại hơn là để AI đoán rồi mới sửa sai. |
| **Option được chọn** | **Option C (AI Diagnostic)** | **Option C (AI Diagnostic)** | **Option A (User Control)** |
| **Trade-off (Sự đánh đổi)** | Chấp nhận trả lời hỏi đáp để tự kiểm tra năng lực bản thân; từ chối B vì phiền toái. | Chấp nhận trả lời thêm 2 câu quiz trước khi xem giải thích thay vì được chọn ngay. | Chấp nhận tự suy nghĩ xem mình hổng ở đâu để đổi lấy toàn quyền chủ động, không bị ngắt mạch. |
| **Counter-evidence** | Nhóm tưởng user ngại làm test, nhưng thực tế tester cực kỳ ủng hộ vì muốn được thử thách. | Chọn C nhưng lần đầu đọc giải thích vẫn chưa hiểu, phải bấm lại nút cứu trợ lần nữa. | Nhóm tưởng C là tốt nhất, nhưng tester lại chê trắc nghiệm là "sáng tạo nhưng hơi dài dòng". |

---

## 2. Tổng kết

### - Tóm tắt điểm chung từ 3 feedback:
1. **Bản tổng hợp ghi các trở ngại với Option B:** Việc tự động nhảy popup/gợi ý khi video tạm dừng bị đánh giá là can thiệp thô bạo (intrusive) hoặc gây hiểu lầm là lag. Người học dừng video có thể chỉ để đọc kỹ code/slide chứ không hẳn là cần AI trợ giúp.
2. **Sự giằng co giữa Tự chủ (Option A) và Chẩn đoán (Option C):** 
   - 2/3 tester (của Quyền và Dũng) chọn **Option C** với lý do cần đối chiếu ghi chép gốc: *"không biết mình đang hổng ở đâu"* và thích cảm giác được làm quiz để tự đánh giá năng lực.
   - 1/3 tester (của Hinh) chọn **Option A** vì muốn tốc độ nhanh, được tự quyết định và ghét việc bị ép làm trắc nghiệm làm đứt mạch học.

### - Một Next Change nhóm chốt (Group Next Change):
> **Cho phép người học tự chọn khái niệm hoặc chủ động mở chẩn đoán hai câu hỏi trong cùng luồng hỗ trợ:**
> 1. **Khung chính là Option A (Quyền tự chủ):** Khi bấm *"Tôi không hiểu đoạn này"*, hiển thị ngay Sơ đồ kiến thức để người dùng tự do bấm vào chủ đề mình muốn ôn (phục vụ nhóm tester thích tốc độ và tự chủ như tester của Hinh).
> 2. **Tích hợp Option C dưới dạng tính năng bổ trợ (On-demand):** Trên góc sơ đồ kiến thức, bổ sung nút: *"Bạn bối rối không biết mình hổng chỗ nào? Làm bài test 2 câu để AI bắt bệnh"*. Chỉ khi người học chủ động bấm vào nút này thì luồng quiz trắc nghiệm mới xuất hiện (thỏa mãn nhóm tester cần định hướng như tester của Quyền và Dũng).
> Đây là một thay đổi về luồng hỗ trợ theo lựa chọn của người học, chưa triển khai đầy đủ trong HTML hiện tại.

### - Evidence nào dẫn tới quyết định này:
- Tester của Quyền và Dũng đều chủ động tương tác với quiz và khẳng định: *"có hỏi đáp để bản thân biết mình hiểu bài hay không"* và *"thử thách mình"*, gợi ý rằng một số người học có thể muốn được định hướng bằng câu hỏi; chưa chứng minh nhu cầu chung.
- Tester của Hinh phản ánh *"hơi dài dòng, ngắt mạch học"*, gợi ý nên kiểm thử thêm một luồng không bắt buộc làm quiz.
- Cả 3 tester đều chần chừ, bối rối hoặc khó chịu với cơ chế tự kích hoạt của Option B (*"khi dừng lại mình đang muốn xem mà sao tự nhiên nhảy lên"*).

### - Still Unproven sau ba feedback:
1. **Ngưỡng quá tải nhận thức khi sơ đồ mở rộng:** Trong prototype chỉ có 3 khái niệm cơ bản (Biến số $\rightarrow$ Kiểu dữ liệu $\rightarrow$ Vòng lặp). Vẫn chưa chứng minh được nếu bài học nâng cao có 15–20 khái niệm đan xen phức tạp thì người học có còn tự tìm được ở Option A hay sẽ bắt buộc phải dựa vào quiz chẩn đoán của Option C.
2. **Độ chính xác và độ tin cậy của 2 câu hỏi quiz:** Với chỉ 2 câu hỏi ngắn, liệu AI có bắt sai bệnh trong các tình huống thực tế hay không? Nếu AI chẩn đoán sai liên tục, liệu tester của Quyền và Dũng có còn giữ sự hào hứng với Option C hay sẽ chuyển sang thất vọng?

## 3. Pattern và điểm đối lập

| Nội dung | Nhận định từ bản tổng hợp |
| --- | --- |
| First Action | Có người thử chuyển option trước, có người bấm ngay nút hỗ trợ. |
| Major Breakdown | B gây khó hiểu hoặc gián đoạn ở các phiên được mô tả; C cũng có thể cần đọc lại hoặc làm đứt mạch học. |
| Control Taken | Có người quay lại video, có người mở lại hỗ trợ. Góp ý thay đổi thiết kế không được coi là thao tác recovery đã thực hiện. |
| Selected Option | Bản tổng hợp ghi C/C/A; lựa chọn khác nhau, không chứng minh thị trường. |
| Trade-off | Định hướng bằng quiz đánh đổi số bước; tự chọn đánh đổi công sức xác định phần cần ôn. |

**Giới hạn kỹ thuật:** B dùng bộ đếm ba giây sau khi chọn option, không phát hiện video dừng thật. C không phân tích đáp án; kết quả luôn là Kiểu dữ liệu. Chưa chứng minh được độ chính xác hay hiệu quả học tập bằng mô phỏng này.

**Nguồn:** [Feedback của Dũng](prototype-feedback-note.md). Hai bản Feedback Notes độc lập của Quyền/Hinh chưa đính kèm; cần bổ sung nguồn hoặc link chung trước khi nộp.
