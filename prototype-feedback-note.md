# Prototype Feedback Note — AI Tutor

**Người phỏng vấn:**  Hoàng Quốc Dũng MHV:2A202602523
**Tester / Bối cảnh:**  Trần Thị Thu Trang(2A202602581) - Tham gia phỏng vấn trực tiếp, đóng vai người gặp khó khăn khi học bài giảng
**Prototype:** [prototype.html](prototype.html)  
**Phương án tester chọn:** Option C — AI Diagnostic.

> Bản nháp do AI hỗ trợ. Danh tính, lựa chọn C và hành vi bấm lại hỗ trợ đã được cung cấp. Các quan sát khác và lý do trade-off cần đối chiếu ghi chép thật trước khi coi là evidence. Bối cảnh học thực tế của tester chưa được ghi nhận ở đây.

## Nhiệm vụ chung cho A/B/C

Khi đang xem bài giảng Cấu trúc dữ liệu và gặp đoạn chưa hiểu, hãy dùng từng phương án để tìm kiến thức nền cần ôn và quay lại học tiếp.

## Ghi nhận phản hồi

| Tiêu điểm | Nội dung nháp cần đối chiếu với buổi test |
| --- | --- |
| First Action | Ở A và C, tester bấm “Tôi không hiểu đoạn này!”. Ở B, tester đọc sơ đồ kiến thức và chờ gợi ý xuất hiện. |
| Hesitation / Misunderstanding | Ở A, tester do dự khi phải tự chọn khái niệm mình chưa hiểu. Ở C, tester dừng lại ở kết quả “Bắt đúng bệnh!” vì chưa rõ căn cứ chẩn đoán. |
| Evidence Checking | Tester đọc phần giải thích “Kiểu dữ liệu” ở C. |
| Help Needed | Chưa có dữ liệu về số lần hoặc nội dung hỏi người điều phối; không suy ra là không cần trợ giúp. |
| Control & Recovery | Ở B, tester thử “Không phải, bỏ qua” (cần xác nhận). Ở C, tester quay lại bấm nút hỗ trợ để xem giải thích lần nữa. |
| Selected Option | **Option C — AI Diagnostic.** |
| Trade-offs | Tester chọn C và chấp nhận trả lời thêm hai câu hỏi trước khi xem giải thích; trong khi A cho phép chọn trực tiếp khái niệm cần ôn, còn B chủ động đưa ra gợi ý mà không cần trả lời câu hỏi. |
| Counter-evidence | Tester chọn C nhưng sau lần giải thích đầu vẫn chưa hiểu, nên bấm lại “Tôi không hiểu đoạn này!” để xem lại phần giải thích rồi mới hiểu. |

## Bốn tầng tư duy

**1. OBSERVED:** Tester chọn C và bấm lại hỗ trợ sau lần giải thích đầu chưa hiểu. Các thao tác khác cần xác nhận; chưa có lời nói nguyên văn của tester.

**2. INTERPRETED:** Giả thuyết là tester muốn được hỗ trợ xác định lỗ hổng kiến thức thay vì tự đoán như ở A. Chưa thể khẳng định đây là lý do thực tế nếu chưa hỏi về sự đánh đổi.

**3. DECIDED — NEXT CHANGE:** Cho phép người học tự chọn khái niệm hoặc chủ động mở chẩn đoán hai câu hỏi trong cùng luồng hỗ trợ. HTML hiện đã có đường từ C sang tự chọn; chiều mở quiz từ sơ đồ là thay đổi tiếp theo.

**4. STILL UNPROVEN:** Chưa biết C có xác định đúng phần kiến thức bị thiếu và giúp người dùng hiểu bài tốt hơn hay không. Trong prototype hiện tại, mọi lựa chọn trả lời đều dẫn đến cùng kết quả “Kiểu dữ liệu”; lựa chọn C chưa chứng minh độ chính xác của AI hay giá trị thị trường.
