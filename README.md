# Skyfellow Initiative — Website

Bilingual (EN / JP) single-page website for the Skyfellow Initiative.  
Built for deployment on **GitHub Pages** with no external dependencies.

---

## File Structure

```
skyfellow-site/
├── index.html                   ← Main website (single file, all CSS + JS included)
├── suzuki-profile-photo.jpeg    ← Hidemichi Suzuki profile photo
├── miwa-profile-photo.jpeg      ← Akira Miwa profile photo
├── skyfellow-hero-bg.jpeg       ← Hero section background image
├── skyfellow-global-network.jpeg← Purpose section supporting image
├── skyfellow-bridge-concept.jpeg← Approach section supporting image
└── skyfellow-ogp.jpeg           ← OGP / LinkedIn share image (metadata only)
```

---

## GitHub Pages Deployment Steps

### Option A — New Repository (recommended)

1. Go to [github.com](https://github.com) and sign in.
2. Click **+** → **New repository**.
3. Name it `skyfellow-initiative` (or any name you prefer).
4. Set visibility to **Public**.
5. Click **Create repository**.
6. On the next screen, click **uploading an existing file**.
7. Drag and drop **all files** in this folder into the upload area.
8. Click **Commit changes**.
9. Go to **Settings** → **Pages** (left sidebar).
10. Under **Branch**, select `main` and folder `/` (root) → click **Save**.
11. Wait ~1 minute. Your site will be live at:  
    `https://<your-github-username>.github.io/skyfellow-initiative/`

### Option B — Existing Repository via GitHub Desktop

1. Open **GitHub Desktop** and clone or open your repository.
2. Copy all files from this folder into the repository root.
3. Commit with message: `Add Skyfellow Initiative website`.
4. Push to `main`.
5. Enable GitHub Pages in repository Settings → Pages.

---

## Updating Content

All content is inside `index.html`. Open it in any text editor.

- **English text**: inside `<div class="en">` blocks
- **Japanese text**: inside `<div class="jp">` blocks
- **Contact form links**: search for `docs.google.com/forms` — two separate links (EN and JP)
- **Profile photos**: replace the `.jpeg` files with the same filenames
- **Colors**: CSS variables are at the top of the `<style>` block (`:root { ... }`)

---

## Technical Notes

- No external libraries or CDN dependencies — works offline after initial load.
- GitHub Pages compatible (pure static HTML/CSS/JS).
- Responsive: desktop, tablet, and mobile.
- Language toggle: EN / JP — default is English.
- All external links open in a new tab (`target="_blank"`).
- No email addresses are displayed visibly on the page.
