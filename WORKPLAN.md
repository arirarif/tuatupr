# túatú PR — Static HTML Mockup Workplan

**Goal:** Impress client `abundant_attrac` (tuatupr.com) with a static HTML preview of their Squarespace → WooCommerce migration. Match current pattern (black + gold + serif), modernize execution. Deliver 3 pages: Home, Shop, Product.

**Folder:** `mockup/`
**Status convention:** `[ ]` pending · `[~]` in progress · `[x]` done

---

## 0. Source of truth & content vault

### Brand kit (locked)
- **Colors:** `--black: #0A0A0A`, `--gold: #C8A04E`, `--gold-dark: #A8842F`, `--gold-soft: #F5EBD3`, `--bg-soft: #FAF8F3`, `--ink: #1A1A1A`, `--muted: #6B7280`, `--line: #E7E4DC`
- **Fonts:** Headings = Playfair Display (serif), Body = Inter (sans). Load from Google Fonts.
- **Logo:** Text-based `túatú PR` with circular black mark "t" in gold. (Hotlinking Squarespace CDN logo is unreliable — text logo is safer.)
- **Pattern matched from tuatupr.com:** Black hero, gold accent links, serif headings, country product grid, 4-tier pricing (Essential / Standard / Pro / Enterprise), guaranteed-publication messaging, EN/ES/ZH languages.

### Files
```
mockup/
├── WORKPLAN.md           ← this file (kept up to date as work progresses)
├── index.html            ← Home
├── shop.html             ← Country shop archive
├── product.html          ← Spain single product
└── assets/
    └── styles.css        ← shared (already built)
```

### Nav (all pages)
- Announcement bar: `✓ Guaranteed publications  ·  ⚡ 48–72h delivery  ·  🌍 12+ countries`
- Logo · Services · Shop · Blog · About · Contact · [EN | ES | 中文] · [Start now →]

### Footer (all pages)
- Brand col: logo + tagline + socials (FB, LinkedIn, X, YT)
- Services col: Press Release Distribution, Media Relations, Online Communication, SEO/SEM, Web Design
- Company col: About, Blog, Case Studies, Careers, Press
- Contact col: Calle Canteras de Tilly 3, 1ºC, Madrid · +34 692 037 728 · info@tuatupr.com
- Bottom: © 2026 túatú PR · Aviso Legal · Privacidad · Cookies

### Content vault — extracted from tuatupr.com
**Hero (Home):**
- H1: `INTERNATIONAL PRESS RELEASE DISTRIBUTION` with italic gold accent on `with guaranteed publications`
- Lead: `Get your press release published in trusted media outlets across Europe and LATAM. 100% guaranteed placements. Delivered in 48–72 hours.`
- CTAs: `Start your distribution now` (primary) · `See country pricing` (ghost)
- Stats: `12+ Countries · 391 Publications delivered · 100% Placement guarantee · 48–72h Turnaround`

**Trust strip:** `EL PAÍS · LA REPUBBLICA · LE MONDE · DIE WELT · THE GUARDIAN · O GLOBO · EL UNIVERSAL`

**Countries — live (6):**
| Country | Region | From  | Slug   | Flag bg key |
|---------|--------|-------|--------|-------------|
| Spain   | Europe | €100  | spain   | spain   |
| Portugal| Europe | €125  | portugal| portugal|
| Germany | Europe | €260  | germany | germany |
| Italy   | Europe | €290  | italy   | italy   |
| France  | Europe | €350  | france  | france  |
| UK      | Europe | €395  | uk      | uk      |

**Countries — coming soon (5):**
Mexico · Colombia · Argentina · Brazil · Chile (all LATAM)

**Country one-liners:**
- Spain: `Get featured in major Spanish media — 100% guaranteed placements. You choose how many publications.`
- Portugal: `Published in trusted Portuguese media. 100% guaranteed. One simple plan, complete visibility.`
- Germany: `Appear in trusted German media with guaranteed results. No exceptions — your release is published.`
- Italy: `Get published in relevant Italian media outlets. 100% guaranteed placements.`
- France: `Get published in relevant French media outlets. You choose how many publications.`
- UK: `Reach national and local UK audiences via reputable digital outlets. Every placement guaranteed.`

**How it works (3 steps):**
1. **Pick your country & tier** — Choose where you want coverage and how many publications.
2. **Send your story (or we write it)** — Upload your draft or get our newsroom to write it for you.
3. **Live in 48–72 hours** — Approved, distributed, and published in guaranteed outlets. Full report sent.

**Services (4 cards for home preview):**
- 🌍 Press Release Distribution — Guaranteed placements across 12+ countries
- 📰 Media Relations — Expert pitching to top-tier journalists
- 💻 Online Communication — Digital PR, content & community management
- 📊 SEO & Online Advertising — Performance-driven campaigns

**Testimonial:**
> *"I hired túatú for help with the distribution of a press release in LATAM, and the results were great. We exceeded our expected number of publications and achieved regional media coverage quickly. The process was fast and seamless."*
> — **Veronica Santana**, Director Brand Marketing · Zumba Fitness, LLC

