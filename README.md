# Big Shiny Rounds

Cleaning rounds that run in your browser. It's part of the Big apps, alongside [Big Minty Finances](https://github.com/dontdoubtdusty/budget), [Big Skinny Health](https://github.com/dontdoubtdusty/diet) and [Big Saucy Recipes](https://github.com/dontdoubtdusty/cooking). It's one file (`index.html`) with no build step and no server.

## Features

- Your building set up as floors and areas, in the order you walk them
- One standard task set (sweep, mop, dust, windows and door glass) that every area gets, with per-area extras and the option to turn a standard task off in a specific area
- Each task has a frequency: every round, daily, weekly, monthly or as needed. Rounds only shows what's due.
- Start and finish a round; every task you check off is stamped with the date and time
- Notes on any completed task ("out of soap", "light out by the door")
- Overdue weekly and monthly tasks show on Today
- History of everything you've done, with a **Print report** button that gives a clean page for a supervisor (or Save as PDF from the print screen)
- Supplies with counts, units, where they're kept, and a "running low" warning level
- History is kept for 3, 6 or 12 months (Settings), so storage never fills up
- Light, dark, automatic and Day/Night themes, haptics, backups, and optional sync across devices, all shared with the other Big apps

## Using it

Create a new repo (for example `rounds`), upload these files, then turn on GitHub Pages (**Settings → Pages → Deploy from a branch → `main` / root**) and open the link it gives you.

### Install it as an app

- **iPhone or iPad (Safari):** tap Share, then **Add to Home Screen**.
- **Android (Chrome):** tap the menu, then **Install app** (or **Add to Home screen**).

### Files

| File | What it does |
| --- | --- |
| `index.html` | The whole app |
| `sync.js` | Optional sync across devices (shared by all the Big apps) |
| `feedback.js` | Haptic ticks and button press feedback (shared by all the Big apps) |
| `manifest.webmanifest` | The app's name, colors and icons, used when it's installed |
| `sw.js` | Saves a copy of the app so it opens offline |
| `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | The app icon at each size browsers and phones ask for |
