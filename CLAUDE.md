# CarApp Marketing Site — CLAUDE.md

## Project Overview
Marketing website for CarApp, a vehicle marketplace operating in Argentina and Uruguay. BONAPARTE builds and owns the marketing frontend. The app itself (marketplace) runs on Bubble and is maintained by Ataraxy Digital (Martin Alcalde).

## Domain Architecture
```
carapp.pro/              → Country selector (homepage)
carapp.pro/es-ar/        → Argentina marketing landing page
carapp.pro/es-uy/        → Uruguay marketing landing page
argentina.carapp.pro/    → Argentina app (Bubble — Ataraxy Digital)
uruguay.carapp.pro/      → Uruguay app (Bubble — Ataraxy Digital)
```

## Stack
- Hosting: Vercel (team: Bonaparte). Git-connected to this repo — `master` is the Production Branch (`carapp.pro`), other branches deploy as Previews. Preview alias: `carapp-pi-pied.vercel.app`.
- Build: Eleventy (11ty) — build command `npx @11ty/eleventy`, output directory `_site`
- Code: HTML/CSS/JS via Eleventy templating — no CMS
- DNS: carapp.pro — domain access granted, confirmed live and pointed at Vercel as of 2026-07-21
- Repo: GitHub (BONAPARTE-managed), BonaparteDigital/carapp

## Key Contacts
| Name | Role | Contact |
|------|------|---------|
| Gonzalo Perez Dematteis | CarApp founder (AR) | gpd2703@gmail.com |
| Sebastian Fernandez | CarApp founder (UY) | sebastian@tupaseapp.com / sebastian.f.fernandez@gmail.com |
| Martin Alcalde | Dev — Bubble apps | martin@ataraxydigital.com |

## Project Status
- [x] Domain access to carapp.pro granted to BONAPARTE
- [x] BONAPARTE builds country selector (carapp.pro/) — live, flags link directly to argentina.carapp.pro / uruguay.carapp.pro
- [x] Vercel connected: production → carapp.pro (master branch), preview → carapp-pi-pied.vercel.app
- [ ] Martin migrates apps to argentina.carapp.pro / uruguay.carapp.pro
- [ ] BONAPARTE builds Argentina landing (carapp.pro/es-ar/) — placeholder only, not linked from selector
- [ ] BONAPARTE builds Uruguay landing (carapp.pro/es-uy/) — placeholder only, not linked from selector
- [ ] Ad pixels + UTM tracking wired up

## Important Context
- Do NOT use carappar.com for the marketing site. That domain exists but was rejected to avoid split-domain SEO issues.
- The Bubble apps live on subdomains — BONAPARTE does not touch those.
- Each country needs its own landing page (different copy, pricing, value props may differ).
- Ads accounts (Meta + Google) are already set up and ready by BONAPARTE — waiting on site to launch.
- CarApp AR and UY are separate apps (clones) with separate ad campaigns.

## BONAPARTE Contact
- Guido Rossetti — guido@bonapartedigital.com
