# CloudSave Sync Studio

<div align="center">

**Ứng Dụng Desktop Windows Tự Động Đồng Bộ & Bảo Vệ Save Game Đa Thiết Bị Qua Google Drive**

[![Release](https://img.shields.io/badge/Release-V1.0.0-emerald.svg?style=for-the-badge)](https://github.com/minhnguyenbd2-blip/CloudSave-Sync/releases/latest)
[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%2F%2011%20x64-blue.svg?style=for-the-badge)](https://github.com/minhnguyenbd2-blip/CloudSave-Sync/releases/latest)
[![Cloud](https://img.shields.io/badge/Cloud-Google%20Drive%20OAuth-amber.svg?style=for-the-badge)](https://github.com/minhnguyenbd2-blip/CloudSave-Sync)
[![License](https://img.shields.io/badge/License-MIT-purple.svg?style=for-the-badge)](https://github.com/minhnguyenbd2-blip/CloudSave-Sync)

</div>

---

## 📥 Tải Về & Cài Đặt Cho Người Dùng Windows (1 File Duy Nhất)

Người dùng chỉ cần tải **1 tệp cài đặt duy nhất (`CloudSaveSync-Setup.exe`)** từ trang **GitHub Releases** để cài đặt toàn bộ ứng dụng Native Desktop vào máy tính Windows 10 / Windows 11 (64-bit):

| Gói Phân Phối Chính Thức | Định Dạng | Mô Tả | Liên Kết Tải Về |
| :--- | :---: | :--- | :---: |
| **CloudSaveSync-Setup.exe** | `.exe` (Standalone) | **Trình cài đặt trọn gói Windows Setup Wizard (Khuyên dùng)** | [**Tải Bản Mới Nhất Tại GitHub Releases**](https://github.com/minhnguyenbd2-blip/CloudSave-Sync/releases/latest/download/CloudSaveSync-Setup.exe) |
| **CloudSaveSync-Setup-V1.0.0-Win11-x64.exe** | `.exe` (Versioned) | Bản cài đặt chính thức đóng dấu phiên bản V1.0.0 | [**Tải Bản V1.0.0**](https://github.com/minhnguyenbd2-blip/CloudSave-Sync/releases/download/V1.0.0/CloudSaveSync-Setup-V1.0.0-Win11-x64.exe) |
| **RELEASE_NOTES.md & SHA256SUMS.txt** | Tài liệu & Mã băm | Thông tin cập nhật & mã kiểm tra toàn vẹn tệp tin SHA-256 | [**Xem Chi Tiết**](02_User_Official_Release/github-release/RELEASE_NOTES.md) |

---

## 🚀 Hướng Dẫn Cài Đặt Nhanh

1. Tải tệp **[`CloudSaveSync-Setup.exe`](https://github.com/minhnguyenbd2-blip/CloudSave-Sync/releases/latest/download/CloudSaveSync-Setup.exe)** về máy tính.
2. Nhấp đúp chuột chạy file để mở trình cài đặt **Windows Setup Wizard**.
3. Chọn thư mục cài đặt (Mặc định: `%LOCALAPPDATA%\CloudSaveSync`) và nhấn **Cài đặt (Install)**.
4. Trình cài đặt sẽ tự động giải nén toàn bộ ứng dụng Native Desktop, tạo biểu tượng trên **Desktop** & **Start Menu**, đăng ký vào **Windows Installed Apps**, và khởi chạy ứng dụng ngay lập tức!

---

## ✨ Tính Năng Nổi Bật Dành Cho Game Thủ

### 1. 🖥️ Ứng Dụng Native Desktop & Quét Phần Cứng Thực Tế
- Hoạt động độc lập như một ứng dụng Windows Native thực thụ (tích hợp khay hệ thống System Tray, theo dõi tiến trình game thời gian thực).
- Tự động nhận diện chính xác cấu hình máy tính đang sử dụng (`Hostname`, `Windows Build`, `CPU`, `GPU`, `RAM`, `Local IP`).

### 2. 🔍 Tự Động Nhận Diện Game & Quét Chính Xác Vị Trí File Save
- **Quét Thư Mục Game Thông Minh:** Chỉ cần chọn thư mục chứa game hoặc thư viện game, ứng dụng sẽ tự động dò tệp thực thi `.exe`, trích xuất phiên bản thực tế từ PE Binary Header / `steam_appid.txt` / `.acf` manifest, và nhận diện đầy đủ thông tin game từ cơ sở dữ liệu Steam & PCGamingWiki.
- **Dò Tìm File Save Đa Tầng (Deep Save Discovery):** Tự động quét chính xác vị trí lưu file save trên hệ thống (`%LOCALAPPDATA%`, `%APPDATA%`, `%USERPROFILE%\Saved Games`, `Documents`, `Steam\userdata`, Goldberg, RUNE) cho bất kỳ tựa game nào (*Black Myth: Wukong, Elden Ring, Cyberpunk 2077, Baldur's Gate 3, Clair Obscur: Expedition 33, Red Dead Redemption 2, v.v.*).

### 3. ☁️ Tự Động Đồng Bộ 2 Chiều Qua Google Drive & Mã Hóa AES-256-GCM
- Tự động sao lưu tiến trình chơi game lên Google Drive cá nhân ngay khi bạn đóng game.
- Hỗ trợ mã hóa dữ liệu Save chuẩn **AES-256-GCM** và cơ chế **Safe Snapshot** dự phòng bất biến, cho phép khôi phục lại bất kỳ mốc thời gian nào chỉ với 1 cú nhấp chuột.

### 4. 🔄 Tự Động Nhận Diện & Cập Nhật Phiên Bản Mới (Live Auto-Update)
- Ứng dụng tự động kiểm tra phiên bản chính thức mới nhất từ máy chủ & GitHub Releases.
- Khi có bản cập nhật mới, ứng dụng hiển thị thông báo trực tiếp và hỗ trợ tải về + nâng cấp tự động ngay trong ứng dụng.

---

## 📂 Cấu Trúc Thư Mục Phát Hành Chính Thức

```
CloudSave-Sync/
├── 📁 02_User_Official_Release/
│   ├── 📁 github-release/
│   │   ├── RELEASE_NOTES.md                  # Ghi chú phát hành & hướng dẫn tải bộ cài .exe
│   │   └── SHA256SUMS.txt                    # Mã băm kiểm tra toàn vẹn bộ cài đặt
│   ├── production_release.json               # Manifest phiên bản chính thức phục vụ Auto-Update
│   └── HUONG_DAN_CAI_DAT_VA_SU_DUNG.txt      # Cẩm nang hướng dẫn sử dụng chi tiết tiếng Việt
└── 📄 README.md                              # Trang giới thiệu dành cho người dùng
```

---

## 💻 Yêu Cầu Hệ Thống

- **Hệ điều hành:** Windows 10 (Build 19041 trở lên) hoặc Windows 11 (64-bit).
- **RAM:** Tối thiểu 4 GB (Khuyên dùng 8 GB trở lên).
- **Dung lượng ổ đĩa:** 250 MB trống cho ứng dụng và kho lưu trữ Snapshot dự phòng.
- **Kết nối mạng:** Kết nối Internet để đồng bộ Google Drive và nhận bản cập nhật tự động.

---

## 📄 Bản Quyền

Phát triển bởi **Đỗ Minh Nguyên Studio**. Phân phối chính thức dành cho người dùng cuối.
