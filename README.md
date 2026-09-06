# FilmoScope Support Site

Public support / privacy / developer page for App Store and Google Play submission.

This folder is **outside** the FilmoScope app project so it is not bundled when you build or publish the app.

## What’s here

| File | Purpose |
|------|---------|
| `index.html` | Main page: about, how-to video, privacy, developer, support |
| `assets/` | App logo and icon |

## Before you publish

1. Add a demo video under **How to use** (comments in `index.html` show YouTube embed or `assets/demo.mp4`).
2. Support email is set to `poemcode.c@gmail.com`.

## Publish on GitHub Pages

On a machine with Git and GitHub CLI:

```bash
cd "C:\Users\cc_wi\Documents\C\App Project\FilmoScope-Support-Site"
git init
git add .
git commit -m "Add FilmoScope support and privacy page"
gh repo create FilmoScope-Support --public --source=. --remote=origin --push
```

Then in the GitHub repo: **Settings → Pages → Source: Deploy from a branch → `main` / root**.

Your URLs will look like:

- Support / home: `https://YOUR_USERNAME.github.io/FilmoScope-Support/`
- Privacy (same page): `https://YOUR_USERNAME.github.io/FilmoScope-Support/#privacy`
- How-to video: `https://YOUR_USERNAME.github.io/FilmoScope-Support/#guide`

Use those links in App Store Connect and Google Play Console.

## Preview locally

Open `index.html` in Chrome or Edge (double-click, or right-click → Open with).
