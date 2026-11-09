# XOAIP v2.2 – Thông báo tin nhắn

- Giữ Firebase xoaip5, giao diện và các chức năng cũ.
- USER: badge chỉ đếm tin ADMIN chưa đọc, tự ẩn sau khi mở chat và xem tin.
- ADMIN: badge ở tiêu đề chat và từng hội thoại đếm số tin USER chưa đọc, ẩn khi đã xem.
- Hai phía có âm báo khi nhận tin mới (trình duyệt có thể yêu cầu tương tác trước khi phát).
- Không phát âm báo cho tin nhắn của chính mình hoặc khi tải lịch sử ban đầu.
- Giữ Enter gửi, Shift+Enter xuống dòng, Ctrl+V ảnh, Spam.

## Triển khai
1. Sao lưu repository và Firebase Rules hiện tại.
2. Tải nội dung ZIP vào đúng repository trên GitHub, chờ Vercel Ready.
3. Giữ Firebase xoaip5; database.rules.json kèm theo tương thích readStates và Spam. Chỉ publish Rules nếu đang thiếu các nhánh này, sau khi đối chiếu bản đang dùng.
4. Kiểm thử bằng 2 trình duyệt/tài khoản khác nhau. Khi mở chat, số chưa đọc trở về 0.

Lưu ý: Âm thanh trong trình duyệt thường chỉ phát sau một lần người dùng tương tác với trang. Không thể bảo đảm âm báo khi tab đã đóng.
