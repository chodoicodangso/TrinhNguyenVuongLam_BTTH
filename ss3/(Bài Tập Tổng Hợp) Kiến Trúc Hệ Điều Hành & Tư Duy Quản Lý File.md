Phần 1 — Kiến trúc Hệ điều hành  
Quản lý tài nguyên: Là chức năng Quản lý tiến trình & phân chia tài nguyên (CPU, RAM). Các phần mềm chạy song song không xung đột nhờ cơ chế phân bổ bộ nhớ ảo, chia sẻ thời gian (Time-sharing) và cách ly vùng nhớ của từng ứng dụng.  
Shell vs Kernel: Double-click mở file chạy qua lớp Shell trước để nhận lệnh từ GUI, sau đó truyền xuống Kernel (nhân hệ điều hành) để tương tác trực tiếp phần cứng. Người dùng không thao tác trực tiếp với Kernel để đảm bảo bảo mật và tránh làm sập hệ thống.  
Phần 2 — Cây thư mục & Ổ đĩa  
Cây thư mục:  
Root Directory: D:\\  
Parent Directory của anh 1.jpg: Thư mục Hinh anh  
Vai trò file anh 1.jpg: Là "lá" (file dữ liệu cuối cùng).  
Rủi ro lưu ở Desktop/Downloads (ổ C:\\): Dễ mất dữ liệu khi cài lại Windows; ổ C dễ bị phân mảnh làm chậm máy. Nên lưu trên ổ D:\\.  
Phần 3 — Đường dẫn Path  
Absolute Path:D:\\Nam1\\HocKy1\\MonHoc\\CongNgheThongTin\\BaiTapLon\\Session02\\BaoCaoCuoiKy\\Chuong1\\Hinh anh\\anh 1.jpg  
Relative Path (chèn logo.png vào report.html):assets/logo.png (giúp liên kết không bị gãy khi chuyển máy khác).  
Phần 4 — Quy tắc Đặt tên  
Tên file theo kebab-case:bao-cao-bai-tap-lon-it101-ban-cuoi-v2.docx  
Phần 5 — Tổ chức Ổ đĩa  
Thiết kế lại: Đường dẫn cũ lồng tới 8 cấp (vi phạm chuẩn gọn nhẹ). Sửa lại theo Quy tắc 3 Cấp và mô hình 4 Trụ Cột trên ổ D:\\:D:\\02\_Projects\\bai-tap-lon-it101\\chuong-1\\anh-1.jpg  
Phần 6 — Đuôi file & File ẩn  
Cạm bẫy: Máy ẩn đuôi mở rộng khiến file độc hại de-thi-dap-an.pdf.exe hiển thị lừa người dùng tưởng file PDF.  
Cách phát hiện: Vào File Explorer $\rightarrow$ chọn thẻ View $\rightarrow$ tích chọn File name extensions để hiển thị đúng đuôi file