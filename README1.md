Phần 1. Phân tích các lỗi cú pháp
Đoạn mã Markdown của sinh viên có 3 lỗi chính dẫn đến việc render bị lộn xộn:
1.	Lỗi chèn ảnh: [Logo PTIT] ([https://ptit.edu.vn/logo.png](https://ptit.edu.vn/logo.png))
○	Nguyên nhân: Cú pháp này thiếu dấu chấm than ! ở đầu để khai báo đây là một hình ảnh. Thêm vào đó, có một khoảng trắng thừa giữa dấu ngoặc vuông ] và dấu ngoặc đơn (.
○	Hậu quả: Trình biên dịch không hiển thị ảnh mà sẽ render thành một đoạn text hoặc một link bị lỗi (do có khoảng trắng). Cú pháp đúng phải là ![Alt text](URL).
2.	Lỗi phân cấp tiêu đề (Heading): Từ # Tiêu đề 1 nhảy thẳng xuống ### Giới thiệu dự án
○	Nguyên nhân: Sử dụng thẻ H3 (###) ngay sau thẻ H1 (#) mà bỏ qua thẻ H2 (##).
○	Hậu quả: Mặc dù Markdown vẫn render ra chữ nhỏ hơn, nhưng về mặt cấu trúc (logic hierarchy) là sai quy tắc. Các tiêu đề cần được phân cấp tuần tự từ H1 đến H2, rồi mới đến H3 để mục lục (Table of Contents) được tạo ra chính xác.
3.	Lỗi định dạng in đậm: Đây là đoạn văn bản in đậm.
○	Nguyên nhân: Thiếu ký tự đặc biệt để Markdown nhận diện đây là văn bản cần in đậm (Bold).
○	Hậu quả: Dòng này sẽ chỉ hiển thị như văn bản bình thường (plain text). Để in đậm, cần bao quanh đoạn text bằng hai dấu sao ** hoặc hai dấu gạch dưới __.
Phần 2. Hoàn thiện đoạn mã
Dưới đây là đoạn mã Markdown đã được sửa lại chuẩn cú pháp, tuân thủ quy tắc 1 thẻ H1 duy nhất và phân cấp Heading H1 -> H2 hợp lý:
Markdown
# Tiêu đề 1

## Giới thiệu dự án

![Logo PTIT](https://ptit.edu.vn/logo.png)

**Đây là đoạn văn bản in đậm.**

## Mục tiêu

- Quản lý sinh viên
- Quản lý môn học
