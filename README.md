# Freebuff Android wrapper (unofficial)

This project builds an installable Android APK that opens the official Freebuff web service in an Android WebView.

**This is an unofficial WebView wrapper, not a native port of Freebuff.** It does not bundle the Freebuff agent or bypass its account, regional, service, or usage restrictions.

## Build with GitHub Actions

1. Open the repository's **Actions** tab and enable Actions if prompted.
2. Run **Build Android APK** using **Run workflow**.
3. When the run succeeds, open the run and download the `freebuff-android-debug-apk` artifact.
4. Extract the ZIP and install `app-debug.apk` on your Android phone. Android may ask you to allow installs from the app used to download it.

The workflow also runs on pushes that change this project.

## Important limitations

- The APK is a debug build, suitable for personal testing, not a Play Store release.
- The app loads `https://freebuff.com/chat` in a WebView. Login, OAuth, file uploads, popups, downloads, and browser-specific features may need extra work or may not work in WebView.
- External links are opened in the system browser.
- No credentials or API keys are embedded in this project.
- Review the Freebuff privacy policy: https://freebuff.com/privacy-policy
