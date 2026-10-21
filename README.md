# Shubham’s Workout Split PWA

**Creator / app concept:** Shubham

This project is branded as Shubham’s Workout Split. The creator credit is included in the app interface and project documentation.

## What's included
- Preserves the original Monday–Sunday workout split, exercise names, sets/reps and coaching cues.
- Per-set weight (kg), reps, and completion tracking.
- Local workout progress saving, session history, and JSON export.
- Configurable rest timer; completing a set starts the timer automatically.
- Exercise demonstration links open a YouTube search for the exercise.
- Installable Progressive Web App manifest, service worker/offline shell, and icons.

## Run locally
A PWA must be served from `localhost` or HTTPS; opening `index.html` directly as a `file://` page will not enable installation or the service worker.

With Python installed, open a terminal in this folder and run:
```bash
python -m http.server 8000
```
Then open `http://localhost:8000` in a browser.

## Install on phone
1. Upload the contents of this folder to a static host that serves HTTPS (for example, GitHub Pages, Netlify, or your own HTTPS web host).
2. Open the hosted URL in Safari on iPhone or Chrome on Android.
3. iPhone: Share → Add to Home Screen. Android: use the Install app prompt or browser menu.
4. The initial load should be online so the app shell can be cached. Exercise demo links require internet.

## Data note
Workout logs are stored in browser local storage on that device/browser. Use Workout History → Export workout data for a backup. Clearing browser data or switching devices may remove or not transfer logs.
