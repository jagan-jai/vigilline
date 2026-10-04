# VigilLine — site source

Static one-page subscription site. No build step: edit `index.html`, push, done.

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
- `index.html` — the entire site (self-contained CSS; company voice; plans: Monitor / Intelligence / Desk)
- `assets/og.png` — social share card (1200×630)
- `assets/fonts/` — self-hosted Inter + Instrument Serif (no Google dependency)

## Notes
- v1 (samples-first design) archived outside the repo: `../archive/site-v1-index.html`
- Sample PDFs are **not** in the public repo — they carry portfolio / sole-proprietor language.
  Share via email until they are rebuilt in company voice.
- Palette: deep slate blue `#2C4A7C` + ink `#0E1729` on paper `#FAFAF7` (the slate-blue option
  from the brand identity sheet; gold is reserved for print pieces).
- Prices on the page (₹25K / ₹55K / ₹95K per month) are editable placeholders aligned with
  `../05-pricing/` — adjust before first outreach if needed.
