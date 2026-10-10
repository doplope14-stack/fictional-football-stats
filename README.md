# Fictional Football Stats — Android PWA

A mobile-first, installable web app inspired by football score/stat apps. It is an independent fan project, not affiliated with FotMob.

## Included
- Player creation/edit/delete and search
- Season stats with competition-by-competition appearances, goals and assists
- Career totals calculated from season stats
- International caps, goals and assists
- Market value, overall rating, nationality, club, position and notes
- Transfer history, awards and trophies
- Enter match results and auto-calculate league-style standings
- Compare two players
- JSON export/import backup
- Local browser storage and offline service worker
- Seed data for the fictional players whose details were already established

## Install on Android
A PWA must be served from an HTTPS website (or localhost) to be installable. Opening `index.html` as a local file is useful for a quick test, but browser install/offline features may not work in file mode.

### Easiest route: GitHub Pages
1. Create/sign into a GitHub account.
2. Create a new public repository, e.g. `fictional-football`.
3. Upload all files in this folder to the repository root.
4. Open repository **Settings → Pages**.
5. Under build/deployment, select **Deploy from a branch**, choose `main` and `/ (root)`, then Save.
6. Wait for GitHub Pages to provide the HTTPS site URL.
7. Open that URL in Chrome on Android.
8. Tap Chrome's three-dot menu → **Install app** or **Add to Home screen**.
9. Launch it from your home screen.

If you use a different static HTTPS host, upload the same files and open its HTTPS URL in Chrome.

## Important data note
Player data is stored locally in the browser/app origin. It does not sync between devices. Use **More → Backup & restore → Download backup** regularly. Keep a copy of the JSON file. Importing a backup replaces current app data.

## Seed-data accuracy
This demo preloads the known fictional player details available from the conversation. Any unconfirmed fields are placeholders or blank; review and edit them in the app. Some historical season totals were given as combined club + national-team totals, so they are not fabricated into a competition breakdown unless a breakdown was known. Enter missing seasons and competition stats yourself.

## Files
- `index.html`: the app
- `manifest.json`: installable app metadata
- `sw.js`: offline cache
- `icon-192.png`, `icon-512.png`: home-screen icons
