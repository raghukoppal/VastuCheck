# Pyramid Vastu — New Website

## What's in this package
- `index.html` — the complete website (one file, no build step needed)
- `robots.txt` + `sitemap.xml` — drop these in your site's root alongside `index.html`

## Latest update
- The hero **Vastu Purusha Mandala** now has the **Vastu Purusha figure** drawn at its centre — head toward the auspicious north-east (Ishanya) corner, feet toward the south-west (Nairutya), per classical Vastu Shastra convention. This is an original line illustration in the site's own gold/copper style, not a copy of any third-party image, so there's no licensing concern using it commercially.
- The **About** section now uses an actual photo frame for Shankar Medigoudar instead of initials. It points to `assets/img/shankar_m.png` — the same path your original site used — so it should pick up automatically once deployed. If that file isn't present, the page gracefully falls back to the initials avatar instead of showing a broken image.
- **Services** now opens with a line about bringing prosperity, wealth, peace and abundance to land, sites, flats, villas, stores and commercial buildings — plus a row of property-type chips. The Vastu Check form's property options were broadened to match (Land/Site, Commercial/Store).

## What changed from the original site (first rebuild)
- New visual identity built around the **Vastu Purusha Mandala** (the classical 9×9 directional grid) instead of a generic compass image — used in the hero, the Vastu Check section, and as the form's life-area tags (e.g. Health → NE, Wealth → N).
- New **"Vastu Check" form** for Flat / Independent House / Land / Commercial requests, with property details, facing direction, and a checklist of concerns (health, wealth, relationships, career, peace of mind, legal). On submit, it builds a pre-filled **WhatsApp message** and **email** so the enquiry reaches +91 99889 59995 / spslifeeasy@gmail.com immediately — no server required.
- **Products section** (Space Wave Resonator, Geopathic Rods, Harmony Pyramid) — each has an "Enquire" button that jumps to the form and pre-fills the message.
- Services, About, Testimonials all rebuilt from your original content with sharper copy, plus a new **FAQ** section (also marked up as FAQ schema for Google).
- Full SEO pass: descriptive title/meta description, Open Graph + Twitter cards, canonical tag, JSON-LD structured data (Business, Services, Products, FAQ), semantic headings, alt text throughout, `robots.txt`, `sitemap.xml`.
- Fully responsive (mobile menu, stacked layouts), accessible (visible focus states, aria labels, respects "reduce motion" settings), and fast (no external images — all graphics are inline SVG).

## Important: the form needs your attention before launch
This is a static HTML file, so there's no server to *receive* form submissions automatically. Right now, submitting the form opens a **pre-filled WhatsApp chat** or **pre-filled email** so the request still reaches you reliably with zero setup.

If you'd prefer submissions to land silently in your inbox or a spreadsheet (no click required from the visitor), I can wire the form up to a free service like **Web3Forms** or **Formspree** — just say the word and share/create an account, and I'll plug in the endpoint.

## Things to swap in before you publish
1. **Logo** — currently a generated pyramid/mandala mark. Replace `.brand-mark` SVG with your real logo if you have one.
2. **Open Graph image** — `og:image` points to `/assets/img/og-image.jpg`, which doesn't exist yet. Add a 1200×630px image at that path (a nice mandala/hero shot) so links look good when shared on WhatsApp/social.
3. **Map embed** — currently centered on "Bangalore" generally. If you have an exact office address, I can point the embedded map to that pin.
4. **Phone/email** — currently using the same details as your original site (+91 99889 59995 / spslifeeasy@gmail.com). Update in `index.html` (search for these strings) if anything has changed.

## How to publish
Upload `index.html`, `robots.txt`, and `sitemap.xml` to the root of your hosting (wherever vastucheck.com currently points) — no build tools needed, it's plain HTML/CSS/JS.
