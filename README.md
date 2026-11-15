# Chasing Shadows: The Apex Predator Expedition

A 3D snakehead (Channa) tank game for Android. Every push to `main` builds an APK with GitHub Actions and publishes it as a release.

## Get the APK

1. Create a new **public** repository on GitHub (for example `chasing-shadows`).
2. Upload everything in this folder, keeping the folder structure. On the repo page choose **Add file > Upload files** and drag all the files and folders in, including `.github`.
3. If `.github` does not upload by drag and drop, choose **Add file > Create new file**, name it `.github/workflows/build-apk.yml`, and paste in the contents of that file.
4. Open the **Actions** tab. The "Build APK" run takes a few minutes.
5. When it finishes, open **Releases** and download `chasing-shadows.apk`.

The download link never changes:

    https://github.com/YOUR-USERNAME/YOUR-REPO/releases/latest/download/chasing-shadows.apk

The in-game **Share** button shows a QR code for that link, filled in automatically during the build.

## Installing

Open the APK on the phone and allow "install unknown apps" when asked. Every build is signed with the same key (`app/debug.keystore`), so new versions install over the old one. That key is public in this repo, so treat the APK as a personal build, not a Play Store release.

## Where things are

- `app/src/main/assets/index.html` is the game. Edit this to change it.
- `index.html` in the repo root is the same game for browsers. Turn on GitHub Pages (Settings > Pages > Deploy from branch > main) to get a web link.
- `app/src/main/res/mipmap-*` holds the app icon.
