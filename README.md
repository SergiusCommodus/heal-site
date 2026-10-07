# H.E.A.L. Website

Investor focused redesign of heal-veins.com for H.E.A.L. (Healthcare Engineering & Life Science).

Static site, no build step. Visual direction follows the H.E.A.L. product sheet: clinical white, navy wordmark, cyan accent. Shared styles live in `assets/site.css`; product imagery in `assets/`.

Three pages:

- `index.html` – home: investor intro, problem, device, business model, roadmap, team, CTA
- `resources.html` – chronic venous insufficiency primer with CEAP table and references
- `contact.html` – investor / clinical / partner inquiry form

## Host on GitHub Pages
Settings → Pages → Source: Deploy from a branch → `main` / root → Save.
To use the heal-veins.com domain, add a `CNAME` file containing `heal-veins.com` and point the domain's DNS at GitHub Pages.

## Before going public
- Product images in `assets/` are cropped from the concept render sheet. Swap in final renders when available.
- Replace bracketed placeholders: four team headshots, investor and general emails, phone, privacy and terms links.
- Confirm sources for the three market figures (35% CVD prevalence, $4–10B annual spend, $2.6B market by 2032).
- Wire the contact form to a form service (see the TODO in `contact.html`); it currently only shows the thank you state.
