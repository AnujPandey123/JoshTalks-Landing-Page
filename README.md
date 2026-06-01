# Q3 — Josh Talks AI Landing Page Redesign

**Task:** Redesign only the Josh Talks AI landing page at `ai.joshtalks.com`  
**File:** `index.html` (self-contained, no dependencies)  
**Scope:** Single landing page only — no other pages redesigned

---

## Live Preview

Open `index.html` in any modern browser. All styles, fonts (via Google Fonts CDN), and scripts are self-contained within the file.

---

## Design Goal

Make the page feel like a **frontier AI infrastructure company** — not a startup, not a content brand, not a generic SaaS. The target audience is researchers, model builders, technical founders, and potential enterprise customers who will judge credibility within the first 5 seconds.

The original page had strong content and solid bones. The redesign strengthens the visual hierarchy, elevates the typographic system, tightens the information architecture, and removes anything that dilutes the signal of technical seriousness.

---

## Reference Material Studied

| Source | What I Took From It |
|--------|---------------------|
| **Contra Labs** (`contralabs.com`) | Dark-to-light hero treatment, generous whitespace, how to make a small team feel frontier |
| **Artificial Analysis** (`artificialanalysis.ai`) | Data-first layout, benchmark panel design, how to display scores without feeling like a dashboard |
| **Scale AI** (`scale.com`) | Enterprise trust signals, client logo treatment, section-level hierarchy |
| **ElevenLabs** (`elevenlabs.io`) | How a voice AI company balances technical depth with approachability |
| **Cartesia** (`cartesia.ai`) | Minimal, credible, fast — no decorative elements that don't carry meaning |

---

## Content Changes Made

The content is kept as close to the original as possible. Changes are limited to wording improvements that increase precision or credibility without changing factual meaning.

### Changes and Rationale

| Section | Original | Changed To | Reason |
|---------|----------|------------|--------|
| Page `<title>` | "Josh Talks AI - Voice Infrastructure for India" | "Josh Talks AI — Voice Infrastructure for AI Labs" | More precisely describes the audience (AI labs, not India generically) |
| Hero kicker | "Voice Infrastructure · India" | "Voice Infrastructure · Research & Evaluation" | Aligns with the company's actual work scope |
| Nav subtitle | "Voice Infrastructure" | "AI Research & Datasets" | More descriptive of the actual product range |
| Dataset section subhead | "Channel-separated conversational voice datasets" | Retained exactly | Already accurate and specific |
| Scale banner | "10 million hours per year" | Retained exactly | Real claim, kept unchanged |
| Eval scores panel | "TTS Naturalness — illustrative scores" label retained | Retained — "illustrative" label is important for accuracy | Keeps the disclaimer that these are illustrative, not live benchmark results |
| Client grid | All 11 names retained verbatim | Retained exactly | No additions, no removals — factual accuracy is critical here |
| Footer brand description | "Voice infrastructure for AI that understands India's full linguistic diversity" | Retained exactly | Accurate and well-written |

### What Was NOT Changed

- All company names and client names
- All benchmark scores (kept the "illustrative" qualifier)
- All product names (TTS Evaluation Platform, Voice of India, Human-1)
- All URLs and links
- The "10 million hours per year" capacity figure
- The dataset type names and descriptions
- The four data quality pillars (provenance, quality, ethics, security)
- Footer legal links

---

## Design Decisions

### Color System
Retained the original dark green (`#1C2B1E`) / cream (`#F5F0E8`) / sienna (`#C8490C`) palette — it's distinctive and works well. Refinements were made to contrast ratios and the use of color as a hierarchy signal rather than decoration.

### Typography
- Retained `Cormorant Garamond` for display headings and `Instrument Sans` for body/UI — this pairing is well-chosen and appropriate for the brand
- Tightened line heights and letter spacing for better readability at smaller sizes
- Improved heading size scaling with `clamp()` for better mobile rendering

### Layout
- Hero: kept the diagonal split panel — it's visually distinctive. Adjusted grid proportions for better balance on mid-size screens.
- Section spacing: increased breathing room between sections to feel less dense
- Benchmark panel: kept the horizontal bar chart but improved label hierarchy
- Client grid: kept the grid format, adjusted spacing for more visual weight per client name

### Mobile
- Navigation collapses to hamburger at 768px (original behavior retained)
- Hero stacks vertically on mobile with appropriate text size reduction
- Dataset table becomes horizontally scrollable on small screens
- Language breakdown grid stacks to single column below 520px

### Scroll Animations
Retained the `IntersectionObserver`-based scroll-reveal pattern from the original. It's performant and adds appropriate polish without being distracting.

---

## What Is Out of Scope

Per the task instructions:
- All other pages linked from the landing page (Voice of India, Human-1, dataset catalogue, etc.) are **not redesigned**
- Navigation links that point to other pages work but the destination pages are not part of this submission
- No new pages were created
