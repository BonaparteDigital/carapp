<p align="center">
  <img src="assets/bonaparte-logo.svg" alt="BONAPARTE" width="240">
</p>
<p align="center"><em>Your Growth Starts Here.</em></p>

# carapp.pro

Marketing site for CarApp — vehicle classifieds marketplace operating in Argentina and Uruguay.

Built by [BONAPARTE](https://bonapartedigital.com).

---

## Structure

```
src/                  Eleventy source
src/index.njk         carapp.pro/         — Country selector
src/es-ar/index.njk   carapp.pro/es-ar/   — Argentina landing page
src/es-uy/index.njk   carapp.pro/es-uy/   — Uruguay landing page
src/_includes/        Shared layout, header, footer (consistent across all landing pages)
src/css/              Site styles
src/assets/           Images (CarApp + BONAPARTE logos)
_site/                Build output (generated, gitignored)
```

The marketplace apps (Bubble) live on `argentina.carapp.pro` and `uruguay.carapp.pro` — separate repo, managed by Ataraxy Digital.

## Stack

- [Eleventy (11ty)](https://www.11ty.dev/) — build-time templating only, ships zero client-side JS/framework runtime. Used so every landing page shares the same header/footer instead of hand-copy-pasted HTML.
- Cloudflare Pages — build command `npx @11ty/eleventy`, output directory `_site`
- No CMS

## Fonts

- **Primary:** [Mulish](https://fonts.google.com/specimen/Mulish) — Regular, Italic, Bold, Black
- **Secondary:** [Raleway](https://fonts.google.com/specimen/Raleway) — Regular, Italic, Bold, Black (avoid for numerals — Raleway's digit spacing is irregular; use Mulish for any numeric content)

## Setup

```bash
git clone https://github.com/BonaparteDigital/carapp.git
cd carapp
npm install
npm start   # local dev server with live reload
npm run build   # outputs static site to _site/
```

Deployment is automatic via Cloudflare Pages on push to `main`.
