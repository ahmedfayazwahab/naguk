# Naguk Inc. — Restaurant Group Website

Marketing website for **Naguk Inc.**, Toronto's restaurant group behind Thai Room Grand,
Kohlipe, Savor, Le Lert, and more — fine Thai and Indian dining across the GTA.

**🔴 Live at [naguk.ca](https://naguk.ca)**

## What this is

A static, multi-page marketing site — no backend, no build step. Every page is a
self-contained HTML file that pulls in shared CSS/JS from `css/` and `js/`. Contact and
newsletter forms submit directly to Formspree; table reservations link out to OpenTable/Tock.

## Pages

| Page | Purpose |
|---|---|
| `index.html` | Home — restaurant family overview, reservations |
| `services.html` | Services offered |
| `privatedining.html` | Private dining info |
| `team.html` | Our chefs |
| `gallery-image.html` / `gallery-video.html` | Photo/video galleries |
| `cart.html` | Gift card |
| `contact.html` | Contact form (Formspree), location/hours |
| `404.html` | Custom not-found page |

**Not part of the live site:** `blog2.html` ("Candóre \| Restaurant & Wine Bar") and
`coming-soon.html` ("Naguk Enterprises") carry titles unrelated to any of Naguk's listed
restaurants — leftover pages from template reuse or an earlier concept, not linked from
the current site nav.

## Tech stack

- **Markup/styling:** HTML5, CSS3, [Bootstrap](https://getbootstrap.com/)
- **Animation/interaction:** WOW.js (scroll animations), Vegas (hero background slider), Stellar.js (parallax), Pace.js (page-load progress), custom scripts (`js/custom.js`)
- **UI components:** Owl Carousel, Isotope (filtering/layout), Magnific Popup (lightbox), Select2 (dropdowns), Smoke.js, ScrollIt, Sticky-kit, a reservation datepicker
- **Forms:** [Formspree](https://formspree.io/) — no server-side code required
- **Reservations:** OpenTable / Tock (linked out, no in-site booking)
- **Analytics:** Google Analytics (gtag.js)
- **SEO:** `sitemap.xml`, `robots.txt`, per-page meta/Open Graph/Twitter tags

## Running locally

No install or build step needed — it's static HTML. Serve the folder with any static
file server and open it in a browser, e.g.:

```bash
npx serve .
# or
python3 -m http.server 8000
```

Then visit `http://localhost:8000` (or the port shown).

## Status

Live production website for Naguk Inc., currently deployed at naguk.ca.
