# Denge: update notes

- The app is developed as a claude.ai artifact (single HTML file). This repo hosts the installable PWA build on GitHub Pages: https://tirsphone.github.io/denge/
- On every artifact update, rebuild `index.html` from the artifact HTML: add the `<head>` block (charset, viewport, theme-color, manifest, icons, apple meta) before `<title>`, close `</head><body>` after the first `</style>`, and append the service-worker registration script before `</body>`.
- Change the `VERSION` string in `sw.js` on every release so the old cache is dropped.
- `index.html` is fetched network-first, so installed phones pick up the new version on the next online launch.
- Never commit user data; data lives in the phone's localStorage (`pd.*` keys).
- Talk to the owner in Turkish.
