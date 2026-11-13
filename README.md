# Pickup Hoops Tracker (installable web app)

Courtside organizer for pickup basketball. Runs fully on the phone, works offline, no account.

## Files

- `index.html` – the whole app
- `sw.js` – keeps a copy on the phone so it opens without internet
- `manifest.webmanifest`, `icons/` – name and icon for the home screen
- `.nojekyll` – tells GitHub Pages to serve the files as they are

## Put it on GitHub Pages

1. Create a new **public** repository on GitHub, for example `pickup-hoops`.
2. Upload everything in this folder to the repository root (keep the `icons` folder).
3. Repository **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, folder `/ (root)`. Save.
4. After a minute the app is at `https://<your-username>.github.io/pickup-hoops/`.

## Install on a phone

- **Android (Chrome):** open the link, menu ⋮ → *Install app* (or *Add to Home screen*).
- **iPhone (Safari):** open the link, Share → *Add to Home Screen*.

Open it once while online. After that it also opens with no connection.

## Updating

Replace `index.html`, and change `VERSION` in `sw.js` (for example `pickup-hoops-v2`).
Phones pick up the new version the next time they open the app while online.

## Data

Everything is stored on the phone only. Use **History → Backup → Save backup file**
after each session, and **Restore from file** to load it on another phone.
