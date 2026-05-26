---
title: "The Stack"
date: 2026-05-26
description: "Candidate UK-owned vendors across the technology stack — working draft, internal review only."
hidemeta: true
showtoc: true
---

<div style="background: #fff3cd; border: 2px solid #ffc107; border-radius: 6px; padding: 1rem 1.25rem; margin-bottom: 2rem;">
<strong>🚧 Work in progress — internal review only.</strong> This page is an early-draft mapping of candidate UK-owned vendors across the stack layers. It has <em>not</em> been validated against the certification standard, vendor ownership has not been independently verified, and entries are likely to change. Not for public consumption. Treat every entry as a hypothesis to investigate, not a recommendation.
</div>

## How to read this page

Each stack layer lists candidate UK-owned vendors that may qualify for certification. A "candidate" is a vendor that — on first inspection — appears to meet some or all of the sovereignty criteria (UK incorporation, UK ownership, UK data residency, UK-domiciled directors). Full certification requires deeper diligence on shareholder structure, supply chain, and operational control.

Where no qualifying UK vendor is known, the layer is marked **Gap**. Gaps are where the acqui-build model applies.

---

## Infrastructure layer

### Cloud, hosting and colocation

| Candidate | Notes |
|---|---|
| **Civo** | UK-based managed Kubernetes; UK data centres. |
| **Krystal** | UK-owned hosting; SME-focused; UK data centres. |
| **Mythic Beasts** | UK-owned ISP/hosting; small but reputable; UK data centres. |
| **Iomart** | UK-listed managed services; cloud and colocation. |
| **Pulsant** | UK colocation and managed services. |
| **Custodian Data Centres** | UK colocation. |
| **Memset** | UK-owned hosting (legacy presence; ownership to confirm). |

**Notes:** UKCloud (formerly the flagship UK sovereign cloud) entered administration in 2022 — the gap it left has not been fully filled. AWS UK Regions, Microsoft for Government, and Google Cloud UK do **not** qualify (US-owned, sovereignty-washing).

### DNS and domains

| Candidate | Notes |
|---|---|
| **Mythic Beasts** | DNS + domain registration. |
| **Krystal** | Domain registration. |
| **Nominet** | UK registry operator for `.uk` (not a registrar but adjacent). |

**Disqualified:** 123-reg (owned by Newfold Digital — US).

### CDN and edge

**Gap.** No significant UK-owned CDN. Cloudflare, Fastly, Akamai, BunnyCDN are all non-UK. Candidate for acqui-build or partnership.

---

## Productivity and collaboration

### Email

| Candidate | Notes |
|---|---|
| **Mythic Beasts** | Hosted email on UK infrastructure. |
| **Krystal** | Hosted email bundled with hosting. |

**Disqualified:** FastMail (Australia), ProtonMail (Switzerland), Tutanota (Germany), Google Workspace, Microsoft 365.

### Documents, sheets, slides

**Gap.** No mature UK-owned office suite. Open-source self-hosted alternatives (Nextcloud — German foundation; CryptPad — French; OnlyOffice — origin uncertain) do not meet the standard. Likely the largest single gap in the entire stack.

### Storage and file sharing

**Gap.** Self-hosted on UK infrastructure (e.g. Nextcloud on Krystal/Civo) is a workable interim — but no native UK-owned product currently competes with Dropbox or Google Drive at the SME level.

### Messaging and video

| Candidate | Notes |
|---|---|
| **Element** | UK-based, Matrix protocol; secure messaging and collaboration; used by UK government. |

**Disqualified:** Slack (US), Microsoft Teams (US), Zoom (US), Whereby (Norway).

---

## Business systems

### CRM

| Candidate | Notes |
|---|---|
| **Capsule CRM** | UK-owned (Manchester); SME-focused. |
| **Attio** | UK-owned (London); modern relationship-focused CRM; ownership and data-residency to confirm against the standard. |

**Disqualified:** Salesforce, HubSpot, Pipedrive (Estonia), Insightly. Adjacent: OnePageCRM (Ireland — not UK).

### Accounting and finance

| Candidate | Notes |
|---|---|
| **Sage** | UK-listed (Newcastle); long-established. |
| **FreeAgent** | UK-owned (Edinburgh); owned by NatWest. |
| **KashFlow** | UK-owned (owned by Iris Software Group — UK PE-backed; ownership to confirm). |
| **Crunch** | UK-owned; accounting and bookkeeping platform. |
| **Pandle** | UK-owned (free tier; SME-focused). |

**Disqualified:** Xero (New Zealand), QuickBooks (Intuit — US), Wave (US).

### Payments and banking

| Candidate | Notes |
|---|---|
| **GoCardless** | UK-owned (London); direct debit and recurring payments. |
| **Modulr** | UK-owned; payments infrastructure. |
| **Truelayer** | UK-owned; open banking. |
| **Form3** | UK-owned; payments infrastructure. |
| **Tide** | UK-owned; SME business banking. |
| **Starling Bank** | UK-owned; SME banking. |

