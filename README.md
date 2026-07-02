# Masul Digital — Landing Page

A single-file, self-contained landing page for **masuldigital.co.uk**, live now
while the full multi-page site (`../masul-digital-site`) finishes testing.

## What it is
- One `index.html` with inline CSS/JS — no build step, no external CSS dependency
  (only Google Fonts: Poppins / Jost / JetBrains Mono).
- Exact brand reused from the main site: teal `#0087A8`, the arch "bridge" mark,
  light + dark (Masul Ink) themes with a toggle.
- **Live page is a minimal, single-screen coming-soon**: animated Falcon "orb", a
  "Launching soon · in final testing" pill, the *"AI front office … almost here"*
  headline, a notify-me email capture, WhatsApp/email, and a Masul Group endorsement.
- Primary CTA → WhatsApp (`+44 7375 440623`); secondary → `info@masuldigital.co.uk`.
- SEO: meta + Open Graph + Twitter + JSON-LD `ProfessionalService`, robots, sitemap.

## Structure
```
index.html                 LIVE — original minimal coming-soon (almost-here)
full-landing.html          Full marketing landing — swap in post-launch
landing-full-comingsoon.html  Full landing + coming-soon framing (backup)
coming-soon.html           Source of index.html (pre-bugfix), kept for reference
assets/                    Brand mark (SVG), favicon, mark-512, brand/ = Masul Group lockups
vercel.json                Clean URLs + security headers (matches main site)
robots.txt / sitemap.xml
```

## Deploy
Static — no build. Either:
- Push to a GitHub repo and connect to Vercel (Framework: **Other**), or
- From this folder: `vercel --prod` (Vercel CLI session `ibrahim-8743`).

Point `masuldigital.co.uk` at this project for the launch window, then switch the
domain to the full site once it passes tests.
