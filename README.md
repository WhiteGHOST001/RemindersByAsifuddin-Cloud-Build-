# Reminders by Asifuddin

An Android-native reminders starter app inspired by the supplied Apple Reminders screenshots. Includes dashboard tiles, list/category navigation, local reminder storage, add/edit/delete/complete actions, date/time alarms, notification channel, urgent/flagged markers, and Asifuddin branding.

## Build the APK
1. Install Android Studio (current stable) and Android SDK Platform 35.
2. Open this folder in Android Studio.
3. Allow Gradle sync to finish.
4. Choose **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
5. Android Studio will show the generated APK location (usually `app/build/outputs/apk/debug/app-debug.apk`).

## Notes
- This project source has not been compiled in this environment because Android SDK/Gradle are not installed here.
- On Android 13+, allow notification permission when prompted.
- Exact alarm behavior depends on Android version and device settings. Some devices may require enabling alarms/reminders in system settings.
- Android does not provide a universal Apple Dynamic Island API. The app uses high-priority Android notifications; compatible devices or third-party island apps may present them in a pill/overlay.
- This is an original Android implementation inspired by the reference images, not Apple's proprietary source code or a pixel-perfect iOS clone.

## Build in the cloud (for laptops with 8 GB RAM)
This project includes `.github/workflows/build-apk.yml`. You can build the APK on GitHub's hosted runner instead of installing Android Studio locally:
1. Create a GitHub repository and upload the **contents** of this project folder (including the hidden `.github` folder).
2. Open the repository's **Actions** tab and select **Build Android APK**.
3. Click **Run workflow** (or push to `main` to trigger it automatically).
4. When the run succeeds, open the run's **Artifacts** section and download `RemindersByAsifuddin-debug-apk`.
5. Extract the downloaded artifact and install the APK on your Android phone. You may need to allow installing apps from your browser/file manager.

GitHub account limits and workflow availability can vary. This workflow builds a debug APK; it is not a signed Play Store release.
