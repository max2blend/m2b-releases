# Cài đặt M2B

## 1. Tải đúng gói

Từ mục **Releases**, tải ZIP phù hợp cùng file `.sha256`. Không giải nén ZIP.

## 2. Kiểm tra SHA-256

### Windows PowerShell

```powershell
Get-FileHash .\m2b-<version>-windows-x64.zip -Algorithm SHA256
```

So sánh giá trị `Hash` với file `.sha256` đi kèm.

### Linux

```bash
sha256sum -c m2b-<version>-linux-x64.zip.sha256
```

M2B dùng Secret Service để bảo vệ phiên đăng nhập. Ubuntu/Debian cần công cụ:

```bash
sudo apt install libsecret-tools
```

### macOS

```bash
shasum -a 256 -c m2b-<version>-macos-universal.zip.sha256
```

macOS có thể hỏi quyền dùng Keychain khi M2B lưu phiên đăng nhập. Chỉ chấp nhận
khi Blender và M2B được tải từ kênh này.

## 3. Cài trong Blender

1. Mở **Edit → Preferences → Add-ons** hoặc **Get Extensions**.
2. Chọn menu góc phải → **Install from Disk**.
3. Chọn nguyên file ZIP vừa tải.
4. Bật M2B và khởi động lại Blender.

Phiên bản pre-release hiện chưa có chữ ký Authenticode/Developer ID. Windows
SmartScreen hoặc macOS Gatekeeper có thể hiển thị cảnh báo. Chỉ tiếp tục khi
tên file và SHA-256 khớp chính xác với Release chính thức; không tắt cơ chế bảo
vệ của hệ điều hành trên toàn máy.

## 4. Đăng nhập

M2B mở cổng tài khoản trong trình duyệt. PIN email chỉ xác minh quyền sở hữu
email; không phải license key. Không gửi PIN hoặc license key cho người khác.

## Yêu cầu

- Blender 4.2 trở lên.
- Windows 64-bit, Linux x86-64, hoặc macOS Intel/Apple Silicon.
- Kết nối mạng khi đăng nhập và khi máy chủ kiểm tra quyền sử dụng.
