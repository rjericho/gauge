# Gauge, home-screen build

Everything in this folder is the finished app. Put the folder on any static web host and open its address in Safari on the iPhone, then Share → Add to Home Screen. After the first visit it opens with no signal.

## Hosting

This repository is hosted with GitHub Pages at https://rjericho.github.io/gauge/. Settings → Pages has its source set to GitHub Actions, and the workflow in `.github/workflows/pages.yml` publishes every push to `main` within a minute or two.

On the iPhone, open the address in Safari, tap Share, then Add to Home Screen.

## Updating

Push a newer `index.html` to `main`. Phones pick up the new version the next time they open the app with a connection.

## What is in here

- `index.html` is the whole app.
- `pdf.min.js` and `pdf.worker.min.js` read PDFs on the phone (Mozilla's pdf.js, Apache 2.0).
- `sw.js` keeps a copy of the app on the phone for offline use.
- `manifest.webmanifest` and the icons make it install like an app.
