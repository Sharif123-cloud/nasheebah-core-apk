# Nasheebah Core — Android APK

**School Report Card System v2.0**  
Engineered with obsession by **Sserunjogi Sharif** 📞 +256787816686

---

## 📱 About

Nasheebah Core is a complete school report card management system wrapped in a native Android WebView. It supports:

- O-Level (Senior 1–4) and A-Level (Senior 5–6) report cards
- Multi-class, multi-subject, multi-student management
- CA + EOT marks entry with automatic grade computation
- PDF report generation (downloadable per student or class-wide)
- Badge/logo upload for your school
- All data stored locally on-device (localStorage)

## 🔨 Building the APK

### Via GitHub Actions (Recommended)

1. Push to `main` branch (or trigger manually from **Actions** tab)
2. GitHub Actions will automatically build the debug APK
3. Download from **Actions → latest run → Artifacts → nasheebah-core-debug**

### Manual Build

```bash
# Requirements: JDK 17, Android SDK (ANDROID_HOME set)
./gradlew assembleDebug
# Output: app/build/outputs/apk/debug/app-debug.apk
```

## 📦 Project Structure

```
nasheebah-core-apk/
├── app/
│   └── src/main/
│       ├── assets/index.html          ← Full web app
│       ├── java/com/nasheebah/core/
│       │   └── MainActivity.java      ← WebView wrapper
│       └── res/                       ← Android resources
├── .github/workflows/build-apk.yml   ← CI/CD workflow
└── build.gradle                      ← Gradle config
```

## 📜 Workflow Settings

- **Trigger:** Push to `main` + manual dispatch
- **Java:** 17 (Temurin)
- **Gradle:** 8.4 via wrapper
- **Build type:** Debug (ready to install)
- **Artifact retention:** 30 days

## 🔒 Terms

See in-app Terms & Conditions. Contact: +256787816686
