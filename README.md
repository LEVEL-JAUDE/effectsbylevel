# LEVEL-JAUDE

Landing page for **[effectsbylevel.com](https://effectsbylevel.com)** — a single-page funnel splash that drives visitors to the LEVEL Shopify store ([levelexperience.shop](https://levelexperience.shop)).

## What it is
A self-contained, on-brand splash page (`index.html`, no build step) with an animated brand-color aurora, an equalizer "levels" mark, the four effect categories (Sleep · Calm · Focus · Energy), and a primary **Shop LEVEL** CTA. The CTA and footer links are UTM-tagged (`utm_source=effectsbylevel`) so the funnel is trackable in Shopify analytics.

## Hosting
Served via **GitHub Pages** from the `main` branch (root). The custom domain is configured by the [`CNAME`](CNAME) file.

### GoDaddy DNS (apex domain `effectsbylevel.com`)
Point the domain at GitHub Pages with these records:

| Type | Name | Value |
|------|------|-------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | feasterjamie-hash.github.io |

After DNS propagates, enable **Enforce HTTPS** in the repo's Pages settings.

## Editing
Everything lives in [`index.html`](index.html) — colors are CSS variables at the top of the `<style>` block, matching the official LEVEL Pantone palette. Edit and push to `main`; GitHub Pages redeploys automatically.
