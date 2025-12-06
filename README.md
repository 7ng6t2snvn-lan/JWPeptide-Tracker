# Shot Tracker v3.0.0

A mobile-friendly PWA for tracking peptide doses and schedules.

## What's New in v3.0.0

- **Error Boundary**: App now shows a friendly error screen instead of blank page if something crashes
- **Force Refresh**: New button in Settings to clear cache and reload
- **Auto-Update Detection**: PWA prompts you when a new version is available
- **Network-First Caching**: Always tries to fetch fresh content first
- **Version Display**: Shows current version in the header

## Features

- 📅 Daily dose tracking with calendar view
- 💉 Reconstitution calculator with visual syringe
- 📊 97 peptide database with dosing info
- 🏪 Top 10 peptide vendor rankings
- 🔒 PIN protection (default: 0119)
- 📱 Works offline as PWA
- 💾 Local storage persistence
- 📤 Export/import data backups
- 🔄 Force refresh option for PWA updates

## Deploy to GitHub Pages

1. Create a new GitHub repo
2. Upload all files (including `.nojekyll`)
3. Go to **Settings** → **Pages**
4. Source: **main** branch, **/ (root)**
5. Save — your site will be live at `https://yourusername.github.io/repo-name/`

## Files

- `index.html` — Main app (self-contained React app)
- `sw.js` — Service worker for offline support and caching
- `manifest.json` — PWA manifest
- `icon-192.png` — App icon (192x192)
- `icon-512.png` — App icon (512x512)
- `.nojekyll` — Prevents Jekyll processing on GitHub Pages

## Usage

1. Open the app and enter PIN: **0119**
2. View/manage schedules in the **Schedules** tab
3. Log doses in the **Today** tab
4. Use the **Calc** tab for reconstitution math
5. Browse peptides in the **Database** tab
6. Toggle between **💊 Peptides** and **🏪 Vendors** in Database

## Add to Home Screen (iOS)

1. Open in Safari
2. Tap Share button
3. Tap "Add to Home Screen"
4. Name it and tap Add

## PWA Updates

When you deploy a new version:
1. The app will detect the update
2. You'll see a prompt to reload
3. If you have issues, use **Settings → Force Refresh App**

## Data

All data is stored locally in your browser's localStorage. Use Export/Import in Settings to backup your data.

## Troubleshooting

**Blank screen after PIN?**
1. Try Settings → Force Refresh App
2. If that doesn't work, try Settings → Clear All Data (warning: loses your data!)
3. Delete the app from home screen and re-add it

**PWA not updating?**
1. Delete the app from home screen
2. Clear Safari website data for this site
3. Re-add to home screen
