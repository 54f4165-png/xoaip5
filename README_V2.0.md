# XOAIP v2.0 – triển khai an toàn

- Giữ nguyên Firebase xoaip5, adminUids, approvedUsers, chatRooms.
- USER: chat hỗ trợ, thông báo trình duyệt theo yêu cầu, giao diện mobile cải thiện.
- ADMIN: tìm kiếm USER, tìm kiếm và lọc hội thoại, đánh dấu chưa đọc/đã xem.
- Cả hai: trạng thái đọc được lưu ở chatRooms/{uid}/readStates.
- Để trạng thái đã đọc hoạt động, sao lưu Rules hiện tại và cập nhật database.rules.json ở Firebase xoaip5 > Realtime Database > Rules. Không thay Rules dự án admin008.
- Giữ nguyên URL triển khai Vercel; upload nội dung ZIP vào root repo, đảm bảo index.html và xoaip-chat.js cùng cấp.
- Kiểm thử trên preview Vercel trước khi cập nhật production.
- Tệp đính kèm cần Firebase Storage và quy tắc Storage phù hợp; Storage Rules trong ZIP là bản v1.9 chưa được xác thực hoạt động với quyền ADMIN qua adminUids.
- Dữ liệu tài khoản/nhật ký hiện có không bị xóa bởi việc cập nhật file tĩnh.
- Không thay thế v1.9 trước khi kiểm thử đăng nhập, danh sách USER, chat, F5 và quyền truy cập.
