# Hasinee Atigala — Personal Website

Single-page portfolio site for Hasinee Atigala (Urban & Regional Planner).

## What's in this folder

- `index.html` — single-page site (Hero, About, Experience, Awards, Education, Skills, Contact)
- `styles.css` — all styling (warm rust accent, mobile-responsive)
- `script.js` — minimal vanilla JS (mobile nav toggle + footer year)
- `assets/Hasinee_Atigala_Resume.pdf` — the downloadable CV (kept in sync with the portfolio LaTeX)
- `README.md` — this file

No build step, no framework, no npm. Just open `index.html` in a browser.

## Preview locally

Just open `index.html` in any browser — that works. If you prefer a quick local server:

```bash
cd hasinee/website
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy options

### Option 1 — Netlify (drag-and-drop, ~30 seconds)

1. Go to <https://app.netlify.com/drop>
2. Drag the entire `website/` folder onto the drop zone
3. Netlify gives you a URL like `https://eager-curie-123abc.netlify.app`
4. (Optional) In Netlify Site settings → Domain management → change the subdomain to something like `hasinee-atigala.netlify.app`
5. (Optional) Attach a custom domain later (e.g. `hasineeatigala.com`)

### Option 2 — Vercel

1. Sign up at <https://vercel.com>
2. Click "Add New… → Project" → "Import" a folder
3. Deploy

### Option 3 — GitHub Pages

1. Create a new public GitHub repo (e.g. `hasinee-atigala/hasinee-atigala.github.io` for a user site, or any name for a project site)
2. Push the contents of this folder into the repo root
3. In repo Settings → Pages → set Source to `main` branch / root
4. Site available at `https://<username>.github.io/<repo>/`

## Updating the CV PDF

When the LaTeX resume changes, copy the latest PDF over:

```bash
cp ../hasinee_atigala_portfolio.pdf assets/Hasinee_Atigala_Resume.pdf
```

Then re-deploy (Netlify drag-and-drop again, or push to git).
