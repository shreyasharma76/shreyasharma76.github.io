# Shreya Sharma — Portfolio v1 (scroll tour)

The scroll-driven version of Shreya Sharma's portfolio. A 3D pixel-art character walks visitors through three projects (HealNova AI, Google Meet Live Transcription, ML recommenders), then a grid of work and education, then contact details.

It's a finished, static website: no install step and no build step.

---

## Run it

> **Don't double-click `index.html`.** Browsers block the page's scripts when it's opened as a file, so the animations and character won't load. Serve the folder with a tiny local web server instead. Pick any one option below.

### Option 1: Python (already on most computers)

1. Unzip this folder.
2. Open a terminal **inside** the unzipped folder (the one that contains `index.html`).
   - **Windows:** open the folder in File Explorer, click the address bar, type `cmd` and press Enter.
   - **macOS:** right-click the folder in Finder and choose **New Terminal at Folder**.
3. Run:

   ```bash
   python -m http.server 8000
   ```

   On macOS or Linux, use `python3` if `python` isn't found.
4. Open **http://localhost:8000** in your browser.
5. Press `Ctrl + C` in the terminal to stop the server.

### Option 2: Node.js

```bash
npx serve .
```

Then open the address it prints (usually http://localhost:3000).

### Option 3: VS Code

Install the **Live Server** extension, open this folder in VS Code, right-click `index.html` and choose **Open with Live Server**.

---

## Put it online

All paths are relative, so the folder works at a domain root or inside a sub-folder.

- **GitHub Pages:** create a repository, upload everything in this folder (including the hidden `.nojekyll` file), then go to **Settings → Pages → Deploy from a branch → main / root**. If the repository is named `<username>.github.io`, the site appears at `https://<username>.github.io/`.
- **Netlify:** drag the unzipped folder onto https://app.netlify.com/drop.
- **Any static host:** upload the folder contents as they are.

---

## What's inside

| Path | What it is |
| --- | --- |
| `index.html` | The whole page: text, project tour, work grid and contact section. |
| `_astro/` | Bundled scripts, styles and fonts (compiled; don't edit unless you have to). |
| `assets/images/` | Project screens and work-card covers. |
| `assets/Shreya_Sharma_Resume.pdf` | Résumé linked from the page. |
| `favicon*`, `apple-touch-icon.png`, `og-image.png`, `site.webmanifest` | Browser icons and the link-preview image. |

## Making small changes

- **Text:** search `index.html` for the words you want to change and edit them in place.
- **The character's look:** find `data-look=` in `index.html`. `hair` can be `long`, `curly` or anything else for short hair, `beard` is `true`/`false`, and `colors` holds hex colours (the quotes are written as `&#34;`).
- **Images:** replace a file in `assets/images/` with one of the same name and size. Desktop screens are 1440×900, phone screens 640×1386 and covers 1200×800.

## Good to know

- Scroll slowly through the project tour; the animations are tied to the scroll position.
- Try grabbing the character, clicking **Do a trick** in the footer, or typing `shreya.wave()` in the browser console.
- The project screens are illustrative mock-ups, not real product screenshots.
- If you see a blank space where the character should be, your browser or device has WebGL turned off.
