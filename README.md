# Streaks – habit tracker

Data is saved on-device (survives restarts). Summary tab shows completion %, streaks and per-habit bars for 7 days / 30 days / 1 year.

## Get the APK (no Android Studio needed)
1. Create a new GitHub repo and upload everything in this folder (keep the .github folder).
2. Open the repo's **Actions** tab → **Build APK** → wait ~4 minutes.
3. Open the finished run, download the **streaks-apk** artifact, unzip it.
4. Copy app-debug.apk to your phone, tap it, allow "Install unknown apps" when asked.

## Or build locally
Needs Node 20, JDK 17, Android SDK:
    npm install && npx cap add android && npx cap sync android
    cd android && ./gradlew assembleDebug
APK: android/app/build/outputs/apk/debug/app-debug.apk
