GROVE — your downtime & intentions app
======================================

WHAT THIS IS
A self-contained app. No accounts, no servers, no tracking. Everything you
log stays in your phone's local storage. It works fully offline once installed.

WHAT'S IN THIS FOLDER
  index.html              the whole app
  manifest.webmanifest    makes it installable with its own icon
  sw.js                   service worker (offline support)
  icon-192.png            app icon
  icon-512.png            app icon
  apple-touch-icon.png    iOS icon
Keep all files together in the same folder.


GET IT ON YOUR PHONE — easiest route (no tools, ~2 minutes)
-----------------------------------------------------------
A phone "installable" app needs to be served over https. The simplest way:

1. On your computer, go to:  https://app.netlify.com/drop
2. Drag this whole "grove" folder onto the page.
   (A free Netlify account may be asked for — that's fine.)
3. It gives you a link like  https://something-random.netlify.app
4. Open that link on your phone (text it to yourself, or it shows a QR).
5. Install it (see "ADD TO HOME SCREEN" below).

That link is yours and stays live. Bookmark it in case you reinstall.

Alternatives that also work: GitHub Pages, Cloudflare Pages, Vercel — any
static host over https.


ADD TO HOME SCREEN (so it becomes a real app icon)
--------------------------------------------------
Chrome on Android:
  - Open the link, tap the ⋮ menu, tap "Add to Home screen" / "Install app".
Samsung Internet:
  - Open the link, tap the menu, tap "Add page to" → "Home screen".

After that, Grove launches full-screen from its own icon and runs offline.


YOUR DATA
- Stored only on this device (browser local storage).
- More tab → JSON / Logs CSV gives you a backup any time.
- Clearing the browser's site data, or uninstalling, erases it — so export
  now and then if it matters to you.
- Reinstalling from the same link is fine; just don't "clear site data".


WANT TO CHANGE SOMETHING LATER
- Small text/colour tweaks: edit index.html and re-upload the folder.
- Bigger changes, or to build a native version: hand this folder to Claude
  Code (Code tab in the Claude desktop app). It can run a real build, add
  features, and redeploy for you. The whole thing is plain HTML/CSS/JS, so
  it's easy to extend.

Built around one idea: make the effort visible, keep the rest gentle.
