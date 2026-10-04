# Gauge, home-screen build

Everything in this folder is the finished app. Put the folder on any static web host and open its address in Safari on the iPhone, then Share → Add to Home Screen. After the first visit it opens with no signal.

## Free hosting on GitHub Pages

1. Sign in at github.com and create a new repository called `gauge`. Public is fine; the app holds no data of its own, every project stays on the phone.
2. Upload every file in this folder to the repository (Add file → Upload files). Keep the names exactly as they are.
3. In the repository, open Settings → Pages. Under Build and deployment choose "Deploy from a branch", pick `main` and `/ (root)`, and save.
4. In a minute or two the page reports the address, normally `https://<your-username>.github.io/gauge/`.
5. On the iPhone, open that address in Safari, tap Share, then Add to Home Screen.

## Updating

Replace `index.html` in the repository with a newer one. Phones pick up the new version the next time they open the app with a connection.

## What is in here

- `index.html` is the whole app.
- `pdf.min.js` and `pdf.worker.min.js` read PDFs on the phone (Mozilla's pdf.js, Apache 2.0).
- `sw.js` keeps a copy of the app on the phone for offline use.
- `manifest.webmanifest` and the icons make it install like an app.
