# StudyPlay PWA (offline + ads-free)

## Files
- `index.html`: the StudyPlay quiz app
- `manifest.webmanifest`: install name, colors, and icons
- `sw.js`: offline caching service worker
- `icon-192.png` and `icon-512.png`: app icons

## Publish on GitHub Pages (phone-friendly)
1. Extract this ZIP on your phone.
2. Open your public GitHub repository named `studyplay` (or use your existing repository).
3. Upload the files to the repository root. Keep the filenames exactly as shown. `index.html` must be at the root.
4. Commit the uploaded files.
5. In repository Settings → Pages, choose `Deploy from a branch`, branch `main`, folder `/(root)`, then Save.
6. Wait for deployment. Open the published site in Chrome while online and wait for it to finish loading once.
7. Test it: open the quiz, then turn off Wi-Fi and mobile data and reload/reopen the installed app.
8. In Chrome menu, choose `Add to Home screen` or `Install app` if offered.

## Important
- The first visit needs internet so the browser can download and cache the files.
- The service worker requires HTTPS; GitHub Pages provides HTTPS.
- Public repositories expose source code publicly. Do not upload passwords, private information, or secret keys.
- This is a beta question bank; it does not yet cover every class/subject comprehensively.
- No ad network has been added. The app does not intentionally show ads.
- After changing app files, increment `CACHE_NAME` in `sw.js` (for example `studyplay-offline-v2`) to help devices fetch the new version.
