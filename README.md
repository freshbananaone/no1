# Giảm chi phí vận hành Chatbot AI
## Phần 1. Phân tích bài toán

Trong AI **Token** là đơn vị nhỏ nhất, có ý nghĩa trong văn bản. Mỗi token có thể là một từ, một phần của từ hoặc ký hiệu. Số token đầu vào càng lớn thì chi phí thường càng cao và thời gian xử lý đầu vào có thể tăng.

Với cùng một nội dung, Markdown thường dùng ít ký tự dịnh dạng so với HTML. Ví dụ, để in đậm từ “Lúa”:

- Markdown: `**Lúa**` — 7 ký tự.
- HTML: `<strong>Lúa</strong>` — 20 ký tự.

HTML có thêm thẻ mở và thẻ đóng nên AI phải tiếp nhận cả những phần ký hiệu này. Markdown ngắn gọn hơn, thường giúp giảm token đầu vào, tiết kiệm chi phí và góp phần giảm thời gian xử lý. Tuy nhiên, **số token chính xác phụ thuộc vào bộ tách token của mô hình**, không thể suy ra trực tiếp chỉ từ số ký tự.

## Phần 2. So sánh và đánh giá
| Tiêu chí | Markdown | HTML |
|---|---|---|
| Ký tự định dạng | Ít, cú pháp ngắn gọn như `**Lúa**` | Nhiều hơn do dùng thẻ như `<strong>Lúa</strong>` |
| Khả năng đọc trực tiếp | Dễ đọc ngay cả khi chưa hiển thị định dạng | Khó đọc hơn khi có nhiều thẻ và thuộc tính |
| Token đầu vào | Thường ít hơn với nội dung tương đương | Thường nhiều hơn, đặc biệt khi chứa mã giao diện |
| Hiệu quả xử lý AI | Giảm phần định dạng dư thừa, giúp tiết kiệm chi phí | Tốn thêm tài nguyên để xử lý các thẻ không cần thiết |
| Khả năng trình bày | Phù hợp với tiêu đề, danh sách, bảng và hướng dẫn | Phù hợp với trang web có cấu trúc và giao diện phức tạp |

# Giải pháp cho hệ thống GreenTech
Nên sử dụng **Markdown làm định dạng nội dung gửi cho AI**, tổ chức kiến thức nông nghiệp bằng tiêu đề, danh sách và bảng đơn giản. Ví dụ, hướng dẫn chăm sóc lúa có thể chia thành các mục: triệu chứng, nguyên nhân và cách xử lý.

Lựa chọn này giúp giảm token định dạng, tiết kiệm chi phí và thuận tiện cho nhân viên kiểm tra, cập nhật kiến thức. Khi hiển thị cho người nông dân trên website, hệ thống có thể chuyển Markdown thành HTML. Với dữ liệu HTML có sẵn, cần loại bỏ các thành phần giao diện không cần thiết nhưng vẫn giữ đầy đủ nội dung và cấu trúc có ý nghĩa trước khi gửi cho AI.# IT13
