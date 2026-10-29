Phần 1 CLI vs GUI & Cấu trúc câu lệnh  
Phân tích câu lệnh ls \-Force C:\\Windows\\Logs:  
Command: ls  
Options/Flags: \-Force  
Argument: C:\\Windows\\Logs  
Lý do dùng Terminal với máy chủ Cloud: Các máy chủ Cloud thường chạy hệ điều hành dòng lệnh và quản lý qua SSH, hoàn toàn không cài giao diện đồ họa (GUI) để tối ưu hiệu suất và tiết kiệm tài nguyên.  
Phần 2 Điều hướng hệ thống file  
Relative Path vào thư mục dự án: cd quan-ly-sinh-vien  
Absolute Path tới main.py: C:\\Users\\student\\Desktop\\quan-ly-sinh-vien\\src\\main.py  
Xem nội dung kể cả file ẩn của data\\ từ src\\: ls \-Force ..\\data  
Phần 3 Thao tác file và thư mục  
Tạo cùng lúc 2 thư mục con: mkdir quan-ly-sinh-vien\\src, quan-ly-sinh-vien\\data  
Tạo 3 file rỗng trong 1 dòng lệnh: New-Item quan-ly-sinh-vien\\src\\main.py, quan-ly-sinh-vien\\src\\utils.py, quan-ly-sinh-vien\\README.md \-ItemType File  
Đổi tên và sao lưu project:  
Đổi tên: mv quan-ly-sv quan-ly-sinh-vien  
Sao lưu đệ quy: cp \-Recurse quan-ly-sinh-vien backup-quan-ly-sinh-vien  
Phần 4 Xử lý lỗi Terminal  
Log lỗi số 2 (cd scr): Gõ sai chính tả (scr thay vì src). Khắc phục: Gõ cd s rồi nhấn phím Tab để tự động hoàn thiện.  
Log lỗi số 3 (Access is denied): Bị chặn quyền thực thi script bảo mật trên PowerShell. Khắc phục: Chạy Set-ExecutionPolicy Unrestricted \-Scope Process.  
Log lỗi số 1 (rm old-version hỏi xác nhận): Thư mục có chứa dữ liệu con bên trong nên cần cờ đệ quy để xóa. Lệnh xóa không cần hỏi: rm old-version \-Recurse \-Force.  
Log lỗi số 4 (Python FileNotFoundError):  
(a) Dòng thông điệp lỗi: FileNotFoundError: \[Errno 2\] No such file or directory: 'data/input.csv'  
(b) Từ khóa lỗi: FileNotFoundError / No such file or directory  
(c) Kiểm tra tiếp: Đang đứng trong thư mục src nhưng code gọi đường dẫn 'data/input.csv' sai cấp; cần sửa lại thành ..\\data\\input.csv.  
