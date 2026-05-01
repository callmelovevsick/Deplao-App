<div align="center">
  <img src="icon.png" width="100" alt="Dép Lào Logo" />
  <h1>🩴 Dép Lào Desktop</h1>
  <p>Ứng dụng Dép Lào Desktop — Chạy trên nhân Chrome (Chromium)</p>

  [![Release](https://img.shields.io/github/v/release/Tio-dev71/Deplao-App?style=flat-square)](https://github.com/Tio-dev71/Deplao-App/releases/latest)
  [![Windows](https://img.shields.io/badge/Windows-x64-blue?style=flat-square&logo=windows)](https://github.com/Tio-dev71/Deplao-App/releases/latest)
  [![Linux](https://img.shields.io/badge/Linux-x64-orange?style=flat-square&logo=linux)](https://github.com/Tio-dev71/Deplao-App/releases/latest)
  [![macOS](https://img.shields.io/badge/macOS-x64%20%7C%20arm64-lightgrey?style=flat-square&logo=apple)](https://github.com/Tio-dev71/Deplao-App/releases/latest)
</div>

---

## 📥 Tải về

Vào trang [**Releases**](https://github.com/Tio-dev71/Deplao-App/releases/latest) để tải bản mới nhất:

| Hệ điều hành | File | Ghi chú |
|---|---|---|
| 🪟 Windows | `*-Setup.exe` | Bản cài đặt |
| 🪟 Windows | `*-Portable.exe` | Bản portable |
| 🐧 Linux | `*.AppImage` | Chạy trực tiếp |
| 🐧 Linux | `*.deb` | Ubuntu / Debian |
| 🍎 macOS | `*.dmg` | Intel & Apple Silicon |

---

## 🛠️ Phát triển

### Yêu cầu
- Node.js 18+
- npm

### Cài đặt & chạy
```bash
git clone https://github.com/Tio-dev71/Deplao-App.git
cd Deplao-App
npm install
npm start
```

### Build thủ công
```bash
# Windows
npm run build:win

# Linux
npm run build:linux

# macOS
npm run build:mac

# Tất cả cùng lúc
npm run build:all
```

---

## 🚀 Tạo Release mới

1. Cập nhật `"version"` trong `package.json`
2. Commit và push lên `main`
3. Tạo tag và push:
   ```bash
   git tag v1.2.0
   git push origin v1.2.0
   ```
4. GitHub Actions tự động build cho **Windows**, **Linux**, **macOS** và đăng lên **Releases** ✅

> **Lưu ý:** Không cần cấu hình thêm secret — workflow dùng `GITHUB_TOKEN` có sẵn của GitHub.

---

## 📁 Cấu trúc project

```
Deplao-App/
├── .github/
│   └── workflows/
│       ├── release.yml   # Auto build + release khi push tag
│       └── build.yml     # Build thủ công theo platform
├── main.js
├── preload.js
├── renderer.js
├── index.html
├── custom_style.css
├── package.json
└── icon.png / icon.ico
```

---

## 📄 License

MIT © [Tio-dev71](https://github.com/Tio-dev71)
