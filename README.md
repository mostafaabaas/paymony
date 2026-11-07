# Paymony — paymony.net (static landing site)

The fintech UGC desk of **influUGC**. Built Nov 6, 2026. **Files only — not deployed.**

## ⚠️ Content model + design direction (owner orders, Nov 5–6, 2026)

- **Content-first (owner update, Nov 6, 00:24):** network sites must NOT be pure
  company brochures. They lead with useful **content** — tips, guides and
  information that search engines and AI answers surface and that brings
  traffic — with influUGC's services and real work woven inside the content,
  and the central CTAs doing the conversion. This site applies the model: the
  homepage carries a full **"Guides for fintech marketers"** section
  (3 substantive starter guides, below) ahead of the services list, and each
  guide closes with a soft woven-in influUGC line + the standard central CTA.
- **Identity (owner order, Nov 5, 23:57):** ALL network satellite sites use the
  main influUGC identity — black background `#000`, neon lime accent `#C8FF00`,
  dark panels, bold heavy typography, the www.influugc.com feel.
- Brand lockup: `Paymony.` wordmark with the subline "UGC & content for
  fintech by influUGC" (Arabic: «UGC ومحتوى للفينتك من influUGC»).
- Only real company data: est. 2020, Arab League St Agouza (Giza 12651),
  Egypt + Saudi/Gulf, real client names (Riyadh Season, Saudi Tourism
  Authority, flynas, Saudia, realme, Domino's, TikTok Live, Zanussi).
  No prices, no invented figures or statistics, no testimonials, no stock
  imagery (CSS/text only).

## ⚠️ Fintech claims discipline (site-wide, no exceptions)

- **NO financial claims and NO promised outcomes anywhere on this site** —
  no promised returns, no profit claims, no "guaranteed" anything, no
  earnings language, no invented rates/figures. The site's own copy states
  this rule explicitly (FAQ #2, services intro, footer note).
- The guides present **general good-practice principles only** and say so —
  they are **not legal advice**; each brand's compliance team and market
  regulator have the final word (stated on the guides section intro).
- The site states plainly that influUGC/Paymony is a **content agency, not
  a financial adviser** (Why section + footer note).

## Pages built (3 HTML pages, 2 languages)

| File | What |
|---|---|
| `index.html` | English-first landing (LTR): hero, client proof strip, **Guides for fintech marketers** (3 starter guides, anchor-linked), 5 services (app-demo UGC, trust-building creator content, onboarding explainers, launch & feature content, monthly packs), 4-step how-it-works (incl. compliance review gate), deliverables checklist, why influUGC (with the in-body editorial link to influugc.com), 6-question answer-first FAQ, contact/CTA band, network footer. |
| `ar.html` | Full Arabic mirror (RTL), same structure, guides and FAQ. |
| `404.html` | Branded not-found page (English). |

Plus: `styles.css`, `favicon.svg` (black + lime PM mark), `sitemap.xml`
(hreflang-annotated), `robots.txt`, `llms.txt`, `render.yaml`.

### The 3 starter guides (on-page sections, both languages)

1. `#guide-trust` — **UGC for finance apps — the trust rules**: never promise
   returns/profits/outcomes; demonstrate real flows, never project results;
   risk and fee language in plain words; claims only from published product
   documentation as compliance approved; disclose the partnership; one
   accountable reviewer (the brand's compliance/legal review before
   publishing).
2. `#guide-demo` — **How to demo a payment app on camera without exposing
   real money or data**: test/demo/sandbox or dedicated staged accounts
   only; staged balances/amounts; notifications silenced; frame cleaned
   before recording; OTPs, PINs, full card numbers, IBANs, real-account QR
   codes and real customer data never on camera; frames checked before
   delivery; staged credentials rotated/closed after the campaign.
3. `#guide-brief` — **Creator briefs for fintech — the compliance
   checklist**: the approved claims list (only stateable facts; licence/
   regulatory wording exactly as approved), the never-say list, disclosure
   written into the brief, and the approval gate (draft → brand compliance
   review → corrections → publish) for every format incl. stories; usage
   scope settled in the same document.

Each guide ends with a soft woven-in line (influUGC runs exactly this for
fintech clients) + the standard book/WhatsApp CTAs with `utm_source=paymony`.

## SEO / GEO

- Canonical base `https://paymony.net/` (the real domain; if this site is
  first deployed to an `onrender.com` URL before the domain attaches, switch
  all canonical/OG/sitemap/robots/llms bases in one pass, same as the
  ugccompany rule in `../DEPLOY.md` §2).
- Title/meta target "UGC & content marketing for fintech" + Egypt /
  Saudi Arabia in both languages; OpenGraph + Twitter cards; hreflang
  ar/en both ways.
- JSON-LD: `Organization` (with `parentOrganization: influUGC`, postal
  address, areaServed, the four real social profiles), `WebSite`, and
  `FAQPage` matching each page's visible FAQ.

## CTAs (both carry the satellite UTM set)

- Booking → `https://www.influugc.com/book?utm_source=paymony&utm_medium=satellite&utm_campaign=network`
- WhatsApp (client line) → `https://wa.me/201029979797?utm_source=paymony&utm_medium=satellite&utm_campaign=network`
- Footer legal line: "Part of the influUGC network" linking to the hub.

## What remains (not done here)

1. **Deploy** — static folder; Render Static Site (free tier per the network
   rule). The repo's `render.yaml` blueprint pre-fills the service name
   (`paymony`) and publish path (`.`). Live since Nov 6, 2026 at
   https://paymony-7t51.onrender.com — Render suffixed the service name
   (`paymony` was already taken), so the plain `paymony.onrender.com` URL
   does NOT resolve; the live URL is the suffixed one.
2. **Domain attach** — point `paymony.net` DNS at the host (same checklist
   pattern as `../DEPLOY.md` §4: apex A + www CNAME from the host's screen;
   no MX changes — mail stays on influugc.com).
3. **Marketplace note:** paymony.net was pulled from the $200 sale tier into
   the network by the owner's Nov 6 activation order — if a $200 listing
   still exists anywhere for it, it must come off before traffic is pointed
   at the domain.
4. After go-live: dedicated Google Search Console property + submit
   `sitemap.xml`; verify both pages return 200, the guides render, and the
   FAQ matches the JSON-LD.

## Deploy status (Nov 6, 2026)

- **Repo**: https://github.com/mostafaabaas/paymony (PUBLIC from birth, per
  the Nov 6 activation design; branch `main`) — source pushed Nov 6, 2026.
- **Hosting**: PENDING-DASHBOARD — the Render Static Site service has **not**
  been created yet; creation happens in the parent activation wave.
