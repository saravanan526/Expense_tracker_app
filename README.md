# Expense Tracker (Android)
Web app wrapped as a native Android app with Capacitor. Data is saved on-device (local storage), works offline.

## Get the APK (no Android Studio needed)
1. Create a free GitHub account and a new repository.
2. Upload all files of this folder (keep the .github/workflows folder).
3. Open the repo -> Actions -> "Build APK" -> wait ~5 min (or Run workflow).
4. Open the finished run -> Artifacts -> download "expense-tracker-apk" (zip) -> extract app-debug.apk.

## Install on phone
1. Copy app-debug.apk to your phone and tap it.
2. Allow "Install unknown apps" for your file manager/browser when asked.
3. Open "Expense Tracker".

## Build locally instead
npm install && npx cap add android && npx cap sync android
cd android && ./gradlew assembleDebug
APK: android/app/build/outputs/apk/debug/app-debug.apk
(Needs Node 20+, JDK 21, Android SDK.)

## Edit the app
All app code is in www/index.html. Re-run the build after changes.
