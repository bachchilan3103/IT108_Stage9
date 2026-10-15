Phần 1: Phân tích lỗi
1. Liệt kê các lỗi cú pháp và 2. Giải thích hậu quả khi render:
●	Lỗi 1: ###Lưu ý quan trọng
○	Lỗi cú pháp: Thiếu dấu cách (space) giữa các ký tự # và nội dung văn bản.
○	Hậu quả: Hệ thống sẽ không nhận diện đây là thẻ tiêu đề (Heading 3). Thay vào đó, nó sẽ hiển thị dưới dạng văn bản bình thường (plain text) kèm theo các dấu # ở đầu.
●	Lỗi 2: -Bước 1:, -Bước 2:, -Bước 3:, -Bước 4:
○	Lỗi cú pháp: Thiếu dấu cách sau ký tự gạch ngang - để tạo danh sách (list).
○	Hậu quả: Markdown sẽ không hiển thị các dòng này thành danh sách có dấu chấm (bullet list) mà chỉ xem đây là các đoạn văn bản (paragraphs) bình thường bắt đầu bằng dấu gạch ngang.
●	Lỗi 3: [GitHub]( github.com )
○	Lỗi cú pháp: Phần URL bị thiếu giao thức https:// ở đầu. (Ngoài ra có khoảng trắng thừa không cần thiết trong cặp ngoặc đơn).
○	Hậu quả: Sinh viên nhấn vào đường link sẽ bị lỗi, không trỏ tới trang web của GitHub được. (Giải thích kỹ hơn ở phần bẫy dữ liệu).
●	Lỗi 4: **HNKS25CNTT1_IT101_Session08
○	Lỗi cú pháp: Mở thẻ in đậm bằng ** nhưng quên đóng lại bằng ** ở cuối tên file.
○	Hậu quả: Chuỗi văn bản này sẽ không được in đậm, hoặc tệ hơn, trình biên dịch Markdown sẽ in đậm nhầm toàn bộ phần văn bản phía sau nó cho đến khi tìm thấy cụm ** tiếp theo.
●	Lỗi 5: *Nộp muộn sẽ bị trừ 50% điểm!**
○	Lỗi cú pháp: Không đồng nhất cú pháp đóng mở (mở bằng 1 dấu sao * tương đương in nghiêng, nhưng đóng bằng 2 dấu sao ** tương đương in đậm).
○	Hậu quả: Không thể áp dụng đúng định dạng in đậm hay in nghiêng. Hệ thống sẽ hiển thị sai định dạng hiển thị hoặc lộ nguyên các dấu sao ra ngoài màn hình.
Phần 2: Sửa lỗi
3. Đoạn Markdown sau khi đã sửa lại đúng cú pháp:
Markdown
## Hướng Dẫn Nộp Bài Tập - Session 08

### Lưu ý quan trọng
Các bước nộp bài:
- Bước 1: Tạo tài khoản GitHub tại [GitHub](https://github.com)
- Bước 2: Tạo repository mới đặt tên theo định dạng **HNKS25CNTT1_IT101_Session08**
- Bước 3: Upload file .md của bài làm lên repository
- Bước 4: Copy đường dẫn và nộp lên *Portal*

> Deadline: Chủ nhật 23:59 — **Nộp muộn sẽ bị trừ 50% điểm!**

4. Bẫy dữ liệu: Nếu sinh viên dán đường link GitHub vào Markdown mà quên gõ https:// ở đầu (tức là chỉ nhập (github.com)), thì khi render trang web, trình duyệt sẽ hiểu đây là một đường dẫn tương đối (relative path).
Thay vì điều hướng ra ngoài trang web GitHub thực sự, hệ thống sẽ chèn đoạn "github.com" vào nối tiếp ngay sau đường dẫn URL của trang web hiện tại (ví dụ: [https://lms-student.rikkei.edu.vn/.../github.com](https://lms-student.rikkei.edu.vn/.../github.com)). Kết quả là người dùng khi click vào sẽ bị điều hướng tới một trang web không tồn tại và gặp lỗi 404 (Not Found).

