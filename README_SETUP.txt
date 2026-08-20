TRIPKIRA DOWNLOAD PORTAL SETUP
==============================

Recommended structure:
QR -> permanent TripKIRA download webpage -> GitHub Release APK.

1. CREATE GITHUB REPOSITORY
- Sign in to GitHub.
- Create a public repository, for example: tripkira-download
- Upload: index.html, style.css, config.js, app.js, tripkira_banner.png, tripkira_icon.png
- Commit.

2. ENABLE GITHUB PAGES
- Repository -> Settings -> Pages
- Source: Deploy from a branch
- Branch: main
- Folder: /(root)
- Save
- GitHub will give a Pages URL similar to:
  https://YOURNAME.github.io/tripkira-download/

The QR on the page automatically points to the page URL, so it stays permanent.

3. UPLOAD YOUR APK AS A GITHUB RELEASE
- Build your SIGNED TripKIRA v3.31 APK.
- Rename it: TripKIRA-v3.31.apk
- Repository -> Releases -> Draft a new release
- Tag: v3.31
- Upload TripKIRA-v3.31.apk
- Publish.

4. CONNECT THE DOWNLOAD BUTTON
- Open the published release.
- Copy the APK asset link.
- Edit config.js.
- Replace:
  PASTE_DIRECT_APK_DOWNLOAD_URL_HERE
  with the APK asset URL.
- Commit.

5. DRIVER INSTALLATION
- Scan QR.
- Open TripKIRA download page.
- Tap DOWNLOAD TRIPKIRA.
- Open the APK.
- Allow installation from this source if Android asks.
- Tap Install.

6. FUTURE VERSION
For v3.32:
- Build with the SAME signing key/keystore.
- Upload TripKIRA-v3.32.apk to a new GitHub Release.
- Change only version/apkFileName/apkUrl in config.js.
- Keep the same GitHub Pages URL.
- The QR does NOT need to change.

IMPORTANT
- The APK must be signed.
- Keep your Android signing keystore safe.
- Use the same signing key for all future TripKIRA updates.
