# Codependent web app (v10)

This folder is Codependent as an installable web app. `index.html` is the same page as `Codependent-V10.html`, plus the links that make it installable.

| File | What it does |
|------|--------------|
| `index.html` | The app itself |
| `manifest.webmanifest` | Name, icon and colours, so Android offers "Install app" |
| `sw.js` | Keeps the app's files on the phone so it opens without internet |
| `icon-192.png`, `icon-512.png` | App icons |

## Putting it online (needed before Android offers "Install")
Android only installs web apps served from a website over HTTPS. Opening `index.html` from the phone's storage won't offer it.

**GitHub Pages (free)**
1. Sign in at github.com and create a new public repository, e.g. `codependent`.
2. Choose "uploading an existing file" and drag in all the files from this folder (not the folder itself). Commit.
3. In the repository go to Settings > Pages, set Source to "Deploy from a branch", branch `main`, folder `/ (root)`, and Save.
4. After a minute the page is at `https://<your-user-name>.github.io/codependent/`.

**Netlify Drop (free, no account needed to try)**
1. Go to app.netlify.com/drop and drag this folder onto the page.
2. It gives you an `https://….netlify.app` address.

## Installing on Android
1. Open the address in Chrome on the phone.
2. Tap the ⋮ menu, then "Install app" (or "Add to Home screen").
3. Codependent appears on the home screen and opens full screen.

## Good to know
- The app remembers your text on that phone between opens. Clearing Chrome's site data for the address erases it, so use Save as .txt for anything you want to keep.
- To update the app, upload the new files over the old ones. The phone picks up the new version the time after next that the app is opened.
- Save as .html downloads a copy of the page; the installed app keeps loading the online version.
