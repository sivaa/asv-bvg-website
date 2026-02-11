# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static website for **ASV-BVG e.V.**, a fishing club (_Angelsportverein_) in Berlin-Lichterfelde. Pure HTML/CSS with ~30 lines of vanilla JS (hamburger menu only). No build step, no frameworks, no package manager.

```
┌─────────────────────────────────────────────────────────┐
│  Architecture: Zero-dependency static site              │
│                                                         │
│  index.html ─────┐                                      │
│  pages/           │    css/style.css                     │
│    impressum.html ├──▶ (single stylesheet, mobile-first)│
│    datenschutz.html│                                     │
│  404.html ───────┘    images/ (favicon, logo, icons)    │
│                                                         │
│  Hosting: Vercel (auto-deploy on push to main)          │
│  Domain target: asv-bvg.de                              │
└─────────────────────────────────────────────────────────┘
```

## Development

**Local server** (any static file server works):

```bash
python3 -m http.server 8000
# or
npx serve .
```

Note: Python's dev server won't serve the custom `404.html` — that's Vercel-specific routing. Test 404 behavior on Vercel preview deployments.

**Deploy:** Commit and push directly to `main` — Vercel auto-deploys. No build command needed. No PRs, no feature branches. All changes go straight to `main`.

**Vercel Account & Credentials:**

```
┌──────────────────────────────────────────────────────────┐
│  Account:  sivasubramaniama-7684                         │
│  Team:     siva-as-projects-628a5fc6                     │
│  Token:    .env file (VERCEL=<token>)                    │
│  URL:      https://asv-bvg-website.vercel.app            │
│                                                          │
│  ⚠️  ALWAYS use --token from .env for Vercel CLI calls   │
│  The default CLI login (siva-7663) is a DIFFERENT account│
│  and does NOT have this project.                         │
└──────────────────────────────────────────────────────────┘
```

Usage: `npx vercel --token=$(grep VERCEL .env | cut -d= -f2)`

## Design System

```
┌────────────────────────────────────────────────────┐
│  Colors                                            │
│  Background:   #EBE8E6  (warm beige)               │
│  Text:         #1D1F25  (dark charcoal)            │
│  Accent:       #A04535  (terracotta, WCAG AA)      │
│  Accent hover: #8B3A2C  (deep rust)                │
│                                                    │
│  Typography                                        │
│  Font: Readex Pro (Google Fonts, non-blocking)     │
│  Fallback: system stack                            │
│  Size: 18px base, line-height 1.75                 │
│                                                    │
│  Breakpoints (mobile-first)                        │
│  Default    → mobile (<768px)                      │
│  768px      → tablet (nav becomes inline)          │
│  1024px     → desktop                              │
│                                                    │
│  Layout                                            │
│  max-width: 800px, centered                        │
│  Padding: clamp(1.75rem, 6vw, 3rem)               │
└────────────────────────────────────────────────────┘
```

## Core Rule: Never Regress Scores

Every change MUST improve (or at minimum maintain) Core Web Vitals and SEO scores. Never introduce changes that decrease Lighthouse Performance, Accessibility, Best Practices, or SEO scores. If a change risks regressing any metric, don't make it.

## Architecture Constraints

- **All content is in German** — page titles, nav labels, ARIA labels, legal text
- **No hero section, no colored blocks, no dark footer** — unified beige background everywhere
- **Links must have underlines** (WCAG SC 1.4.1 accessibility requirement)
- **CTA = text link with arrow** (`→`), never a button
- **Nav structure is critical:** `nav-links` (`<ul>`) must be INSIDE `nav-inner` (`<div>`) for flex-wrap alignment. Breaking this nesting breaks the hamburger menu layout.
- **Google Maps uses click-to-load** (two-click consent). Data only transfers to Google after user clicks "Google Maps laden". Datenschutz page documents this.
- **`noindex, nofollow`** is set only on `404.html` (error pages). All content pages are indexed.
- **All pages duplicate** the nav/footer HTML and the hamburger JS inline — there's no templating system. Changes to shared elements must be applied to all 4 HTML files.

## File Conventions

| File | Purpose |
|------|---------|
| `index.html` | Single-page home (sections: willkommen, ueber-uns, mitglied-werden, kontakt) |
| `pages/impressum.html` | Legal: Impressum (DDG §5 / MStV §18) |
| `pages/datenschutz.html` | Legal: Datenschutzerklärung (DSGVO) |
| `404.html` | Custom error page (root-level for Vercel) |
| `css/style.css` | All styles — mobile-first with tablet/desktop media queries + print stylesheet |
| `docs/DELIVERABLE.md` | Project handoff document for the club board |
| `robots.txt` | Search engine directives |
| `sitemap.xml` | Site map for search engines (URLs use `asv-bvg.de` domain) |

## Link Paths

From `index.html` and `404.html` (root): link to legal pages as `/pages/impressum.html`.
From `pages/*.html`: footer links use relative paths `impressum.html`, `datenschutz.html`. Nav links back to index use `/#section-id`.
All asset paths (`/css/style.css`, `/images/*`) are root-relative.
