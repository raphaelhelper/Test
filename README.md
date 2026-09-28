# Word Popup Overlay

Ứng dụng Android giúp hiển thị cửa sổ từ vựng nổi (Overlay Popup) đè lên các ứng dụng khác, hỗ trợ học từ vựng trực quan và định kỳ.

---

## 🚀 Tính năng & Công nghệ
- **Overlay Window:** Hiển thị popup từ vựng floating đè lên ứng dụng khác (`SYSTEM_ALERT_WINDOW`).
- **Foreground Service:** Chạy ngầm ổn định để nhắc từ vựng theo thời gian đặt sẵn.
- **Gradle Kotlin DSL:** Cấu hình build hiện đại với Kotlin (`.gradle.kts`).
- **CI/CD Build Automation:** Tích hợp GitHub Actions tự động build ra file APK khi push code.

---

## 📁 Cấu trúc dự án

Dự án sử dụng script `setup_project.sh` để gom các file flat thành cấu trúc Android chuẩn:

```text
.
├── app/
│   ├── build.gradle.kts
│   └── src/
│       └── main/
│           ├── AndroidManifest.xml
│           ├── java/com/qui/wordpopup/
│           │   └── MainActivity.kt
│           └── res/
│               ├── drawable/popup_bg.xml
│               ├── layout/activity_main.xml
│               └── values/styles.xml
├── build.gradle.kts
├── settings.gradle.kts
├── setup_project.sh
└── .github/
    └── workflows/
        └── build.yml
