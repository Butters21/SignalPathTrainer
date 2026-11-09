# Signal Path Trainer

Interactive training for new live sound technicians: signal flow, gain structure, buses and plugins, microphones, monitors, patching, system, cables and safety, plus practice desks, fault finding, quizzes, show control and a Dante lab.

The whole app is one HTML file. It works in any modern browser. On iPhone and iPad it detects the device and switches to a touch layout with a bottom tab bar.

## Folders

| Path | What it is |
|---|---|
| `index.html` | The stable app |
| `manifest.webmanifest`, `icons/` | Name and icons for Add to Home Screen |
| `sw.js` | Offline support. It caches the app after the first visit |
| `beta/` | A test copy with its own saved progress, so testing never touches real progress |
| `.nojekyll`, `404.html` | GitHub Pages housekeeping |

## Publish with GitHub Pages (one time)

1. Create a repository on github.com (for example `signal-path-trainer`). Free accounts need it to be **Public** for Pages; private repos need a paid plan.
2. **Add file → Upload files** and drag in everything from this folder, including the `beta` and `icons` folders. Commit.
3. Go to **Settings → Pages**. Under *Build and deployment*, choose **Deploy from a branch**, then branch **main** and folder **/ (root)**. Save.
4. After a minute or two the site is live at `https://<your-user>.github.io/signal-path-trainer/`. The beta copy is at `.../signal-path-trainer/beta/`.

## Use it like an app on iPhone or iPad

Open the link in **Safari**, tap **Share → Add to Home Screen**. It opens full screen with its own icon and works offline after the first load.

## Updating while it's being built

1. Upload the new `index.html` and `sw.js` into **`beta/`** first and test on your phone.
2. When happy, upload the new root `index.html` and `sw.js` too.
3. Each build writes a new version number into `sw.js`, which tells installed copies to refresh. Always upload `sw.js` together with `index.html`.

Saved progress lives in each browser. Clearing Safari's website data resets it.

## Content notes

All teaching text is written in our own words. Manufacturer manuals and books were used as references only and are **not** included here. Please don't add copyrighted PDFs to this repository.
