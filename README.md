# Big Shiny Rounds

Cleaning rounds that run in your browser. It's part of the Big apps, alongside [Big Minty Finances](https://github.com/dontdoubtdusty/budget), [Big Saucy Recipes](https://github.com/dontdoubtdusty/cooking), [Big Skinny Health](https://github.com/dontdoubtdusty/diet), [Big Tidy Reminders](https://github.com/dontdoubtdusty/reminders) and [Big Healthy Habits](https://github.com/dontdoubtdusty/habits). You can also open it inside [Big Juicy Suite](https://github.com/dontdoubtdusty/suite), which holds all the Big apps in one place. It's one file (`index.html`) with no build step and no server.

## Features

- More than one property: tap the property name at the top to switch or add one. Each has its own floors, areas, tasks, supplies and history.
- Your building set up as floors and areas, in the order you walk them. Tap **Edit area** on any area's checklist in Rounds to change it right there, and the back button takes you straight back to where you were.
- A map of each floor (Rounds > Map): every room is drawn where it sits in real life, colored by what's left to do. Tap one for its checklist. Lay it out under Setup > Edit map on a pegboard 12 pegs across: drag rooms onto the pegs (drop one on another to swap them), drag a corner peg to resize, make L-shaped rooms, and add labels like Entrance or Closet.
- Sub areas: split an area into parts with their own checklists, like a hallway and each of four offices (Setup > the area > Sub areas). Each sub area gets the standard tasks and its own extras, and a new one starts with a copy of the last one's tasks. On Rounds they show together under the area, each with its own heading and "All done" button; on the map the area stays one room.
- One standard task set (sweep, mop, dust, windows and door glass) that every area gets, with per-area extras and the option to turn a standard task off in a specific area. How often each standard task is done is set per area (Setup > the area), so the lobby can be mopped daily while a study lounge is mopped weekly. New areas start with them all daily.
- Each task has a frequency: daily, weekly, monthly or as needed. Rounds only shows what's due, and the card at the top of Today and Rounds counts what's still due and what you've done today.
- Each task can also have a time of day: anytime, early (like mopping) or later (like vacuuming). It's set per area next to how often, the same way. Early tasks come first in each area's checklist and later ones last, with a small tag. After the time early tasks should be done by (Settings, 12pm to start), any early task still due gets an orange tag. It never hides a task or changes what's due.
- Long-press any task on Rounds to remove tasks without opening the area: tap more tasks (in any area) to add them, then **Remove**. A standard task is switched off in that area and an extra task is deleted; history keeps their names, and **Undo** puts them all back.
- Plain water mop: turn it on under **Setup > Standard tasks** and set how often (every 4 mops to start). Any task with "mop" in its name counts, and each area counts its own mops. That time, the mop task shows a Plain water tag on Rounds, and the history, summary and printed report say "Mop (plain water)".
- Every task you check off is stamped with the date and time
- One-time tasks for anything you're asked to do once that isn't part of an area ("move boxes out of the lobby"). Add them on Today; they also show on Rounds until they're done. Checking one off stamps it with the time, adds it to History and the printed report, and you can add a note to it like any other task. Tap the calendar icon to give one an optional due day and time: dated ones sort to the top, and overdue ones turn red.
- Tours: when someone is being shown a unit, add a tour on Today with the area, day, time and an optional label like "Unit 312". The area gets a tour badge with the time on its Rounds checklist and on the floor map, so you know to steer clear or have it ready. Tours can be edited or deleted, and drop off once their day has passed.
- End of the day: tap **Clock out** at the bottom of Today when you're done working, or **Day off** when you're not working today. The card at the top of Today and Rounds then says you're done instead of counting what's due, and the Shiny card in Big Juicy Suite goes quiet too. It clears itself the next morning, and **Clock back in** (or Undo) takes it back. Anything you didn't get to stays due for tomorrow.
- Wet floor signs: tap **Wet floor sign** on an area's checklist in Rounds when you put one out. The area gets a sign badge on Rounds and on the floor map, and Today lists every sign still out with when it went out, so you remember to pick them up. Tap **Picked up** (or **Picked up sign** on the checklist) to clear it, with Undo.
- **Mark clean** on any area's checklist: done with an area but didn't need to do everything (no trash to take out)? Check what you did, then tap Mark clean. Only the checked tasks go in the history as done, with one "Area marked clean" entry. The Log tab lists what was skipped under it; the printed report and shared summary show just "Area marked clean", and the rest stop being due until tomorrow (weekly and monthly ones come back tomorrow, since they weren't done). Undo from the toast, or delete the entry in the Log.
- An optional note on any area (where the key is, which closet has the mop sink), shown at the top of that area's checklist on Rounds. Add it from the area's checklist or under Setup.
- Notes on any completed task ("out of soap", "light out by the door")
- Overdue weekly and monthly tasks show on Today
- History of everything you've done, with a **Print report** button that gives a clean page for a supervisor (or Save as PDF from the print screen)
- Share a plain-text summary of what got done (grouped by floor and area, with notes) by text or email: **Share today's summary** on Today, or **Share** on the Log tab for any date range. Where sharing isn't available it's copied instead.
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
