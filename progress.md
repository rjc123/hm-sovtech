# Sovereign Tech Stack Hugo Site — Ralph Progress Log

## 2026-04-28 — pa-ilb6.26.6 — Theme re-architecture: sam → PaperMod

**Task:** Re-architect site content around a UK theme/sub-theme. Switch from the sam theme to PaperMod.

**What was done:**

- Added PaperMod as a git submodule at `themes/PaperMod` (git submodule add --depth=1 from github.com/adityatelange/hugo-PaperMod)
- Rewrote `config.toml` to use PaperMod with full B2B nav: The Case / The Platform / The Market / News / About / Join Us
- Configured `homeInfoParams` for PaperMod's hero-style homepage (no posts feed, just info panel)
- Updated all content files with proper PaperMod frontmatter (hidemeta, showtoc, description)
- Created `assets/css/sovereign.css` — Union Jack palette: navy `#00247D`, red `#CF142B`, gold `#B8A355`
- Created `layouts/partials/extend_head.html` to inject custom CSS with fingerprinting
- Disabled theme toggle (light-only, B2B appropriate)
- All 5 existing content pages preserved and adapted: _index.md, the-case.md, the-platform.md, the-market.md, about.md

**Decisions:**
- PaperMod chosen over Ananke: cleaner, more minimal, better suited to B2B certification platform; avoids the editorial/blog aesthetic of Ananke
- homeInfoParams mode (not profile/index_profile) — avoids avatar image requirement and is more appropriate for a corporate site
- Nav added News and Jobs items ahead of those tasks being built — menus are configured in config.toml ready for content

**Build state:** clean — 14 pages, no errors, no warnings

**Next engineer:** Tasks pa-ilb6.26.7 (About/Team), pa-ilb6.26.8 (Jobs/Careers), pa-ilb6.26.9 (News) are next in sequence. All are independent — any order works.

---

## 2026-04-28 — pa-ilb6.26.7 — About/Team page with placeholder leader profiles

**Task:** Add Team page with placeholder senior leader profiles and grey SVG headshot.

**What was done:**

- Created `static/images/placeholder-headshot.svg` — grey silhouette SVG (head + shoulders), used for all three roles
- Created `content/team.md` — Leadership Team page with 3 placeholder profiles: CEO, Head of Vendor Certification, Head of Strategic Partnerships
- Each profile uses the shared SVG headshot, a "Position Vacant — Recruiting Now" status badge, and a substantive placeholder bio
- Added Team to nav in config.toml (weight 55, between About and Join Us)
- Updated `about.md` to reference the Team page
- Enabled `markup.goldmark.renderer.unsafe = true` in config.toml to allow inline HTML (used for CSS grid layout of cards)
- mailto link on team page includes subject and body per convention

**Decisions:**
- Used inline HTML/CSS for the team card grid layout — PaperMod has no built-in card shortcode; inline HTML is the cleanest approach for a single page
- 3 roles created (CEO, Head of Vendor Certification, Head of Strategic Partnerships) per task spec — Head of SME Sales is assigned to the Jobs page (pa-ilb6.26.8) per task breakdown

**Build state:** clean — 15 pages, no errors, no warnings

**Next engineer:** pa-ilb6.26.8 (Jobs/Careers) and pa-ilb6.26.9 (News) remaining.
