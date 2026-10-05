# TruDental Keyword Research & Implementation Cross-Check Report

**Source Research Document:** [Notion Keyword Stats (May 2025 – Apr 2026)](https://app.notion.com/p/61ce9194a45e44c1a2b6b1959f9ca660?v=9659aa0c60ae4f0cbc033166aea227d6)  
**Target Codebase:** [trudental_landing](file:///e:/codes/trudental_landing)  
**Audit Scope:** 501 Keywords cross-referenced against all application pages, visible text copy, headings, and component files.

---

## 1. Executive Summary: Content-Only Cross-Check

Looking strictly at the **visible page contents** (body copy, headings, FAQ accordions, pricing tables, and UI text), here is the exact breakdown:

| Metric | Count | Percentage | What It Means |
| :--- | :---: | :---: | :--- |
| **Strict Exact Phrase Matches in Content** | **1 / 501** | **0.2%** | Only `"Trudental Tourism"` (which currently has 0 recorded monthly search volume). |
| **Normalized Matches (ignoring punctuation/hyphens)** | **2 / 501** | **0.4%** | `"implants istanbul"` (90/mo) inside a blog anchor slug and `"Trudental Tourism"`. |
| **Token / Fragmented Word Matches** | **156 / 501** | **31.1%** | All words of the keyword appear somewhere on the same page, but **scattered across different sentences or table rows**, never structured as an intentional target phrase. |
| **Completely Absent from Content** | **343 / 501** | **68.5%** | One or more core words from the query **never appear anywhere** in the website content. |

> **Direct Answer:** Only **1 keyword (0.2%)** appears as an exact match in the content. While **156 keywords (31.1%)** have their constituent words loosely scattered across pages, **343 keywords (68.5%)** are completely missing from the website text.

---

## 2. Keyword Dataset Analysis & Volume Tiers

Across the 501 keywords extracted from the Notion database:

| Search Volume Tier | Keyword Count | Percentage | Representative Examples |
| :--- | :---: | :---: | :--- |
| **$\ge$ 1,000 / month** | 6 | 1.2% | `dent turkey` (2,900), `turkey dental implants cost` (1,900), `dental implants in turkey price` (1,900), `turkey best dentist` (1,000) |
| **500 – 999 / month** | 4 | 0.8% | `best dentist clinic in turkey` (720), `turkey istanbul dentist` (590), `dentist in turkey marmaris` (590) |
| **100 – 499 / month** | 31 | 6.2% | `dental care istanbul` (480), `dental cost in turkey` (480), `same day dental implants turkey` (260), `composite veneer turkey` (210), `turkey teeth finance` (170) |
| **10 – 99 / month** | 455 | 90.8% | Procedural variations, local queries, long-tail questions, and clinic comparisons. |
| **0 / month** | 5 | 1.0% | Branded variations including `Trudental Tourism`. |

---

## 3. Content Match Breakdown: Where Do Keywords Stand?

### A. The 156 Fragmented / Scattered Matches (31.1%)
For these 156 keywords, the individual words are present on the website, but they are split across separate sentences, table cells, or FAQ items rather than placed together in high-value positions (like H1/H2 headings or focused lead paragraphs).

#### High-Volume Examples of Fragmented Content:
| Keyword | Monthly Volume | Competition | Where Words Appear in Code | Why It Doesn't Rank Currently |
| :--- | :---: | :---: | :--- | :--- |
| `turkey dental implants cost` | 1,900 | Medium | [costCalculator.tsx](file:///e:/codes/trudental_landing/src/pages/pricing/components/costCalculator.tsx), [pricingFaq.tsx](file:///e:/codes/trudental_landing/src/pages/pricing/components/pricingFaq.tsx), [comparesLanding.tsx](file:///e:/codes/trudental_landing/src/pages/landing/components/comparesLanding.tsx) | "Turkey", "dental", "implants", and "cost" exist on the pricing page, but in disconnected sentences. Never combined as a primary heading or target phrase. |
| `dental implants in turkey price` | 1,900 | Medium | [pricingFaq.tsx](file:///e:/codes/trudental_landing/src/pages/pricing/components/pricingFaq.tsx), [howWorksFQ.tsx](file:///e:/codes/trudental_landing/src/pages/how_works/components/howWorksFQ.tsx) | Same as above — scattered across comparison tables and FAQ answers. |
| `price of dental implants turkey` | 1,900 | Medium | [pricingFaq.tsx](file:///e:/codes/trudental_landing/src/pages/pricing/components/pricingFaq.tsx), [costCalculator.tsx](file:///e:/codes/trudental_landing/src/pages/pricing/components/costCalculator.tsx) | Same as above. |
| `turkey best dentist` | 1,000 | High | [howWorksFQ.tsx](file:///e:/codes/trudental_landing/src/pages/how_works/components/howWorksFQ.tsx), [treatmentFaQ.tsx](file:///e:/codes/trudental_landing/src/pages/treatment/components/treatmentFaQ.tsx) | "Turkey", "best", and "dentist" appear loosely in FAQ body paragraphs. |
| `best dentist clinic in turkey` | 720 | Medium | [pricingFaq.tsx](file:///e:/codes/trudental_landing/src/pages/pricing/components/pricingFaq.tsx), [treatmentFaQ.tsx](file:///e:/codes/trudental_landing/src/pages/treatment/components/treatmentFaQ.tsx) | Disjointed across generic clinic descriptions. |
| `turkey istanbul dentist` | 590 | High | [drSinan.tsx](file:///e:/codes/trudental_landing/src/pages/about/components/drSinan.tsx), [treatmentHero.tsx](file:///e:/codes/trudental_landing/src/pages/treatment/components/treatmentHero.tsx) | Mentioned in Dr. Sinan's biography, but not structured into an SEO-focused headline. |
| `dental care istanbul` | 480 | High | [aboutHero.tsx](file:///e:/codes/trudental_landing/src/pages/about/components/aboutHero.tsx), [foundersStory.tsx](file:///e:/codes/trudental_landing/src/pages/about/components/foundersStory.tsx) | Used conversationally in the story text, but never in a main page H1. |
| `dental cost in turkey` | 480 | High | [comparesLanding.tsx](file:///e:/codes/trudental_landing/src/pages/landing/components/comparesLanding.tsx), [howWorksFQ.tsx](file:///e:/codes/trudental_landing/src/pages/how_works/components/howWorksFQ.tsx) | Separated words across cost comparison sections. |
| `same day dental implants turkey` | 260 | Low | [howFit.tsx](file:///e:/codes/trudental_landing/src/pages/treatment/components/howFit.tsx) | Mentioned briefly in technical copy; no dedicated service breakdown or timeline. |

---

### B. The 343 Completely Missing Keywords (68.5%)
These 343 keywords do not exist in the site's content at all. They fall into three clear categories:

1. **Competitor Clinic Brands (41 keywords):**
   - E.g., `magicsmile turkey` (1,300/mo), `smilepod turkey` (320/mo), `dentakay dental clinic antalya` (320/mo), `precious dent turkey` (320/mo), `new look smile antalya` (260/mo), `dental wise turkey` (210/mo), `attelia turkey` (40/mo), `sevil smile turkey` (10/mo).
   - *Status:* Completely absent. (Expected for brand names, but valuable for comparison guides).

2. **Other Turkish Cities & Resort Towns (118 keywords):**
   - Searches targeting Antalya (82), Marmaris (14), Izmir (10), Bodrum (8), Kusadasi (4), and Fethiye (4).
   - E.g., `dentist in turkey marmaris` (590/mo), `dental clinic izmir` (140/mo), `dentist kusadasi turkey` (140/mo), `smiles turkey antalya` (210/mo).
   - *Status:* Completely absent because TruDental operates exclusively in Istanbul.

3. **High-Intent Uncovered Procedures & Commercial Queries (184 keywords):**
   - **Financing:** `turkey teeth finance` (170/mo), `turkey teeth on finance` (110/mo), `finance turkey teeth` (50/mo). The site has no financing/payment plan text.
   - **Veneers & Cosmetics:** `composite veneer turkey` (210/mo), `e max veneers turkey` (70/mo), `smile makeover turkey cost` (50/mo), `lumineers teeth turkey` (20/mo), `natural veneers turkey` (20/mo). The site has no Veneers page.
   - **Whitening & Hygiene:** `teeth whitening prices in turkey` (90/mo), `turkey teeth whitening cost` (90/mo), `teeth cleaning istanbul` (10/mo). Only listed as brief table items.
   - **Informal / Patient Slang:** `fake turkey teeth` (140/mo), `teeth operation turkey`, `dental holidays in turkey` (110/mo), `having your teeth done in turkey`.

---

## 4. Content Architecture Gaps in the Codebase

1. **The Treatments Page is Exclusively About Implants:**
   - In [treatments.tsx](file:///e:/codes/trudental_landing/src/pages/treatment/treatments.tsx), all sections focus on titanium implants (specifically Shinhung).
   - There are no pages, routes, or dedicated content blocks for Veneers, Full Mouth Restoration, Crowns, Bridges, or Teeth Whitening.

2. **Orphaned Component Found:**
   - The file [specializedTreatments.tsx](file:///e:/codes/trudental_landing/src/pages/treatment/components/specializedTreatments.tsx) already contains written copy for **Veneers**, **Full Mouth Restoration**, and **Crowns & Bridges**.
   - However, it is **never imported or rendered** anywhere in the app!

3. **Blog Cards are Hollow Placeholders:**
   - In [blogRowOne.tsx](file:///e:/codes/trudental_landing/src/pages/blogs/components/blogRowOne.tsx) and [blogRowTwo.tsx](file:///e:/codes/trudental_landing/src/pages/blogs/components/blogRowTwo.tsx), articles like *"Composite vs Porcelain Veneers"* and *"All-on-4 Explained"* exist only as preview cards linking to `#hash` anchors.
   - There is no actual article reader or long-form copy to rank in search results.

---

## 5. Strategic Recommendations & Actionable Suggestions

Here are the highest-impact recommendations to bridge the gap between your keyword research and website content:

### 1. Unify Fragmented High-Volume Words into Dedicated Headings
Currently, Google sees words like *"turkey"*, *"dental"*, *"implants"*, and *"cost"* scattered randomly. Unify them into prominent H1 and H2 tags:
- **On [pricing.tsx](file:///e:/codes/trudental_landing/src/pages/pricing/pricing.tsx):**
  - Add an H1: `Dental Implants in Turkey: Full Cost & Price Guide (2026)` (immediately targets 3,800/mo search volume across `turkey dental implants cost` and `dental implants in turkey price`).
  - Add an FAQ accordion specifically titled: `What is the Average Price of Dental Implants in Turkey vs the UK?`.
- **On the Homepage / About Page:**
  - Strengthen headings to include `Top Dental Care in Istanbul, Turkey` and `Experienced English-Speaking Dentists in Istanbul`.

---

### 2. Create Dedicated Procedure Pages (Activate Existing Work)
Instead of forcing all procedures onto one generic treatment page:
- **Activate [specializedTreatments.tsx](file:///e:/codes/trudental_landing/src/pages/treatment/components/specializedTreatments.tsx):** Re-integrate this component into the treatment experience so the existing content for Veneers, Crowns, and Full Mouth Restoration is visible to users and search bots.
- **Create a Dedicated Veneers Page (`/treatments/veneers`):**
  - Target: `composite veneer turkey` (210/mo), `e max veneers turkey` (70/mo), `smile makeover turkey cost` (50/mo), `natural veneers turkey` (20/mo).
  - Include a direct comparison: *Composite Veneers vs Porcelain/E-Max Veneers: Cost, Longevity & Procedure*.
- **Create an All-on-4 / All-on-6 Page (`/treatments/all-on-4`):**
  - Target: `all on 4 dental implants turkey cost` (30/mo), `same day dental implants turkey` (260/mo), `all on 6 dental implants cost in turkey` (30/mo).
  - Outline the day-by-day surgical protocol, materials, and price packages.

---

### 3. Add a "Finance & Flexible Payment Options" Section
- Keywords: `turkey teeth finance` (170/mo), `turkey teeth on finance` (110/mo), `finance turkey teeth` (50/mo).
- **Suggestion:** Add a dedicated section or FAQ on the [pricing page](file:///e:/codes/trudental_landing/src/pages/pricing/pricing.tsx) explaining:
  - Deposit requirements
  - Stage-by-stage payments (pay per visit)
  - Accepted payment methods (UK debit/credit cards, bank transfers, cash in GBP/EUR)
  - Potential UK medical loan financing partners.

---

### 4. Leverage the 71 Istanbul-Specific Keywords as a Competitive Moat
Over 100 keywords in your list target resort towns like Antalya or Marmaris. Use this to TruDental's advantage:
- Write content explicitly highlighting **why Istanbul is the medical capital of Turkey**:
  - Higher concentration of specialized university-trained oral surgeons.
  - Year-round flight availability from all UK airports.
  - Less of a "holiday package assembly-line" feel than beach-resort clinics.
- Target keywords: `turkey istanbul dentist` (590/mo), `dental care istanbul` (480/mo), `best dental implants in istanbul turkey` (30/mo).

---

### 5. Turn the 6 Mockup Blog Cards into Real Rankable Content
You already have great article topics drafted in [blogRowOne.tsx](file:///e:/codes/trudental_landing/src/pages/blogs/components/blogRowOne.tsx) and [blogRowTwo.tsx](file:///e:/codes/trudental_landing/src/pages/blogs/components/blogRowTwo.tsx). Turn them into full articles:
1. *"The Truth About Dental Implants in Istanbul: What UK Patients Really Need to Know"* (Targets `dental care istanbul`, `implants istanbul`).
2. *"Composite vs Porcelain Veneers: Which Is Right for You?"* (Targets `composite veneer turkey`, `veneers price in turkey`).
3. *"All-on-4 Explained: What No One Tells You Before Surgery"* (Targets `all on 4 dental implants turkey cost`, `same day dental implants turkey`).
4. *"How to Plan Your Dental Holiday: A Step-by-Step Guide"* (Targets `dental holidays in turkey`).

---

## 6. Priority Action Matrix

| Priority | Strategy | Primary Target Keywords | Expected Impact |
| :---: | :--- | :--- | :--- |
| **Immediate** | **Pricing Page Heading & FAQ Restructure** | `turkey dental implants cost` (1,900)<br>`dental implants in turkey price` (1,900)<br>`dental cost in turkey` (480) | Directly targets the highest-volume commercial terms with minimal code changes. |
| **High** | **Activate Veneers & All-on-4 Content** | `composite veneer turkey` (210)<br>`same day dental implants turkey` (260)<br>`e max veneers turkey` (70) | Captures procedure-specific search intent; utilizes existing dormant components. |
| **High** | **Add Finance / Payment Options Section** | `turkey teeth finance` (170)<br>`turkey teeth on finance` (110) | Addresses a top patient purchasing barrier and captures high-conversion commercial traffic. |
| **Medium** | **Istanbul Authority & Comparison Guide** | `turkey istanbul dentist` (590)<br>`dental care istanbul` (480) | Positions TruDental as the premium Istanbul alternative to Antalya resort clinics. |
| **Medium** | **Publish Real Blog Articles** | `all on 4 dental implants turkey cost`<br>`dental holidays in turkey` | Drives top-of-funnel informational traffic from UK searchers researching options. |
