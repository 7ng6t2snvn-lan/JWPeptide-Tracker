# Shot Tracker v6.3.0

## What's Fixed

✅ **Calculator Bug Fixed**: All syringes now correctly calculate at 0.01ml/unit (100 units/ml)
✅ **Version Updated**: 6.2.2 → 6.3.0
✅ **Build Date Updated**: January 11, 2026

## Your Data is 100% SAFE

Your schedules, inventory, and logs are stored in browser localStorage.
They will **automatically** persist when you upload these new files!

The app will auto-migrate your data when it loads.

---

## Installation (Simple - 3 steps)

### Step 1: Upload to GitHub
Upload these 3 files to your GitHub Pages repository:
- `index.html` (replaces your current one)
- `sw.js` (replaces your current one)
- `manifest.json` (replaces your current one)

### Step 2: Commit & Push
Commit with message: "Update to v6.3.0 - fix calculator bug"

### Step 3: Force Refresh PWA
On your device:
1. Open https://7ng6t2snvn-lan.github.io
2. Force refresh (pull down to refresh OR close/reopen app)
3. Check version shows: v6.3.0

---

## What Changed

### Calculator Fix
**Before (v6.2.2 - WRONG):**
```javascript
const volumeUnits = volumeMl * syringeInfo.totalUnits;
```

**After (v6.3.0 - CORRECT):**
```javascript
const volumeUnits = volumeMl * 100;
```

This ensures all syringes (1cc, 0.5cc, 0.3cc) correctly calculate units at the standard 0.01ml per unit rate.

### Example
- 10mg peptide in 2ml BAC water
- 250mcg desired dose
- **v6.2.2 Bug**: 1cc showed 5 units (WRONG)
- **v6.3.0 Fixed**: 1cc shows 50 units (CORRECT)

---

## Files in This Package

- **index.html** - Your complete app with the fix applied
- **sw.js** - Service worker (cache version updated to 6.3.0)
- **manifest.json** - App manifest (ready to use)
- **README.md** - This file

---

## Need Help?

If you have any issues:
1. Check that all 3 files uploaded successfully
2. Clear your browser cache
3. Force refresh the PWA
4. Check the app shows v6.3.0 in the header

Your data (schedules, inventory, logs) is stored locally in your browser and will NOT be affected by this update.

---

**Version**: 6.3.0  
**Build Date**: 2026-01-11  
**Previous Version**: 6.2.2