**Disqualified:** Stripe (US), Worldpay (ownership history complex — currently US-controlled), PayPal.

### HR and payroll

| Candidate | Notes |
|---|---|
| **CharlieHR** | UK-owned (London); SME HR platform. |
| **BrightHR** | UK-owned; part of Peninsula Group. |
| **Sage Payroll** | UK-listed. |
| **PeopleHR** | UK-owned (owned by Access Group — UK PE-backed). |

**Disqualified:** PayFit (France), Personio (Germany), BambooHR (US).

### Customer support and helpdesk

| Candidate | Notes |
|---|---|
| **Halo ITSM** | UK-owned; service desk and ITSM. |
| **Hornbill** | UK-owned; service management. |

**Disqualified:** Zendesk, Intercom (Ireland — not UK), Freshdesk, HelpScout.

---

## Publishing and content

### CMS and publishing platforms

| Candidate | Notes |
|---|---|
| **Ghost** | Open-source MIT-licensed publishing platform. Ghost Foundation is non-UK (registered in Singapore), so the hosted Ghost(Pro) service does not qualify under the strict ownership standard — but a self-hosted Ghost on UK-owned infrastructure (e.g. Krystal, Civo) is an interesting edge case for the standard. Flag for tiered-certification discussion. |

**Disqualified (hosted):** WordPress.com (Automattic — US), Squarespace (US), Wix (Israeli), Webflow (US).

---

## Marketing and social

### Social media management

| Candidate | Notes |
|---|---|
| **Brandwatch** | Originally UK (Brighton) — acquired by Cision (US) in 2021. **Disqualified post-acquisition.** |

**Gap.** No significant UK-owned social media management platform at SME scale. Candidate for acqui-build.

### Analytics

**Gap.** Self-hosted Plausible or Matomo on UK infrastructure works as an interim, but no UK-owned analytics product exists at scale. GA4 (Google) dominates the market and is not replaceable on a like-for-like basis.

### Email marketing

**Gap.** Mailchimp (US, owned by Intuit), Klaviyo (US), ConvertKit (US), Brevo (France) — no UK-owned mature equivalent.

---

## AI layer

### Foundation models

**Gap (transitional).** No UK-owned frontier foundation model exists. The April 2026 Sovereign AI Fund is seeding the next generation: Callosum, Primamente, Doubleword AI, Cosine, Cursive AI, Odyssey Systems, Twig Bio. Sovereign Tech Stack proposes a **sovereign-aligned transitional category** for Fund-backed UK AI vendors while UK frontier capability matures.

### Applied AI and tooling

| Candidate | Notes |
|---|---|
| **Stability AI** | UK Ltd registration; ownership structure complex; image generation. |
| **Synthesia** | UK-owned (London); AI video generation. |
| **Wayve** | UK-owned (London); autonomous driving (not SME-applicable today). |
| **ElevenLabs** | UK/US dual-headquartered; ownership status to confirm. |
| **Faculty AI** | UK-owned (London); enterprise AI consulting and platform. |
| **Quantexa** | UK-owned (London); decision intelligence platform. |

---

## Development and engineering

### Source control and CI/CD

**Gap.** GitHub (Microsoft — US), GitLab (US, with remote teams), Bitbucket (Atlassian — Australia), Codeberg (German non-profit). No UK-owned alternative at scale. Self-hosted Gitea or Forgejo on UK infrastructure is a workable interim for in-house teams.

### Project management

**Gap.** Linear (US/Sweden), Asana (US), Monday (Israeli), ClickUp (US), Trello (Atlassian — Australia), Notion (US). No UK-owned mature equivalent.

---

## Gap summary

The largest structural gaps — where no qualifying UK vendor currently exists at SME scale — are:

1. **CDN and edge**
2. **Office productivity** (docs, sheets, slides)
3. **File storage and sharing**
4. **Email marketing and automation**
5. **Social media management** (post-Brandwatch acquisition)
6. **Project management and task tracking**
7. **Source control and CI/CD**
8. **Frontier AI foundation models** (mitigated transitionally via Sovereign AI Fund alignment)

These are the candidates for the acqui-build component of the platform — categories where curation alone cannot deliver a complete certified stack.

---

## What this page is not

This is not the certified vendor directory. It is a working hypothesis list. Every entry needs:

- Independent verification of UK ownership (Companies House + shareholder structure)
- Verification of UK data residency and hosting
- Supply-chain transparency assessment
- Director domicile confirmation
- Operational-control review (especially for PE-backed entities with offshore structures)

Entries marked "to confirm" or with ownership flagged should be treated as provisional. Disqualifications listed here are first-pass assessments based on parent-company nationality — formal disqualification requires the full standard review.
