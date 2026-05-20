# Tectus Atlas — Website

Static marketing site. Discover. Govern. Lead.

## Stack

- Plain HTML + CSS, no build step required
- React + Babel (CDN) only for the in-page Tweaks panel
- Inter (Google Fonts), JetBrains Mono (Google Fonts)

## Files

```
.
├── index.html          # main page (DE/EN, cookie banner, legal modal)
├── homepage.css        # all styles
├── tweaks-panel.jsx    # in-page tweaks controls (dev/preview only)
└── assets/             # logo system + founder portrait
```

## Local preview

Any static server will do:

```bash
npx serve .
# or
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Deploy on Vercel

1. Push this folder to GitHub (see below).
2. <https://vercel.com> → **Add New Project** → import the repo.
3. Framework Preset = **Other**, Build Command = *(empty)*, Output Directory = `.`
4. Deploy. You get a `*.vercel.app` URL instantly.
5. **Settings → Domains** → add `tectus-atlas.com`. Follow the DNS instructions at your registrar (A-Record + CNAME). HTTPS is automatic.

## Pre-launch checklist

Replace the placeholders (search for `[`) before going live:

- [ ] Impressum: `[Straße Hausnummer]`, `[PLZ]`, `[X. Bezirk]`
- [ ] Impressum: `[ATU00000000]` (UID), `[FN 000000 a]` (Firmenbuchnummer)
- [ ] Impressum: `[Name der Versicherung]` (Berufshaftpflicht)
- [ ] Datenschutz: `[Straße]`, `[PLZ Wien]`
- [ ] Mailboxes operational: `hello@`, `privacy@`, `legal@`, `audit@`, `pilot@`
- [ ] AVV PDF available on request via `legal@tectus-atlas.com`
- [ ] Plausible Analytics self-hosted, snippet inserted before `</body>`
- [ ] LinkedIn URL in footer

## License

© 2026 Tectus Atlas. All rights reserved.
