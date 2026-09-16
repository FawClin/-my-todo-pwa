# My To-Do PWA

This package contains the final local PWA version of the task app.

## Files
- index.html
- manifest.webmanifest
- service-worker.js
- icon-192.png
- icon-512.png
- .nojekyll

## JSON restore
The app keeps the JSON Import function from the final prototype.

It accepts:
1. the app's exported JSON backup with a `tasks` array, or
2. a plain JSON task array.

After installing/opening the PWA, use **Import JSON** and choose your saved backup.

## GitHub Pages
Upload all files to the root of the same repository or a new repository.
Then set:
Settings > Pages > Deploy from a branch > main > /(root)

Open the Pages URL in Safari and use:
Share > Add to Home Screen

## Evisionsoft splash
The 1-second Evisionsoft splash runs immediately over the app while the To-Do UI renders underneath.
