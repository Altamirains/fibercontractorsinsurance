# fibercontractorsinsurance

Static SEO landing-page site targeting fiber-optic / ISP subcontractors.

## Stack
- **Plain static HTML/CSS** — no build step.
- Each landing page lives in its own folder with `index.html`.
- Hosted on Netlify.

## Structure
- `index.html` — homepage
- `<carrier>-subcontractor-insurance/` — one folder per ISP/carrier (att, frontier, google-fiber, brightspeed, archtop, bluepeak, intrepid, greenlight-networks, …)
- `<state>/` and `<city>-<state-abbr>/` — geo landing pages (california, arizona, los-angeles-ca, las-vegas-nv, …)
- `<service>-contractor` / `-insurance/` — service-specific (fiber-optic-splicing, cable-installer, low-voltage, isp-subcontractor)
- `blog/` — blog posts
- `get-a-quote/` — quote form landing page

## Conventions
- Mirror the structure of existing pages when adding new carrier/geo/service combos.
- For sitewide changes, search-and-replace across all `index.html` files — there's no shared template.
- Use the SEO-fixes script in `~/Projects/Altamira/tools/seo_fixes/seo_fixes.py` for bulk meta-tag/title sweeps.
