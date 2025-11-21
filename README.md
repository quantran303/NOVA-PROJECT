# Backend cho dự án Ngũ Hành Sơn

Nội dung:
- database.php: kết nối MySQL
- save_tour.php: API nhận POST từ form -> lưu vào table `bookings`
- save_wish.php: API nhận POST -> lưu vào table `wishes`
- api_get_bookings.php, api_get_wishes.php: trả JSON dữ liệu (dùng cho dashboard/ứng dụng)
- admin_login.php, admin_bookings.php, admin_wishes.php, admin_logout.php: giao diện quản trị rất đơn giản (username: admin / password: admin123)

Hướng dẫn nhanh:
1. Import file `export.sql` vào phpMyAdmin hoặc chạy SQL tạo DB.
2. Đặt các file PHP vào thư mục webroot (htdocs hoặc www).
3. Mở admin_login.php để đăng nhập.

Lưu ý về bảo mật:
- Mật khẩu admin trong file là demo. Nếu đưa lên production, chuyển sang hệ thống quản lý user thật, dùng HTTPS, hashing password, CSRF protection, và kiểm tra quyền truy cập.
