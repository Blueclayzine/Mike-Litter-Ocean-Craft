# Mike Litter — Ocean Craft

Single-file landing page for Mike Litter's hand-built wooden ocean craft.

## File structure
```
index.html          - The site (single self-contained HTML/CSS file)
images/             - All photography + logo
fonts/              - Futura .ttf files (loaded via @font-face)
```

## Run locally
Open `index.html` in any browser, or serve it:

```bash
python3 -m http.server 8000
```
Then visit http://localhost:8000

## Deploy to GitHub Pages
1. Push this folder to a GitHub repo (e.g. `mike-litter-site`).
2. In the repo: **Settings → Pages**.
3. Under *Source*, pick **Deploy from a branch** → `main` / `(root)`.
4. Save. Site will be live at `https://<your-username>.github.io/<repo-name>/` in a minute or two.

## Fonts
The original `Futura.ttc` was extracted into five individual `.ttf` files in `/fonts`:
- Futura-Medium.ttf
- Futura-MediumItalic.ttf
- Futura-Bold.ttf
- Futura-CondensedMedium.ttf
- Futura-CondensedExtraBold.ttf

These are loaded via `@font-face` declarations at the top of `index.html`.
For better load performance you can convert these to `.woff2` later (saves ~70%).

## Customizing
- Color palette: `:root` block at the top of `index.html` (`--bg`, `--ink`, `--accent`).
- Replace photos in `/images` keeping the existing filenames.
- All photo sizing is in the `.craft-stack` CSS block.
