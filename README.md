# Daybook: your offline productivity app

Files:
- index.html: the whole app (screens, look, and logic). Edit this to change things.
- manifest.json: name, colours and icon used when installed on the home screen.
- sw.js: makes the app open with no internet. Bump "daybook-v1" to "v2" etc. after every change.
- (main folder)/: home-screen icons (replace with your own PNGs of the same sizes if you like).

## Put it on your phone (one-time, needs internet once)
1. Create a free GitHub account at github.com (Chrome on phone or laptop works).
2. New repository → name it `daybook` → Public → Create.
3. "Add file" → "Upload files" → upload index.html, manifest.json, sw.js, and the icons folder
   (on a laptop you can drag the whole unzipped folder in). Commit.
4. Settings → Pages → Source: "Deploy from a branch" → Branch: main, folder: / (root) → Save.
5. Wait 1–2 minutes. Your app is at https://YOUR-USERNAME.github.io/daybook/
6. Open that link in Chrome on your Android phone → ⋮ menu → "Add to Home screen" / "Install app".
7. Done. Turn on airplane mode and open it from the home screen to confirm it works offline.

## Your data
Stored only on the phone (Chrome's local storage). Use More → "Download backup" regularly.
Uninstalling the app or clearing Chrome's site data deletes it.

## Making changes
Edit index.html (start with the colours at the top of the <style> section), bump the version
in sw.js, re-upload to GitHub. Open the app once while online and it updates itself.

## Testing on a laptop
In this folder run `python -m http.server 8000`, then open http://localhost:8000 in Chrome.
Press F12 → the phone icon to see it at phone size.
