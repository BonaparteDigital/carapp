# CarApp Marketing Site — Project Brief

## What This Is
Marketing frontend for CarApp — a vehicle classifieds marketplace launching in Argentina and Uruguay. Built and maintained by BONAPARTE. Deployed on carapp.pro.

## The Problem We're Solving
CarApp's current setup has the marketplace (app) and marketing pages mixed under the same domain via Bubble. Bubble is a no-code builder — bad for SEO, slow to load, and limits what we can do with tracking and conversion optimization. BONAPARTE is building a clean, fast, code-first marketing site that handles discovery and conversion, while the Bubble apps handle the actual marketplace functionality.

## URL Structure
| URL | What it is |
|-----|-----------|
| `carapp.pro/` | Country selector — user picks AR or UY |
| `carapp.pro/es-ar/` | Argentina marketing landing page |
| `carapp.pro/es-uy/` | Uruguay marketing landing page |
| `argentina.carapp.pro/` | Argentina marketplace app (Bubble — not our code) |
| `uruguay.carapp.pro/` | Uruguay marketplace app (Bubble — not our code) |

## Scope (BONAPARTE)
- Country selector homepage
- Argentina landing page
- Uruguay landing page
- DNS / Vercel domain configuration
- Pixel setup (Meta + Google) per country
- UTM tracking implementation

## Out of Scope
- The Bubble marketplace apps (Ataraxy Digital handles those)
- Backend / database
- User auth, listings, payments

## Stack
- Eleventy (11ty) build-time templating — output is plain HTML/CSS, no client-side framework runtime
- Vercel for hosting (team: Bonaparte), Git-connected — `master` deploys to production (`carapp.pro`), other branches get preview URLs
- GitHub for version control
- No CMS, no page builders

## Why carapp.pro (not separate domains)
Keeping Argentina and Uruguay under the same root domain preserves SEO authority, avoids backlink fragmentation, and means one Vercel project, one GitHub repo, one place to manage DNS. Switching domains after launch costs months of ranking recovery — decision is final.

## Client
CarApp — Gonzalo Perez Dematteis & Sebastian Fernandez
