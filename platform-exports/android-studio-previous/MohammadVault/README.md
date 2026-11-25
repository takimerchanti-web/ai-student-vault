# Mohammad Vault – Android Studio Project

## How to build the APK

### Requirements
- Android Studio (Hedgehog or newer)
- JDK 11 or newer (bundled with Android Studio)

### Steps

1. **Extract** this ZIP anywhere on your PC/Mac.
2. **Open** Android Studio → **Open an existing project** → select the extracted `MohammadVault` folder.
3. Android Studio will automatically download Gradle and all dependencies (internet required, ~2–3 min first time).
4. Wait for the Gradle sync to finish (bottom status bar says "Gradle sync finished").

### Build a debug APK (easiest, for testing)
- Menu → **Build → Build Bundle(s) / APK(s) → Build APK(s)**
- The APK will be at: `app/build/outputs/apk/debug/app-debug.apk`
- Click **"locate"** in the popup to find it.

### Install on your Android phone
- Enable **Developer Options** on your phone → enable **USB Debugging** or **Install via USB**
- OR: copy the `app-debug.apk` to your phone and open it (enable "Install from unknown sources" if prompted)

### Build a release APK (for sharing / sideloading)
- Menu → **Build → Generate Signed Bundle / APK → APK**
- Create a keystore (one-time) → fill in details → build
- Output: `app/build/outputs/apk/release/app-release.apk`

## What's inside
- Your full **Mohammad Vault** app (`index.html`, ~225 KB) runs inside an Android WebView
- Full offline support via IndexedDB
- Camera, file picker, and external-link permissions included
- Works on Android 5.0+ (API 21+)

## Package name
`com.mohammadvault.app` — change it in `app/build.gradle` if needed.
