# Grove

A small, private companion for keeping downtime intentional and effort visible.
No accounts, no servers, no tracking — everything you log stays on your own device.

## What it does

- **Today** — a menu of downtime activities with daily caps you tap down (pips for counts, a bar for minutes), each with a built-in timer. Plus today's intentions to check off, a quick capture box for stray thoughts, and a nap log.
- **Plan** — set tomorrow's one-to-three "for sure" intentions (with rough effort points), and clear your deferred-thoughts inbox.
- **Journal** — a nightly entry: energy rating, mood, what you did, how it felt.
- **Stats** — a forest that grows from your activity (each day is a tree; busy days grow tall, quiet days stay saplings), plus per-activity counts and streaks, an energy trend, and points finished.
- **More** — edit the menu items and caps, export your data, or reset.

## Tech

Plain HTML, CSS, and JavaScript. No build step, no dependencies, no frameworks.
Installable as a PWA and fully offline after first load via a service worker.

## Data & privacy

- All data is stored in the browser's local storage **on the device only**.
- Nothing is sent anywhere. The repo contains code, never personal data.
- Back up any time from **More → JSON / Logs CSV**.
- Clearing the site's data or uninstalling erases everything, so export occasionally.

## Install (Android)

1. Open the live link in Chrome and let it fully load.
2. Reload once so the service worker registers.
3. Menu (⋮) → **Install app**.

## Hosting notes

Served via GitHub Pages from the repo root. All paths are relative, so it works
from a project subpath (e.g. `username.github.io/grove/`) without changes.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The whole app |
| `sw.js` | Service worker (offline caching) |
| `manifest.webmanifest` | Makes it installable with its own icon |
| `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | App icons |

---

*Built around one idea: make the effort visible, keep the rest gentle.*
