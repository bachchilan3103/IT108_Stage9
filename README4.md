# Session08 - Ex01: Plain Text, Rich Text và Markdown
Phần 1. Phân tích
Sai lầm 1: Cho rằng Word phù hợp để lưu trữ tài liệu trên GitHub
Nam sử dụng file Word (.docx) để lưu trữ tài liệu dự án và đưa lên GitHub. Đây là lựa chọn chưa phù hợp vì file Word là định dạng nhị phân (binary file). Khi các thành viên trong nhóm muốn xem nội dung, GitHub không thể hiển thị nội dung trực tiếp một cách thuận tiện như các tệp văn bản.

Ngoài ra, Git khó theo dõi sự thay đổi chi tiết bên trong file Word. Chỉ cần sửa một dấu phẩy hoặc một dòng nhỏ, Git có thể coi toàn bộ file đã thay đổi, làm tăng nguy cơ xảy ra xung đột (Conflict) khi làm việc nhóm.

Sai lầm 2: Cho rằng Markdown không thể tạo tài liệu chuyên nghiệp
Nam nhận định rằng Markdown chỉ là văn bản thô nên không thể tạo tài liệu chuyên nghiệp. Đây là một quan niệm sai lầm.

Markdown hỗ trợ nhiều tính năng trình bày như:

Tiêu đề (Heading)
Danh sách (List)
Bảng (Table)
Hình ảnh (Image)
Liên kết (Link)
Đoạn mã nguồn (Code Block)
Các dự án mã nguồn mở lớn trên GitHub đều sử dụng README.md để xây dựng tài liệu chuyên nghiệp, dễ đọc và dễ bảo trì.

Vì sao Markdown an toàn và nhẹ hơn Word?
1. Dễ phục hồi khi lỗi dữ liệu
Markdown là văn bản thuần (Plain Text).

Ví dụ:

# Giới thiệu dự án

Đây là hệ thống quản lý sinh viên.
Nếu tệp Markdown bị mất một vài ký tự do lỗi mạng, phần lớn nội dung vẫn có thể đọc được.

Ngược lại, file Word (.docx) có cấu trúc phức tạp. Nếu dữ liệu bị hỏng chỉ một phần nhỏ, toàn bộ file có thể không mở được.

2. Kích thước nhỏ
Markdown chỉ lưu nội dung và cú pháp định dạng đơn giản.

Word phải lưu thêm:

Font chữ
Màu sắc
Kiểu định dạng
Hình ảnh nhúng
Metadata
Do đó file Markdown thường nhẹ hơn đáng kể.

3. Hỗ trợ Git Diff tốt
Git có thể dễ dàng xác định dòng nào được thay đổi trong file Markdown.

Ví dụ:

- Hệ thống quản lý sinh viên.
+ Hệ thống quản lý sinh viên và môn học.
Điều này giúp làm việc nhóm hiệu quả và giảm xung đột khi merge code.

Phần 2. Hoàn thiện
Nội dung gốc từ Word
Giới thiệu dự án:

Dự án xây dựng hệ thống quản lý sinh viên cho trường PTIT. Hệ thống hỗ trợ quản lý thông tin sinh viên, môn học và kết quả học tập.

Chuyển sang Markdown bằng StackEdit
# Hệ Thống Quản Lý Sinh Viên PTIT

## Giới thiệu

Dự án xây dựng hệ thống quản lý sinh viên cho trường PTIT.

### Chức năng chính

- Quản lý thông tin sinh viên
- Quản lý môn học
- Quản lý kết quả học tập

### Công nghệ sử dụng

- Git
- GitHub
- Markdown

### Mục tiêu

Xây dựng hệ thống hỗ trợ quản lý dữ liệu sinh viên hiệu quả và dễ sử dụng.
Kết luận
Markdown là định dạng phù hợp hơn Word trong môi trường phát triển phần mềm vì:

Là văn bản thuần (Plain Text)
Dễ đọc và dễ phục hồi dữ liệu
Hỗ trợ Git Diff hiệu quả
Dung lượng nhỏ
Hiển thị trực tiếp trên GitHub
Thuận tiện cho làm việc nhóm