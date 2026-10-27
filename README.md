# New Again — gratitude journal

A small, free, private, installable iPhone PWA. No account, API key, backend, build step, or subscription.

## Features
- Save three gratitude items per day; drafts save as you type.
- Local similarity warnings (not an AI semantic model). Modes: relaxed, balanced, strict.
- Streaks, history, search, basic insights.
- JSON export/import and data deletion.
- Offline use after loading once while online.

## Publish for free via GitHub Pages
1. Create a new **public** GitHub repository, e.g. `new-again`.
2. Upload the contents of this folder to the repository root: `index.html`, `manifest.webmanifest`, `sw.js`, and the `icons` folder. (Do not upload just the .zip.)
3. In GitHub repository **Settings → Pages**, select **Deploy from a branch**, `main`, `/ (root)`, and Save.
4. Visit the HTTPS Pages URL given by GitHub, e.g. `https://YOURNAME.github.io/new-again/`.
5. Open the URL in **Safari on iPhone**. Tap **Share → Add to Home Screen → Add**.
6. Open your installed app from the home screen once while online; afterward, it works offline.

## Privacy / limits
Your journal is saved in your browser's localStorage, on the device. It does **not** sync between browsers or devices. Website data can be cleared by iOS or the user: export backups regularly. If you use the PWA and Safari separately, they may not share the same local data. The matching algorithm is deliberately lightweight and can miss paraphrases or flag related but different entries. There are no notifications yet. Edit history is not yet supported (today's entries are editable).

## Testing on a computer
From this folder, run `python3 -m http.server 8000`, then open `http://localhost:8000`. Service workers work at localhost. Install on iPhone requires an HTTPS-hosted URL.
