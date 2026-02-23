# CigTracker 🚬

A simple, fast, and secure single-page web application to track your daily cigarette consumption. 

## Features

- **Local-First Design:** All data is stored directly in your browser's `localStorage` meaning no servers, no accounts, and complete privacy.
- **Single-File Architecture:** The entire app—HTML, CSS, and JS logic—lives in one incredibly lightweight file (`index.html`), making it lightning fast and simple to host anywhere.
- **Cross-Device Sync:** Instantly sync your history between your desktop and smartphone by generating a secure `#data` URL hash, which you can easily bookmark or share. 
- **Conflict Resolution (Accidental Enterprise Architecture):** Under the hood, this uses a fancy distributed systems concept called a **CRDT (Conflict-free Replicated Data Type)**—specifically a G-Set (Grow-only Set). Basically, because you mathematically cannot "un-smoke" a cigarette in the past, merging two histories from different devices is just a simple, conflict-free union of two sets. Yes, this humble smoking tracker uses the same replication math as Amazon DynamoDB. You're welcome.
- **Live Timer:** See exactly how many hours, minutes, and seconds have passed since your last cigarette right on the dashboard.

## Live Demo

[Live CigTracker App](https://plonzari.github.io/cigtracker/cigarette-counter.html)

## Syncing Between Devices

1. Open the app on your primary device.
2. Click the share icon in the top right to update the URL bar with your data history hash.
3. Save that new URL as a bookmark or copy it to a synced note.
4. Open the link on your secondary device to merge the data automatically. 

*Built with ❤️ via Antigravity Tutorial*
