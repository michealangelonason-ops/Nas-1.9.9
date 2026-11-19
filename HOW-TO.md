# Nas - Track and Improv: how to open it and make it an app

The app has its own built-in tutorial: it opens on first launch, and the ? button in the header reopens it.

## 1. Quick look (no install)
Open index.html in Chrome or Safari. Everything works, but it can't be installed this way.

## 2. Make it a real app (recommended)
An installable app needs to be hosted on a free https link.
- Phone only: create a free GitHub account, make a new repository, use "Add file > Upload files" and upload everything in this folder (also the hidden .github folder if your phone shows it). Then Settings > Pages > Deploy from a branch > main > root. After about a minute you get a link.
- With a computer: drag this folder onto app.netlify.com/drop.
Then open the link on your phone:
- Android (Chrome): tap Install in the app header, or menu > Install app.
- iPhone (Safari): Share > Add to Home Screen.
It opens full screen with its own icon and works offline.

## 3. Get an APK
- Easiest: go to pwabuilder.com, paste your link, choose Android, download the package.
- Automatic: in your GitHub repo open Actions > Build APK > Run workflow. When it finishes, download "nas-apk" and install the APK (allow installs from unknown sources).

## Notes
- Your data is stored on the device. Use Skins > Export backup now and then.
- When you update index.html later, change the cache name in sw.js (nas-v1 to nas-v2).
