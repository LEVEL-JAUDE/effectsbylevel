# LEVEL-JAUDE

Landing page for **[effectsbylevel.com](https://effectsbylevel.com)** — a single-page funnel splash that drives visitors to the LEVEL Shopify store ([levelexperience.shop](https://levelexperience.shop)).

## What it is
A self-contained, on-brand landing page (`index.html`, no build step) styled to match the live LEVEL store (Horizon theme): white background, Inter, near-black type, black 12px-radius buttons. It uses the real LEVEL logo and product photography, a **"Tiny Tablets. Big Effects."** hero, a Sleep → Relief → Relax crossfading product card (with a glow that matches each label color), the four effects (Sleep · Relief · Relax · Calm), a 4.8★ rating line, an **As seen in** press strip (PBS, Wellness, Yahoo Finance, SFGATE), and **Shop now** / **Take the Quiz** CTAs. All store links are UTM-tagged (`utm_source=effectsbylevel`) so the funnel is trackable in Shopify analytics.

## Pages
- **`/`** ([index.html](index.html)) — the splash: "Tiny Tablets. Big Effects." hero with an auto-crossfading product card.
- **`/guide`** ([guide/index.html](guide/index.html)) — the interactive variant: "What do you want to feel?" effect picker. Chips switch the product, aura color, real per-product Judge.me rating, and a deep-linked **Shop {Effect}** CTA (`utm_campaign=guide`, `utm_content=<effect>`), so the two pages are separable in analytics.

## Hosting
Served via **GitHub Pages** from the `main` branch (root) under the **LEVEL-JAUDE** GitHub account. The custom domain is configured by the [`CNAME`](CNAME) file.

### GoDaddy DNS (apex domain `effectsbylevel.com`)
Point the domain at GitHub Pages with these records:

| Type | Name | Value |
|------|------|-------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | level-jaude.github.io |

After DNS propagates, enable **Enforce HTTPS** in the repo's Pages settings.

## Editing
Everything lives in [`index.html`](index.html) — colors are CSS variables at the top of the `<style>` block, matching the official LEVEL Pantone palette. Edit and push to `main`; GitHub Pages redeploys automatically.
