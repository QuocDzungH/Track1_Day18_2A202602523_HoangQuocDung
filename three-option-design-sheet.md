# Three Option Design Sheet — AI Tutor

## 1. Hypothesis Problem

Khi **đang học bài mới và gặp khái niệm khó** (Situation), **người học** (User) gặp khó khăn trong việc **hoàn thành bài học** (Job) vì **không tự xác định được lỗ hổng kiến thức nền** (Barrier), dẫn đến **tra cứu mông lung, mất thời gian và gián đoạn mạch học** (Consequence).

Evidence Day 17 được mô tả trong phiên làm việc: highlight thuật ngữ, khó tìm lại phần cần đọc trong slide dài, mở nhiều tab làm ngắt quãng suy nghĩ. Bản ghi nguồn chưa được đính kèm trong thư mục này.

**Ẩn số:** Trở ngại chính là kiến thức nền hay cách diễn đạt? Hỗ trợ tại chỗ có cải thiện hiệu quả học không?

## 2. Comparison Contract

Cùng người học gặp đoạn chưa hiểu, cùng Bài 5 — Cấu trúc dữ liệu, video mô phỏng, ba khái niệm Biến số/Kiểu dữ liệu/Vòng lặp và đích quay lại học.

**Nhiệm vụ chung:** Dùng từng phương án để tìm kiến thức nền cần ôn rồi quay lại học tiếp.

- **A — Quyền:** Người học mở sơ đồ dựng sẵn, tự chọn node.
- **B — Dũng:** Sau ba giây kể từ khi chọn B, gợi ý Kiểu dữ liệu xuất hiện. Không phát hiện dừng video thật.
- **C — Hinh:** Trả lời hai câu tự đánh giá rồi xem kết quả mẫu Kiểu dữ liệu. Mọi đáp án đều dẫn tới cùng kết quả.

## 3. Human–AI Decision Table — hiện trạng HTML

| Trụ cột | A | B | C |
| --- | --- | --- | --- |
| Expectation | Yêu cầu tự chọn khái niệm; chưa nêu rõ nội dung dựng sẵn. | Thông báo chờ ba giây, hỏi xác nhận; chưa nêu giới hạn suy đoán. | Báo chẩn đoán hai câu; “Bắt đúng bệnh!” đang quá chắc chắn so với kết quả mô phỏng. |
| Role & Agency | User chọn; Act hiển thị thẻ. Không tự kết luận. | Act hiện gợi ý; Ask trước khi mở giải thích đề xuất; user cũng có thể tự chọn node. | User trả lời; Act hiển thị kết quả mẫu, không phân tích đáp án thật. |
| Evidence & Uncertainty | Chưa có nguồn trích dẫn. | Highlight/câu hỏi là dấu hiệu gợi ý, chưa phải căn cứ minh chứng. | Không có cột điểm, trích dẫn hay độ bất định. |
| Control & Recovery | Chọn node khác, đóng bằng × hoặc “Quay lại video”. | “Không phải, bỏ qua”, chọn node khác, đổi option để reset. | Quay lại học hoặc “AI chẩn đoán chưa đúng? Tự chọn phần cần xem lại” để mở A. Bước quiz chưa có nút đóng trực tiếp. |

**Cost of failure:** Ôn nhầm, mất thời gian, hiểu sai năng lực. **Don't Act:** Không tự chấm điểm chính thức, đổi tiến độ hoặc quyết định năng lực thay người học.

Không có API AI, ghi nhớ sở thích, Like/Dislike hoặc lưu lịch sử học. Thẻ A/B còn ngắn; nguồn minh chứng và thông báo giới hạn chưa đầy đủ.

## 4. Vòng tiếp theo

**Một Next Change:** Cho phép người học tự chọn khái niệm hoặc chủ động mở chẩn đoán hai câu hỏi trong cùng luồng hỗ trợ. Hiện có đường từ C sang A; chiều mở quiz từ sơ đồ chưa triển khai.
