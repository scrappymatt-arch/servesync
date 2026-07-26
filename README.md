# ServeSync PWA beta

This folder is ready to host as a Progressive Web App (PWA).

## What this adds
- Installable home-screen app on supported Android browsers
- Standalone full-screen-style launch
- App manifest and ServeSync icons
- Offline caching for the core ServeSync app
- Existing scheduler, packet scanner, cooking mode, wake-lock and alert features

## Important
The PWA must be served over **HTTPS** (or localhost for development). Opening `index.html` directly as a local file is not enough for service workers / installability.

Packet OCR currently loads Tesseract.js from a CDN, so the first packet scan may still require internet access.

## Samsung / Android installation
Once hosted over HTTPS:
1. Open the ServeSync website in Chrome on the Samsung phone.
2. Chrome may show **Install ServeSync** automatically.
3. Otherwise open the Chrome menu (three dots) and choose **Install app** or **Add to Home screen**.
4. Launch ServeSync from the new home-screen icon.

Browser wording varies slightly by Samsung/Chrome version.
