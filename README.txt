STUDY HUB - INSTALLABLE WEB APP
===============================
Files: index.html (the app), manifest.webmanifest (name, icons, colours),
sw.js (offline support), icons/ (app icons).

It must be served over https (or localhost) for installing and offline mode to work.
Opening index.html straight from your files will still run the app but will not install.

FREE WAYS TO PUT IT ONLINE (drag the whole folder, keep the files together)
- Netlify Drop: app.netlify.com/drop
- Cloudflare Pages, GitHub Pages or Vercel

AFTER IT IS ONLINE
- Android / Chrome / Edge: open the link, tap "Install app" (bottom right) or the browser's install icon.
- iPhone / iPad: open in Safari > Share > Add to Home Screen.
- Windows / Mac: Chrome or Edge address bar > Install icon.

TEST LOCALLY: in this folder run "python3 -m http.server 8000" and open http://localhost:8000

NOTES
- Saved decks live in each browser on each device. They do not sync yet (that needs a sign-in backend).
- After you change files, bump VERSION in sw.js so users get the update.
- PDF import and styling libraries load from the internet the first time; after that they are cached for offline use.
