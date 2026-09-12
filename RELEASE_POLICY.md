# Quy tắc phát hành

1. Mã nguồn và quy trình build nằm trong repository riêng tư.
2. Windows, Linux và macOS được dựng từ cùng một commit và cùng số phiên bản.
3. Mỗi nền tảng phải qua Rust tests, Blender registration, cài ZIP thật và
   package-boundary scan.
4. GitHub tag `vX.Y.Z` là bất biến. Không ghi đè asset đã công bố.
5. File cài chỉ tồn tại dưới dạng GitHub Release assets; không commit ZIP vào
   branch `main`.
6. Mỗi ZIP có một file `.sha256` cùng tên.
7. Không đưa source map, log build, file cấu hình, secret hoặc dữ liệu khách
   hàng vào artifact.
8. Bản chưa ký đầy đủ phải là Pre-release. Chỉ nâng thành Latest sau phê duyệt
   production riêng.
