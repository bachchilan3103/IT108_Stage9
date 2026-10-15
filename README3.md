Phần 1: Điền khuyết
1. Giải thích chi tiết các chỗ trống cần điền:
●	Chỗ trống 1 (Sau dấu #): Xóa bỏ ____ (Chỉ cần giữ lại một dấu cách).
○	Lý do: Cú pháp Heading H1 chuẩn trong Markdown là ký tự # theo sau là một dấu cách, sau đó đến nội dung (# 📅 Ứng dụng...).
●	Chỗ trống 2 & 3 (Đóng/mở Code Block): Điền ``` (3 dấu backtick).
○	Lý do: Để tạo một khối mã (code block) cho ngôn ngữ Bash, cần mở đầu bằng ```bash và kết thúc khối mã bằng ```.
●	Chỗ trống 4, 5, 6 (Trước các ô checkbox): Điền dấu - (dấu gạch ngang) hoặc * (dấu sao).
○	Lý do: Cú pháp danh sách công việc (Task List) trong Markdown yêu cầu phải có ký hiệu danh sách (bullet point) trước checkbox. Cú pháp chuẩn là - [x] cho mục đã hoàn thành và - [ ] cho mục chưa hoàn thành.
●	Chỗ trống 7, 8, 9 (Hàng phân cách bảng): Điền --- (3 dấu gạch ngang) vào mỗi ô.
○	Lý do: Để Markdown hiểu đây là một bảng, bắt buộc phải có hàng phân cách giữa dòng tiêu đề (Header) và phần nội dung dữ liệu. Cú pháp cơ bản là | --- | --- | --- |.
Phần 2: Hoàn thiện
2. Nội dung file README.md hoàn chỉnh:
Markdown
# 📅 Ứng dụng Quản lý Lịch Học Cá nhân
Ứng dụng giúp sinh viên ***lên kế hoạch học tập*** hiệu quả.

## 🚀 Hướng dẫn Cài đặt
```bash
git clone https://github.com/nhom5/lich-hoc-app
cd lich-hoc-app

✅ Tính năng đã hoàn thành
●	[x] Đăng ký / Đăng nhập tài khoản
●	[ ] Nhắc nhở lịch học qua email
●	[x] Xuất lịch ra file PDF
📊 Bảng So sánh Công nghệ
Công nghệ	Mục đích	Phiên bản
Python	Backend xử lý dữ liệu	3.11
Markdown	Viết tài liệu README	-

---

### Phần 3: Bẫy dữ liệu
**3. Trả lời câu hỏi bẫy dữ liệu:**
*   **Hiện tượng:** Nếu hàng phân cách bảng (`| --- | --- | --- |`) bị xóa, toàn bộ phần nội dung bảng sẽ **không được hiển thị dưới dạng bảng (table)**. 
*   **Nguyên nhân:** Trình biên dịch Markdown (Markdown parser) sử dụng hàng phân cách này làm dấu hiệu bắt buộc để nhận biết đâu là ranh giới giữa dòng Tiêu đề (Header) và các dòng Dữ liệu (Body). Khi mất đi hàng này, Markdown sẽ chỉ coi các dòng văn bản đó là các đoạn text bình thường có chứa ký tự `|` chứ không render ra cấu trúc bảng HTML.

