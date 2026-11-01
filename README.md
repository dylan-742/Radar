# PC 4022 Radar Review Primer

A phone-first review of the 30 PC 4022 Radar Concepts I exam questions. Each card builds its answer in two or three short tap-to-answer steps, then gives the exam answer and a one-line recall chain.

The site is one HTML page with everything it needs built in: fonts, figures and code. It makes no outside requests and does no tracking. Progress is saved only in your phone's browser. Once you have opened it, it also works with no signal.

## What's in this folder

| File | What it is |
|---|---|
| `index.html` | The whole lesson, with the fonts embedded. |
| `manifest.webmanifest` | Lets phones install it as an app with a name and icon. |
| `sw.js` | Offline cache. It saves the page the first time you open it. |
| `icons/` | Home-screen and browser icons. |
| `fonts-LICENSE.txt` | SIL Open Font License for the embedded IBM Plex and Source Serif 4 fonts. |

## Publish it with GitHub Pages (about 5 minutes, in a browser)

1. Sign in at **github.com** and click **New repository**.
2. Name it, for example **`radar-review`**, and set it to **Public**. GitHub Pages on a free account needs a public repository. Click **Create repository**.
3. On the new repository's page, click **uploading an existing file**, or **Add file → Upload files**.
4. Drag in **everything in this folder**: `index.html`, `manifest.webmanifest`, `sw.js`, `fonts-LICENSE.txt`, `README.md` and the whole **`icons`** folder. Then click **Commit changes**.
   - Dragging a folder works in Chrome, Edge and Firefox on a computer.
   - If your browser won't take the folder, open `icons/` and upload its five files into a folder named `icons`. Typing `icons/` in the file-name box creates the folder.
5. Go to **Settings → Pages**. Under **Build and deployment**, set:
   - **Source**: **Deploy from a branch**
   - **Branch**: **main**
   - **Folder**: **/ (root)**

   Then click **Save**.
6. Wait a minute or two, then refresh the Pages settings screen. It shows your site's address:

   **`https://YOUR-USERNAME.github.io/radar-review/`**

### Or with git, from a terminal

```bash
cd radar-review-site
git init -b main
git add .
git commit -m "Radar review primer"
git remote add origin https://github.com/YOUR-USERNAME/radar-review.git
git push -u origin main
```

Then do step 5 above.

## Put it on your phone

1. Open the address on your phone **while you have a signal**.
2. Install it:
   - **iPhone (Safari):** tap **Share** (the square with an arrow), then **Add to Home Screen**, then **Add**.
   - **Android (Chrome):** tap **⋮**, then **Add to Home screen** or **Install app**.
3. Open it once from the new home-screen icon. From then on it opens like an app and works offline.

Your progress stays on that phone. **Start over**, at the bottom of the page, clears it.

## Updating it later

- **To change the lesson:** upload a new `index.html` to the repository. Phones fetch the new page the next time they open it with a signal.
- **If you change the icons or the manifest:** also edit the first line of `sw.js` from `radar-review-v1` to `radar-review-v2` so phones drop the old cached copies.

## Opening the file directly

`index.html` also works as a plain downloaded file, opened in a desktop browser or in Chrome on Android. It has no offline install that way.

iPhone's Files app shows HTML as a preview without running it, so on iPhone use the GitHub Pages address and **Add to Home Screen**.

## Content

Answers follow the instructor's PC 4022 deck, with slide numbers given on each card. Q13, Q20–Q22 and Q24 go beyond the deck and use cited public sources, dated October 2026.
