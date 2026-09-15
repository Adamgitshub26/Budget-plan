# Budgets — offline budget planner (v1.8)

A monthly income/expense planner that installs to your phone and works with no internet.
It saves all data on your own device (nothing is uploaded anywhere).

## Files in this folder
- `index.html` — the whole app
- `manifest.webmanifest` — lets it install like a real app
- `service-worker.js` — makes it work offline
- `icon-192.png`, `icon-512.png` — app icons

Keep all files together in the same folder.

## Put it on GitHub (free hosting)

1. Sign in at https://github.com and click the **+** (top right) → **New repository**.
2. Name it, e.g. `budgets`. Set it to **Public**. Click **Create repository**.
3. On the new repo page click **uploading an existing file**.
4. Drag in **all** the files from this folder (index.html, manifest.webmanifest, service-worker.js, both icons). Click **Commit changes**.
5. Go to the repo's **Settings** → **Pages** (left menu).
6. Under **Branch**, choose **main** and folder **/ (root)**, then **Save**.
7. Wait about a minute, then refresh. GitHub shows a link like:
   `https://YOUR-USERNAME.github.io/budgets/`

Open that link on your phone.

## Install it on your phone (so it works offline)
- **Android (Chrome):** open the link → menu (⋮) → **Add to Home screen** / **Install app**.
- **iPhone (Safari):** open the link → **Share** button → **Add to Home Screen**.

After installing, open it once while online so it can cache itself. From then on it opens and works even in airplane mode. Your data stays saved on the device.

## Updating the app later
If I give you a new version, upload the new `index.html` (and any changed files) to the repo the same way (step 3–4, "Add file" → "Upload files"), and bump the `CACHE` name inside `service-worker.js` (e.g. `budgets-v1.9`). Reopen the app twice and the update loads.

## Backup
Your data lives only on the device. Use **Export CSV** inside the app now and then to keep a copy (it opens in Excel/Sheets). Clearing your browser data or deleting the app will erase the saved budgets, so export before doing either.

## Note about the data
The app starts with sample Home/Work/Money Sent budgets. Edit the rows to your own, and it remembers everything after that.
