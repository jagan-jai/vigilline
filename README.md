# VigilLine — site source

Static one-page site. No build step: edit `index.html`, push, done.

**Live:** https://jagan-jai.github.io/vigilline/ (until vigilline.com is connected)

## Updating
```bash
cd ~/Work/ci-side-hustle/site
# edit index.html or replace files in assets/
git add -A && git commit -m "update" && git push
```
GitHub Pages rebuilds automatically in ~1 minute.

## Connecting vigilline.com (once the domain is bought)
1. Repo → Settings → Pages → Custom domain → enter `vigilline.com`
2. At the registrar: A records → 185.199.108.153 / 185.199.109.153 / 185.199.110.153 / 185.199.111.153
   and `www` → CNAME → `jagan-jai.github.io`
3. Tick "Enforce HTTPS" (auto-provisions once DNS propagates)

## Structure
- `index.html` — the entire site (self-contained CSS)
- `assets/vigilline-sample-oncology-daraxonrasib.pdf` — public sample (12 pages, 25 sources)
- `assets/vigilline-sample-glp1.pdf` — public sample (13 pages, 22 sources)
- `assets/vigilline-method.pdf`, `assets/vigilline-brochure.pdf`
- `assets/thumb-*.png` — card previews · `assets/og.png` — social card
- `assets/fonts/` — self-hosted Inter + Instrument Serif (no Google dependency)
