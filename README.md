# CigTracker 🚬

A simple, fast, and secure single-page web application to track your daily cigarette consumption. 

## Features

- **Local-First Design:** All data is stored directly in your browser's `localStorage` meaning no servers, no accounts, and complete privacy.
- **Single-File Architecture:** The entire app—HTML, CSS, and JS logic—lives in one incredibly lightweight file (`index.html`), making it lightning fast and simple to host anywhere.
- **Cross-Device Sync:** Instantly sync your history between your desktop and smartphone by generating a secure `#data` URL hash, which you can easily bookmark or share. 
- **Conflict Resolution:** When syncing a session, the app smartly merges both histories by keeping the highest historical counts to prevent data loss.
- **Live Timer:** See exactly how many hours, minutes, and seconds have passed since your last cigarette right on the dashboard.

## Live Demo

[Live CigTracker App](https://plonzari.github.io/cigtracker/)

## Syncing Between Devices

1. Open the app on your primary device.
2. Click the share icon in the top right to update the URL bar with your data history hash.
3. Save that new URL as a bookmark or copy it to a synced note.
4. Open the link on your secondary device to merge the data automatically. 

*Built with ❤️ via Antigravity Tutorial*
