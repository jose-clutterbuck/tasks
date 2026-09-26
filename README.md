# tasks
Personal Task Schedule System 

A personal task planner built as a single offline web app, made to be installed on an iPhone home screen from GitHub Pages. One person, one device, no account, no server. Everything you enter lives in your browser's local database and never leaves the phone.
 
Current version: 3.6
 
## What it does
 
**Plan.** The home tab builds your day for you. It ranks every open task live from the clock (how close the due date is and how much work is left), the stakes you set, whether other work waits on it, and how long it has sat untouched. Today fills to the hours you actually have left, not a fixed count. You can view Today, Tomorrow, or the whole week, each as a timeline Schedule or a List, and dragging tasks in the List reorders the Schedule too. Tasks with a due date show a thin red due pin at the exact time they are due, plus one full length work block on the day the planner or your aim picked.
 
**Capture.** The plus button opens a short set of questions, one page at a time, with Back, Skip, and Next. It asks only what fits the thing you are adding: a to do, an event like a class, a time block like a commute, a background thing like laundry, a project, or a saved template. Typing shorthand in the title works too, like `essay draft friday 4pm ~1h #School @computer`.
 
**Timing that matches real life.** A task can have a due date, a day or stretch you aim to do it in, a date it opens up (like an assignment that unlocks a week before it is due), and a time of day it should land in. Events and blocks can repeat on chosen weekdays, on a day of the month, on something like the second Tuesday, or yearly, and can end on a date or after a set number of times. Sleep and unavailable time are subtracted automatically.
 
**Everything else.** Nested groups, categories with their own colors and icons (36 swatches plus a full color mixer), stakes instead of an importance rating, deep focus windows, dependencies, templates with dates stored as offsets, a calendar with month, week, and day views, weekly and monthly reviews, automatic snapshots, and full export to JSON, Markdown, CSV, or a calendar file with alerts.

## IMPORTANT

Be sure to export backups regularly to your local file storage to ensure your data can be retrieved and easily imported back into the web app in the case you delete the home screen app. 

My recommended backup steps:
1. Go to Settings >
2. Data section >
3. Export and import >
4. Selecting "Full backup (JSON)"
5. Save to dedicated storage folder in your iPhone file manager

My recommended import steps:
1. Go to Settings >
2. Data section >
3. Export and import >
4. Selecting "Import a JSON backup"
5. Select ONLY the JSON file the backup created. No need for the TXT file.
6. Press "Ok"

## Files
 
- `index.html` — the whole app
- `sw.js` — the offline cache (bump `CACHE` when deploying a new build)
- `manifest.json` — home screen install settings
- `icon.svg` — the app icon
## Install on iPhone
 
1. Host these four files on GitHub Pages.
2. Open the page in Safari.
3. Share, then Add to Home Screen.
It works fully offline after the first load. When a new version is deployed, the app picks it up on its next open with a connection.
 
## Privacy
 
There is no backend. Data is stored in IndexedDB on the device. The service worker caches only the app files, never your data. Backups are files you export yourself.
