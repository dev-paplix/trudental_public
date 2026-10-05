# TruDental Keyword Research & Implementation Cross-Check Report

**Source Research Document:** [Notion Keyword Stats (May 2025 – Apr 2026)](https://app.notion.com/p/61ce9194a45e44c1a2b6b1959f9ca660?v=9659aa0c60ae4f0cbc033166aea227d6)  
**Target Codebase:** [trudental_landing](file:///e:/codes/trudental_landing)  
**Audit Scope:** 501 Keywords cross-referenced against all application pages, components, meta tags, and content files.

---

## 1. Executive Summary

| Audit Item | Status | Findings |
| :--- | :---: | :--- |
| **Total Keywords Analyzed** | **501** | High-volume head terms, procedural queries, local Istanbul terms, and competitor brands. |
| **Exact Keyword Matches in Codebase** | **1 / 501 (0.2%)** | Only `"Trudental Tourism"` (which currently has 0 recorded monthly search volume). |
| **Target Keyword Implementation** | **0 / 500** | **Not implemented.** Zero keywords from the 500 active search queries are intentionally targeted via titles, meta descriptions, headings, or focused SEO landing pages. |
| **Dynamic Document Head & Titles** | **None** | All routes share one static title hardcoded in [index.html](file:///e:/codes/trudental_landing/index.html#L6): `"TruDental Tourism - Premium Dental Care in Istanbul"`. |
| **Meta Descriptions** | **Missing** | Zero meta description tags exist across the entire application. |
| **Structured Data (Schema.org)** | **Missing** | No JSON-LD schema markup (`MedicalClinic`, `Dentist`, `FAQPage`, etc.). |
| **Crawl Assets (Sitemap & Robots)** | **Missing** | Neither `sitemap.xml` nor `robots.txt` exists. |
| **Blog System Status** | **Mockup Cards** | Blog cards link to `#hash` anchors; no rankable article pages or long-form copy exist. |

> **Conclusion:** The keyword research is **not yet implemented** in the website. While medical terms (such as *"implants"*, *"veneers"*, and *"Istanbul"*) appear organically in general interface copy, the site currently lacks the technical SEO foundation, on-page keyword targeting, and procedural content depth needed to rank for these high-value search terms.

---

## 2. Keyword Dataset Analysis

### Search Volume Distribution
Across the 501 keywords extracted from the Notion database:

| Search Volume Tier | Keyword Count | Percentage | Representative Examples |
| :--- | :---: | :---: | :--- |
| **$\ge$ 1,000 / month** | 6 | 1.2% | `dent turkey` (2,900), `turkey dental implants cost` (1,900), `dental implants in turkey price` (1,900), `turkey best dentist` (1,000) |
| **500 – 999 / month** | 4 | 0.8% | `best dentist clinic in turkey` (720), `turkey istanbul dentist` (590), `dentist in turkey marmaris` (590) |
| **100 – 499 / month** | 31 | 6.2% | `dental care istanbul` (480), `dental cost in turkey` (480), `same day dental implants turkey` (260), `composite veneer turkey` (210), `turkey teeth finance` (170) |
| **10 – 99 / month** | 455 | 90.8% | Procedural variations, local queries, long-tail questions, and clinic comparisons. |
| **0 / month** | 5 | 1.0% | Branded variations including `Trudental Tourism`. |

---

## 3. Thematic Cluster Cross-Check

### A. High-Volume Generic & Cost Queries (Top Traffic Opportunity)
These queries represent the primary commercial intent for UK/international patients looking for dental work in Turkey:

| Keyword | Monthly Volume | Competition | Implemented? | Codebase Status |
| :--- | :---: | :---: | :---: | :--- |
| `dent turkey` | 2,900 | High | ❌ No | Appears only as separated words ("dent", "turkey") in general text. |
| `turkey dental implants cost` | 1,900 | Medium | ❌ No | Present conceptually on [pricing.tsx](file:///e:/codes/trudental_landing/src/pages/pricing/pricing.tsx), but absent from page titles, H1/H2 tags, and meta copy. |
| `dental implants in turkey price` | 1,900 | Medium | ❌ No | Not explicitly targeted. |
| `price of dental implants turkey` | 1,900 | Medium | ❌ No | Not explicitly targeted. |
| `turkey best dentist` | 1,000 | High | ❌ No | No targeting. |
| `best dentist clinic in turkey` | 720 | Medium | ❌ No | No targeting. |
| `dental cost in turkey` | 480 | High | ❌ No | Not targeted in headings or metadata. |
| `turkey teeth finance` | 170 | High | ❌ No | No financing / payment plan content exists on the site. |
| `turkey teeth on finance` | 110 | High | ❌ No | No financing content. |

---

### B. Istanbul-Specific Queries (71 Keywords — Direct Geographic Relevance)
Because TruDental is based in Istanbul, these keywords offer the highest conversion rates and lowest regional friction:

| Keyword | Monthly Volume | Competition | Implemented? | Codebase Status |
| :--- | :---: | :---: | :---: | :--- |
| `turkey istanbul dentist` | 590 | High | ❌ No | Mentioned in FAQs and Dr. Sinan's bio, but not formatted as an SEO target. |
| `dental care istanbul` | 480 | High | ⚠️ Partial | Present only in the static default `<title>` in [index.html](file:///e:/codes/trudental_landing/index.html#L6); not structured in on-page headings. |
| `implants istanbul` | 90 | High | ❌ No | Not targeted. |
| `all on 4 dental implants istanbul turkey` | 30 | Medium | ❌ No | Not targeted. |
| `best dental implants in istanbul turkey` | 30 | High | ❌ No | Not targeted. |
| `dentist in istanbul turkey` | 20 | High | ❌ No | Not targeted. |
| `cosmetic dentistry istanbul turkey` | 20 | Medium | ❌ No | Not targeted. |
| `dental spa istanbul` | 20 | High | ❌ No | Not targeted. |
| `teeth cleaning istanbul` | 10 | High | ❌ No | Not targeted. |

---

### C. Procedure-Specific Keywords

#### 1. Dental Implants & All-on-4 / All-on-6 (49 Keywords)
- **Top Keywords:**
  - `same day dental implants turkey` (260/mo, Low Competition)
  - `all on 6 dental implants cost in turkey` (30/mo, High Competition)
  - `all on 4 dental implants turkey cost` (30/mo, High Competition)
  - `full dental implants turkey cost` (30/mo, High Competition)
- **Codebase Findings:**
  - The [treatments.tsx](file:///e:/codes/trudental_landing/src/pages/treatment/treatments.tsx) page is exclusively focused on single titanium implants (specifically Shinhung implants).
  - There are **no dedicated landing pages or sections** for *All-on-4*, *All-on-6*, or *Same-Day Implants*.
  - While "All-on-4" appears 8 times across pricing tables and blog teasers, it has zero dedicated content pages to capture organic search traffic.

#### 2. Veneers & Smile Makeovers (35 Keywords)
- **Top Keywords:**
  - `composite veneer turkey` (210/mo, High Competition)
  - `e max veneers turkey` (70/mo, High Competition)
  - `smile makeover turkey cost` (50/mo, Medium Competition)
  - `turkey veneers before and after` (50/mo, Low Competition)
  - `lumineers teeth turkey` (20/mo, Medium Competition)
  - `natural veneers turkey` (20/mo, High Competition)
- **Codebase Findings:**
  - **There is no Veneers page on the website.**
  - An orphaned component, [specializedTreatments.tsx](file:///e:/codes/trudental_landing/src/pages/treatment/components/specializedTreatments.tsx#L94-L122), contains Veneer and Smile Makeover copy, but is **not imported or rendered** anywhere in the application.

#### 3. Teeth Whitening & Cleaning (30 Keywords)
- **Top Keywords:**
  - `teeth whitening prices in turkey` (90/mo, High Competition)
  - `turkey teeth whitening cost` (90/mo, High Competition)
  - `teeth cleaning istanbul` (10/mo, High Competition)
- **Codebase Findings:**
  - Appears solely as single rows in the price table ([priceList.tsx](file:///e:/codes/trudental_landing/src/pages/pricing/components/priceList.tsx)) and cost calculator. No standalone landing page or informational guide exists.

---

### D. Competitor Clinic Queries (41 Keywords)
- **Top Competitor Brands:**
  - `magicsmile turkey` (1,300/mo)
  - `smilepod turkey` (320/mo)
  - `dentakay dental clinic antalya` (320/mo)
  - `precious dent turkey` (320/mo)
  - `new look smile antalya` (260/mo)
  - `dental wise turkey` (210/mo)
  - `attelia turkey` (40/mo)
  - `sevil smile turkey` (10/mo)
- **Codebase Findings:**
  - None are present in the codebase.
  - *Strategic Value:* These keywords can be targeted using comparison or informational articles (e.g., *"Choosing a Dental Clinic in Istanbul: What to Look For Beyond the Big Brands"*).

---

### E. Other City Locations (118 Keywords)
- 118 keywords target locations outside Istanbul (Antalya: 82, Marmaris: 14, Izmir: 10, Bodrum: 8, Fethiye: 4).
- **Codebase Findings:**
  - TruDental is based in Istanbul. These keywords are not directly applicable to TruDental's core service pages, though they can be referenced in comparative travel guides (e.g., *"Dental Tourism: Why Istanbul Offers Superior Clinical Facilities Compared to Resort Cities"*).

---

## 4. Technical SEO Architecture Audit

The technical foundation of [trudental_landing](file:///e:/codes/trudental_landing) currently lacks fundamental SEO mechanisms:

### 1. Document Head & Metadata
- **Index HTML:** [index.html](file:///e:/codes/trudental_landing/index.html#L6) contains only:
  ```html
  <title>TruDental Tourism - Premium Dental Care in Istanbul</title>
  ```
- **Meta Description:** **None.** (Zero `<meta name="description">` tags found).
- **Meta Keywords:** None.
- **OpenGraph & Twitter Cards:** None. Links shared on messaging apps or social networks will fail to render rich previews.
- **Canonical Tags:** None.

### 2. Client-Side Routing Limitations
- The site routing is managed via React state in [index.tsx](file:///e:/codes/trudental_landing/index.tsx#L14-L66).
- When users navigate to `/about`, `/treatments`, `/pricing`, `/how-it-works`, `/testimonials`, `/hospitality`, or `/blog`:
  - `document.title` is **never updated**.
  - Search engine crawlers inspecting the HTML see identical `<head>` data across all URLs.

### 3. Missing Crawl Configuration Files
- No `public/sitemap.xml` exists.
- No `public/robots.txt` exists.

### 4. Blog Infrastructure Status
- In [blogRowOne.tsx](file:///e:/codes/trudental_landing/src/pages/blogs/components/blogRowOne.tsx#L14-L39) and [blogRowTwo.tsx](file:///e:/codes/trudental_landing/src/pages/blogs/components/blogRowTwo.tsx#L15-L46):
  - Articles exist only as preview cards pointing to anchor hashes (e.g., `href="#all-on-4-explained"`).
  - No article reader, markdown parser, or dedicated blog route exists to hold indexable body copy.

---

## 5. Strategic Implementation Roadmap

When you are ready to begin implementation, execute in the following 4 phases:

```
Phase 1: Technical SEO Foundation
  ├── Dynamic page titles & meta descriptions per route
  ├── Canonical tags & Open Graph metadata
  ├── Schema.org JSON-LD (MedicalClinic, Dentist, FAQPage)
  └── sitemap.xml & robots.txt generation

Phase 2: High-Volume Core On-Page Optimization
  ├── Pricing Page: Target "turkey dental implants cost" & "dental implants in turkey price"
  ├── Homepage & Treatment Hero: Target "dental care istanbul" & "turkey istanbul dentist"
  └── Introduce Finance/Payment section targeting "turkey teeth finance"

Phase 3: Procedural Landing Pages & Route Expansion
  ├── /treatments/all-on-4 (Target "all on 4 dental implants turkey cost", "same day dental implants")
  ├── /treatments/veneers (Target "composite veneer turkey", "e max veneers turkey", "smile makeover turkey cost")
  └── Activate and integrate orphaned component: specializedTreatments.tsx

Phase 4: Content & Blog SEO Architecture
  ├── Implement real article routes for existing blog teasers
  └── Publish targeted guides answering informational search queries
```

---

## 6. Priority Target Keyword Matrix for Next Phase

| Priority | Target Keyword | Search Vol / mo | Recommended Target Page | Action Required |
| :---: | :--- | :---: | :--- | :--- |
| **P1** | `turkey dental implants cost` | 1,900 | `/pricing` | Add to `<title>`, H1, FAQ schema, and calculator intro. |
| **P1** | `dental implants in turkey price` | 1,900 | `/pricing` | Add to body copy, meta description, and comparison tables. |
| **P1** | `dental care istanbul` | 480 | `/` (Home) | Reinforce in homepage H1, hero copy, and metadata. |
| **P1** | `turkey istanbul dentist` | 590 | `/about` | Integrate into Dr. Sinan's credentials & clinic overview. |
| **P2** | `same day dental implants turkey` | 260 | `/treatments/implants` | Add dedicated section with treatment timeline and recovery details. |
| **P2** | `composite veneer turkey` | 210 | `/treatments/veneers` | Create dedicated Veneers landing page (using `specializedTreatments.tsx`). |
| **P2** | `turkey teeth finance` | 170 | `/pricing` | Add clear financing & payment schedule information. |
| **P3** | `all on 4 dental implants turkey cost` | 30 | `/treatments/all-on-4` | Create dedicated All-on-4 package & cost breakdown page. |
| **P3** | `e max veneers turkey` | 70 | `/treatments/veneers` | Detail material differences (E-max vs Zirconia vs Composite). |
| **P3** | `smile makeover turkey cost` | 50 | `/treatments/cosmetic` | Highlight before/after transformations and package pricing. |