**FAQ (5 items — from tuatupr.com):**
1. *Where will my press release be published?* — In relevant local and national media outlets matching the country/tier you choose. Full media list provided before distribution.
2. *When will my press release be published?* — 48–72 hours after payment and content approval (excluding weekends and holidays).
3. *Can I add photos or videos?* — Yes. One main image + two contextual images are included. Video coverage requires prior consultation.
4. *Can I send a pre-written press release?* — Yes — or our newsroom can write it for you in English, Spanish or Chinese. Translation included.
5. *Are any topics restricted?* — Some require pre-approval: crypto/blockchain, legal matters, restricted healthcare, weapons, dating services, and political content during election periods.

**Spain product page — pricing tiers (derived progressively, sensible variation pricing):**
| Tier        | Price | Publications | What's included |
|-------------|-------|--------------|-----------------|
| Essential   | €100  | 5 outlets    | 1 country, 1 language, standard outlets, email report |
| Standard ★  | €290  | 15 outlets   | + mid-tier regional press, 1 main image, social mention |
| Pro         | €590  | 30 outlets   | + national press, 2 images, SEO optimization, 3 backlinks |
| Enterprise  | €990  | 60 outlets   | + tier-1 outlets (El País, ABC), video embed allowed, dedicated account manager, full PDF report |

**Spain example media outlets (Media tab):**
- El País (Pro+) · ABC (Pro+) · La Vanguardia (Standard+) · El Mundo (Pro+) · 20 Minutos (Essential+)
- Expansión (Pro+) · El Economista (Standard+) · Cinco Días (Standard+)
- Marca (Pro+) · El Confidencial (Pro+) · Europa Press (Enterprise) · EFE (Enterprise)

**Spain trust badges (under add-to-cart):**
- 🛡 100% placement guarantee · ⚡ 48–72h delivery · 🔒 Stripe + PayPal · 💼 Invoice available

**Spain urgency line:** `🟢 Order before 18:00 CET today for publication this week.`

---

## 1. Build order (todo)

### A. Home page (`index.html`) — ✅ DONE
- [x] A1 — Page shell + announcement bar + sticky nav + lang switcher
- [x] A2 — Hero
- [x] A3 — Trust strip
- [x] A4 — Country grid (6 live + 5 coming-soon)
- [x] A5 — How-it-works
- [x] A6 — Services preview
- [x] A7 — Testimonial
- [x] A8 — FAQ
- [x] A9 — CTA banner + footer

### B. Shop page (`shop.html`) — ✅ DONE
- [x] B1 — Page shell + page hero + breadcrumb
- [x] B2 — Sidebar filters (Region, Price, Language, Tier, Availability)
- [x] B3 — Toolbar + 11-card country grid + pagination
- [x] B4 — CTA banner + footer (reuse)

### C. Product page (`product.html` — Spain) — ✅ DONE
- [x] C1 — Shell + breadcrumb (Home › Shop › Europe › Spain)
- [x] C2 — Gallery (Spain flag main + 4 thumbnails)
- [x] C3 — Product info, h1, rating, pitch, tier selector (4 pills, Standard POPULAR, interactive JS)
- [x] C4 — Tier includes panel + qty stepper + add-to-cart + urgency + 4 trust badges
- [x] C5 — Tabs (Description / Comparison table / Media outlets / FAQ / Reviews) — interactive JS
- [x] C6 — Related countries (4 cards) + footer

### D. QA & polish — ✅ DONE
- [x] D1 — Mockup banner at top of `index.html`
- [x] D2 — Nav updated on all 3 pages to include Home / Shop / Sample Product
- [x] D3 — Real images wired:
  - 11 country cards → Unsplash city photos (Madrid, Lisbon, Berlin, Rome, Paris, London, Mexico City, Bogotá, Rio, Buenos Aires, Santiago) layered over dark gradient + flag-color fallback
  - Hero (`.hero`) → newspaper-press photo behind dark overlay
  - Shop page hero (`.page-hero`) → newsroom photo
  - Testimonial avatar → real portrait (pravatar)
  - Product gallery main → Madrid skyline with caption overlay
  - Product thumbnails → 4 press/newsroom photos
  - 3 review avatars → real portraits
- [x] D4 — WORKPLAN.md updated

### E. Premium animated components (added later) — ✅ DONE
- [x] E1 — Coverflow hero: 11 country slides in 3D rotation, auto-advance every 4s, click center → product page, hover pauses
- [x] E2 — Orbital country network: túatú PR center + 11 country nodes rotating around 480px ring, hover pauses + highlights labels
- [x] E3 — Scrolling testimonials: 3 columns (3/2/1 visible at mobile breakpoints), each pair duplicated for seamless infinite scroll, top/bottom mask fade
- [x] E4 — Animated SVG shadow overlay: turbulence + displacement + hue-rotate behind CTA banner (gold blob morphs continuously)

### Final deliverable layout
```
mockup/
├── index.html       Home (with mockup banner)
├── shop.html        Country shop archive (11 cards, filters, sort, pagination)
├── product.html     Spain product (4 tiers, interactive selector, 5 tabs, reviews)
├── assets/styles.css
└── WORKPLAN.md
```

### To preview
Open `mockup/index.html` in a browser (double-click). Internet required for Google Fonts + Unsplash images + pravatar — they all load via HTTPS, no installs.

---

## 2. Resume protocol
If terminated, the next agent should:
1. Read this file top-to-bottom.
2. `ls mockup/` to see which files exist.
3. Pick up at the first `[ ]` item in section 1.
4. Tick items off in this file as completed.

All content/copy needed is in **section 0 (Content vault)** — no need to re-fetch tuatupr.com.
