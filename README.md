# My To-Do PWA

A simple personal Progressive Web App (PWA).

## Alert colours
- Red: task is due today
- Yellow: task is due within the next 7 days
- Blue: task is more than 7 days away
- Gray: overdue

## Privacy
This version has no cloud database.
Tasks are stored locally in the browser/PWA using localStorage.
The GitHub repository contains the app code only, not your task data.

Important: clearing relevant Safari website data can erase local tasks.
Use Export Backup regularly if the tasks matter.

## Files
- index.html — app interface and task logic
- manifest.webmanifest — PWA installation metadata
- service-worker.js — offline caching
- icon-192.png / icon-512.png — app icons
- .nojekyll — tells GitHub Pages to serve the static files directly

## GitHub Pages
Upload all files to the root of one repository, then:
Settings > Pages > Build and deployment > Source: Deploy from a branch
Branch: main
Folder: /(root)
Save.

Then open the Pages URL in Safari and use Share > Add to Home Screen.


## Recurring tasks
When creating a task, choose:
- Does not repeat
- Daily
- Weekly
- Monthly — same date/day number
- Yearly — same date

When a recurring task is checked as complete, it automatically advances to the next occurrence.
For dates that do not exist in the next month/year (for example the 31st or February 29), the app uses the last valid day of that month.

## Reminder limitation
This local GitHub Pages PWA can show date-based red/yellow/blue alerts whenever you open it.
Reliable scheduled iPhone push notifications while the app is completely closed require a push/backend service, which is not included in this local-only version.
