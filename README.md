# H.E.A.L. Website

Investor and clinician facing site for H.E.A.L. (Healthcare Engineering & Life Science).

Live: https://sergiuscommodus.github.io/heal-site/

Static site, no build step needed to host. Pages:

- `index.html`: home (intro animation, platform, workflow, how it works, applications, business model, market, roadmap, team)
- `resources.html`: chronic venous insufficiency primer with CEAP table and references
- `contact.html`: inquiry form
- `404.html`: not found page

Assets:

- `assets/heal.css`, `assets/heal.js`: readable source
- `assets/heal-v6.min.css`, `assets/heal-v5.min.js`: minified files the pages load. After editing the source, regenerate these and bump the version number in the file name so browsers and GitHub's cache pick up the change.
- Images ship as JPG with WebP versions (`name.webp`, `name-480.webp`, `name-800.webp`). Replace both when swapping an image.

SEO: canonical links, Open Graph and Twitter cards with absolute image URLs, Organization structured data, `robots.txt`, `sitemap.xml`.

## Turn on the contact form

The form currently tells visitors to reach the team on LinkedIn instead of pretending to send.

1. Create a free form at formspree.io pointed at the inbox that should receive inquiries.
2. In `contact.html`, set `var HEAL_FORM_ENDPOINT = "https://formspree.io/f/xxxxxxx";`

## Before sharing widely

- Connect the contact form (above).
- Add investor email and phone in `contact.html` (commented out block ready to uncomment).
- Headshots for Gavin Franzon and James Pappas.
- Confirm the CEO listing now that Karl J. Pappas is CTO.
- Confirm sources for the market figures.
- Privacy policy page (recommended once the form collects data).
- Optional: point heal-veins.com here (add a `CNAME` file and update DNS).
