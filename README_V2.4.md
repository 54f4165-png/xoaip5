# XOAIP USER v2.4 — Âm báo tự động

- Giữ nguyên Firebase xoaip5 và mọi chức năng v2.3.
- Không cần nút bật âm thanh riêng: hệ thống tự mở khóa WebAudio khi người dùng nhấp, gõ phím hoặc chạm vào trang lần đầu.
- Khi có tin nhắn mới từ phía bên kia, âm báo sẽ tự phát nếu trình duyệt cho phép.
- Giữ nguyên cơ chế không báo lại tin cũ khi tải trang và số chưa đọc.
- Trình duyệt không cho phép bảo đảm âm thanh trước tương tác đầu tiên hoặc khi trang đã đóng.
- Nút Bật thông báo (nếu hiển thị) dùng cho quyền thông báo hệ thống, không phải nút bật âm thanh.

Triển khai: thay các file trong repository USER, chờ Vercel Ready, tải lại trang, nhấp một lần và thử gửi tin mới. Không cần đổi Firebase Rules.
