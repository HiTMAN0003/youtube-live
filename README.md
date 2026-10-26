# Live Duo Android-installable web app

This package uses the uploaded `index.html` as the main page and adds the Progressive Web App (PWA) files needed for Chrome's **Install app / Add to Home screen** option.

## Publish to GitHub Pages

1. Open https://github.com/HiTMAN0003/youtube-live
2. Replace the repository-root `index.html` with this package's `index.html`.
3. Upload `manifest.webmanifest`, `sw.js`, and the `icons/` folder into the repository root.
4. In **Settings → Pages**, select **Deploy from a branch**, branch `main`, folder `/(root)`, then Save.
5. Open https://hitman0003.github.io/youtube-live/ in Chrome on Android. Use Chrome's ⋮ menu → **Install app** or **Add to Home screen**.

## Important

- This is an installable PWA, not a standalone APK.
- The web page must be served over HTTPS for service workers and PWA installation.
- Your uploaded page uses YouTube's embedded player/chat. Some streams may disallow embedding, and YouTube can change embed behavior.
- Watching/likes counts use the optional YouTube Data API key entered in the page. Keep in mind the API key is saved in this browser's local storage; don't put a private server secret in a public HTML file.
