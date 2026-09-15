# Changelog

## 1.2.0 — 2026-09-15

- Phát hành đồng nhất Windows x64, Linux x64 và macOS Universal từ cùng một
  commit riêng tư đã qua CI và kiểm tra cài ZIP thật.
- Chuyển tài khoản dùng thử mới sang 7 ngày liên tục kể từ lần kích hoạt addon
  đã xác minh; phiên dùng thử 24 giờ tích lũy đã cấp trước đây vẫn được giữ.
- Tách tuyệt đối Customer Portal và Operations Portal; quyền duyệt thanh toán,
  bổ nhiệm/thu hồi người duyệt và khóa tài khoản đều được kiểm tra phía máy chủ.
- Hỗ trợ ba gói 1/3/5 thiết bị qua Gumroad USD hoặc MoMo VND; quyền chỉ được cấp
  sau khi giao dịch được backend đối soát hợp lệ.
- Dùng kho thông tin đăng nhập bảo vệ bởi hệ điều hành: Windows DPAPI, macOS
  Keychain và Linux Secret Service.
- Giữ signed operation permit và kiểm tra quyền server-side trước thao tác được
  bảo vệ.

Bản 1.2.0 được công bố dạng **Pre-release** vì executable chưa có chữ ký
Authenticode/Developer ID của nhà phát hành. SHA-256 xác minh tính toàn vẹn
file tải, nhưng không thay thế chữ ký danh tính nhà phát hành.
