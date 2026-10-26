# Scoia'tael Media Player — GitHub Pages App

A single-page media player packaged for GitHub Pages, with installable PWA metadata, icons, offline shell caching, cinematic wallpaper, and a media import picker.

## Deploy to GitHub Pages
1. Extract this ZIP.
2. Upload the **contents** of `Scoiatael_GitHub_App` to the root of a GitHub repository.
3. In **Settings → Pages**, choose **Deploy from a branch**, select your main branch and `/(root)`, then save.
4. Open the published HTTPS Pages URL on your phone. Use your browser menu to install/add it to the home screen.

## Grant access to media
Open the app's **Settings → Grant access: photos, audio & videos**. The Android/browser file picker lets you choose media files to import. You can also use the separate Add songs, Add videos, and folder-scan options.

Web apps cannot request unrestricted Android storage permission like native apps. The browser only gives the app access to files/folders you select. Folder scanning and remembered folder access depend on browser support.

## Important metadata limitation
The tag editor stores the edited title/artist/album/keywords/details in the app's own library database. It does **not** rewrite embedded ID3 tags in original audio files or EXIF/IPTC metadata inside original photos. Editing the original embedded metadata requires a native Android app or a dedicated metadata-writing implementation. The app does not upload your selected media to a server; imported media is handled locally by the browser and stored in the app's browser database where supported.


## DIY theme creator

Open **Settings → Themes & colors → Create a DIY theme** to create a theme without editing or creating another HTML file. Choose a name, accent color, icon, animated effect, six tab labels, and the empty-library message. Custom themes are saved in this browser's local storage.

Use **Export my DIY themes (JSON)** to back them up or move them to another browser/device. On the other installation, use **Import DIY themes (JSON)**. The imported themes work with this DIY-enabled player; the theme JSON does not contain or replace the HTML app itself. If browser data is cleared, import your JSON backup to restore themes.
