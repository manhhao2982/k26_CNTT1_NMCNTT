## Phần 1: Phân tích bài toán
*Tại sao Markdown lại giúp AI xử lý tài liệu nhanh hơn và chính xác* ?
- Vì markdown sử dụng các ký hiệu **ngắn gọn**: `#` để làm tên chủ đề,  `*...*` để in nghiêng,...vậy nên sẽ không tốn token hơn so việc sử dụng các định dạng có giao diện đồ họa, ngoài ra việc hỏi AI theo cấu trúc markdown gồm 3 phần chính:
    - 1. Bối cảnh - tôi là ai / bối cảnh
    - 2. Nội dung - chủ đề/ nội dung cần xử lý
    - 3. Yêu cầu - đưa ra yêu cầu mình mong muốn
- Có cấu trúc này AI sẽ phân biệt rõ từng chủ đề và sẽ đưa ra câu phân tích rõ ràng mà không cần suy đoán người hỏi đang muốn AI trả lời theo cách nào, trả lời dài hay ngắn,...
## Phần 2. Lập bảng so sánh Markdown và HTML
|Tiêu chí|Markdown|HTML|
|:---|:---:|:---:|
|Cú pháp| Các kí tự đơn giản (#),(*  *),...|Các thẻ < h1>,< p>,...|
|Định dạng|sẽ dữ nguyên định dạng khi gửi đi|định dạng có thể bị biến tấu|
|Tiện ích|dùng để viết file README, có thể xem lịch sử thay đổi, và không dễ bị mất dữ liệu khi xảy ra sự cố, có thể xem kết quả trên VS code, git,..|hơi phức tạp nếu xảy ra nỗi sẽ làm mất nội dung, hoặc phải chỉnh sửa lại định dạng chữ|
**Lựa chọn cho lập trình viên**: sử dụng markdown vì nó tiện nghi có thể vừa xem kết quả và chỉnh sửa, có định dạng utf8 phù hợp một bản hưởng dẫn sử dụng hay báo cáo cho một dự án.
