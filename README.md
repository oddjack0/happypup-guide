# HappyPup Guide

Dog-care information site — long-tail training & behaviour guides that funnel to Ko-fi printable trackers/guides and the Dogs 2027 calendar. Site #3 in `~/workspace/MASTER-PLAN.md` (see `../MASTER-PLAN.md`, section 3). Team roles: `TEAM.md`.

## What this is

- **Offer:** Step-by-step guides — puppy training basics, crate training, potty training on a schedule, loose-leash walking, separation anxiety — plus printable-help cross-sells.
- **Phase 1 money:** Ko-fi shop (printable tracker/checklist pack) and the Dogs 2027 Calendar ($8, https://ko-fi.com/s/ce961ba7b0).
- **Phase 2 (needs Bruno's approval, only with traffic):** Chewy affiliate (4%), AdSense (~$8–11 page RPM, pets).
- **Kill condition:** No guide in Google top-50 AND <10 Ko-fi clicks in 90 days → pause content, keep as brochure for the dog products.

## Build

Pure static HTML/CSS in `site/` — no build step, no CDNs, no external fonts or images (inline SVG decoration only). Semantic, accessible, mobile-responsive. Per-page meta descriptions + Open Graph tags, `sitemap.xml`, `robots.txt`.

| File | Purpose |
|---|---|
| `site/index.html` | Homepage: hero, 5 guide cards, printables section, calendar promo, disclaimer |
| `site/guide-puppy-training.html` | Guide 1 — first two weeks, first three skills, sample day |
| `site/guide-crate-training.html` | Guide 2 — sizing, day-by-day intro plan, time limits by age |
| `site/guide-potty-training.html` | Guide 3 — schedule, trip protocol, accident protocol |
| `site/guide-leash-pulling.html` | Guide 4 — stop-start method, gear, 4-stage plan |
| `site/guide-separation-anxiety.html` | Guide 5 — signs checklist, graduated absences, when to escalate |
| `site/styles.css` | Shared stylesheet |
| `site/sitemap.xml`, `site/robots.txt` | SEO plumbing |

Canonical base URL assumed for OG/sitemap: `https://oddjack0.github.io/happypup-guide/` (GitHub Pages pattern, same as oddjack-art). Update those absolute URLs if the repo/domain differs at deploy time.

## Content rules

- General information only — **never veterinary or medical advice**. Every page carries the disclaimer; guides name vet/certified-trainer (CPDT-KA, IAABC) escalation points.
- YMYL-adjacent: no miracle promises, realistic timelines, human-style accuracy QA pass before publishing anything new.
- Reward-based methods only; aversive tools (choke/prong/shock) are recommended against.

## Status

Built 2026-10-20 by the Site Lead. **Not deployed** — deploy (GitHub Pages repo under oddjack0, verify locally first) happens on Bruno's go per the master plan. Promotion is Pinterest-first (Growth & Monetization role).
