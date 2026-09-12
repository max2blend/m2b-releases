# Chính sách bảo mật

## Kênh tin cậy

Chỉ các file đính kèm trong **GitHub Releases** của repository này được xem là
bản phát hành M2B. Mỗi ZIP phải có checksum SHA-256 riêng.

Repository phát hành không chứa:

- mã nguồn M2B;
- khóa ký, API key, token hoặc cấu hình máy chủ;
- dữ liệu khách hàng, mã đơn, PIN hoặc license key;
- workflow triển khai hạ tầng nội bộ.

## Báo lỗ hổng

Dùng **Security → Report a vulnerability**. Không công bố lỗ hổng bằng Issue.
Trong báo cáo, chỉ cung cấp phiên bản, hệ điều hành, bước tái hiện và ảnh/log đã
che dữ liệu cá nhân.

## Xác minh bản tải

Kiểm tra tên asset, phiên bản và SHA-256 trước khi cài. Không tiếp tục nếu hash
khác, ZIP bị sửa, hoặc bản tải không đến từ trang Releases chính thức.

## Cấp độ phát hành

Bản chưa có chữ ký nhà phát hành tin cậy trên mọi nền tảng phải được đánh dấu
**Pre-release**. Không đổi một asset sau khi đã phát hành; bản sửa phải tăng số
phiên bản và tạo Release mới.
