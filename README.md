# carapp.pro

Marketing site for CarApp — vehicle classifieds marketplace operating in Argentina and Uruguay.

Built by [BONAPARTE](https://bonapartedigital.com).

---

## Structure

```
carapp.pro/          Country selector
carapp.pro/es-ar/    Argentina landing page
carapp.pro/es-uy/    Uruguay landing page
```

The marketplace apps (Bubble) live on `argentina.carapp.pro` and `uruguay.carapp.pro` — separate repo, managed by Ataraxy Digital.

## Stack

- HTML / CSS / JS
- Cloudflare Pages
- No frameworks, no builders

## Setup

```bash
git clone https://github.com/bonapartedigital/carapp-pro.git
cd carapp-pro
# open index.html in your browser or use a local server
npx serve .
```

Deployment is automatic via Cloudflare Pages on push to `main`.
