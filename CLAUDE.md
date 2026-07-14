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
- Hosting: Cloudflare Pages (or Cloudflare + GitHub Actions)
- Code: Pure HTML/CSS/JS — no page builders, no CMS
- DNS: carapp.pro (domain owner: CarApp — credentials pending)
- Repo: GitHub (BONAPARTE-managed)

## Key Contacts
| Name | Role | Contact |
|------|------|---------|
| Gonzalo Perez Dematteis | CarApp founder (AR) | gpd2703@gmail.com |
| Sebastian Fernandez | CarApp founder (UY) | sebastian@tupaseapp.com / sebastian.f.fernandez@gmail.com |
| Martin Alcalde | Dev — Bubble apps | martin@ataraxydigital.com |

## Project Status
- [ ] Domain access to carapp.pro granted to BONAPARTE (BLOCKER)
- [ ] Martin migrates apps to argentina.carapp.pro / uruguay.carapp.pro
- [ ] BONAPARTE builds country selector (carapp.pro/)
- [ ] BONAPARTE builds Argentina landing (carapp.pro/es-ar/)
- [ ] BONAPARTE builds Uruguay landing (carapp.pro/es-uy/)
- [ ] Cloudflare DNS configured
- [ ] Ad pixels + UTM tracking wired up

## Important Context
- Do NOT use carappar.com for the marketing site. That domain exists but was rejected to avoid split-domain SEO issues.
- The Bubble apps live on subdomains — BONAPARTE does not touch those.
- Each country needs its own landing page (different copy, pricing, value props may differ).
- Ads accounts (Meta + Google) are already set up and ready by BONAPARTE — waiting on site to launch.
- CarApp AR and UY are separate apps (clones) with separate ad campaigns.

## BONAPARTE Contact
- Guido Rossetti — guido@bonapartedigital.com
