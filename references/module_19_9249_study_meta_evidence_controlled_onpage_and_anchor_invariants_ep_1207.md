# Module 19: 9,249-Study Meta-Evidence, Controlled On-Page & Anchor Invariants

*Source: The SEO Meta Study (Krešimir Ćorluka, CEO & co-founder @ Ovisy; September 2026; Zenodo DOI: 10.5281/zenodo.22768160) & The Edward Show Ep. 1191 (Audio release) / Ep. 1207 (YouTube interview: "He Dug Through 9,249 SEO Case Studies. Here's What Actually Works" — Edward Sturm).*

> **Scope Partition:** Scaled content collapse protocols live in **Module 17**. Quality Rater page audits live in **Module 18**. Single-variable isolation and confounder controls live in [`kirby-seo-telemetry`](../../kirby-seo-telemetry/SKILL.md) Module 9 §9.3. This module establishes the **empirical evidence hierarchy, controlled title tag rules, internal linking standards, and footer architecture guidelines** extracted from the 9,249-document systematic review.

---

### **19.1 The 9,249-Study Evidence Calibration & Publication Bias**

The SEO industry suffers from massive survivorship bias. Any strategic plan or agentic workflow must calibrate expectations against empirical corpus realities:

```
┌─────────────────────────────────────────────────────────────────────────┐
│               THE 9,249 SEO META-STUDY REALITY CHECK                   │
├────────────────────────────────────┬────────────────────────────────────┤
│ Corpus Reality Metric              │ Operational Constraint             │
├────────────────────────────────────┼────────────────────────────────────┤
│ 81.9% Positive / 3.8% Negative     │ Never assume case-study results    │
│ published outcome skew             │ are normal; agencies hide failures │
├────────────────────────────────────┼────────────────────────────────────┤
│ 602 of 769 tactics have ZERO       │ Disregard uncalibrated "graph      │
│ controlled split tests             │ moved" posts; prioritize A/B tests │
├────────────────────────────────────┼────────────────────────────────────┤
│ 65 of 118 credited controlled      │ Weight SearchPilot controlled data │
│ measurements belong to SearchPilot │ above all vendor opinion pieces    │
├────────────────────────────────────┼────────────────────────────────────┤
│ 50.5% (92/182) of entries          │ Never attribute traffic to a single│
│ changed multiple variables at once │ bundled redesign or migration      │
└────────────────────────────────────┴────────────────────────────────────┘
```

**Planning Rule:** Never budget for the published median gains on client websites without isolating single variables. Across the meta-study corpus, the **median controlled A/B test gain is +16%**, whereas the **median uncontrolled before/after claim is +106%** for the exact same tactics.

---

### **19.2 Controlled Title Tag Engineering (SearchPilot Invariants)**

Title tags remain the highest-leverage on-page lever for immediate click-through rate (CTR) and ranking adjustments. Apply the three controlled findings:

1. **The `Updated Daily` Recency Signal**:
   - **Flawed Pattern**: Appending static calendar years (e.g., `Best CRM Software for 2026`), which simply adds a modest ~+5% baseline lift but decays quickly into SERP visual monotony.
   - **Controlled Pattern**: Replacing month/year stamps with **`Updated Daily`** generated a **+11% organic sessions lift** (SearchPilot controlled listings test). The underlying mechanism is literal factual freshness; hardcoding a deceptive "updated" stamp on stale content invites algorithmic deprecation.
2. **ALL CAPS Noun Phrase Disruption**:
   - Writing primary entity nouns or titles entirely in CAPITAL LETTERS yielded an average **+17.5% organic traffic lift** across two independent SearchPilot tests due to visual contrast in SERPs.
   - **Implementation**: Do not shout the entire tag; capitalize the core high-intent entity hook:
     `ALL-IN-ONE CRM: Complete Workflow Blueprint [Updated Daily] | Brand`
3. **Dynamic vs. Static Pricing Tags**:
   - **Static Price**: Inserting hardcoded prices (e.g., `$49/mo`) caused a **-7% organic traffic drop** on rental location pages (and a separate e-commerce price-in-title test recorded a **-15% decline**) due to searchers pre-filtering themselves out before consuming the landing page value proposition.
   - **Dynamic Price**: Programmatic price feeds reflecting live inventory produced a **+10% organic traffic gain** on the identical site in back-to-back testing. If pricing fluctuates or requires qualifying variables, omit it from the title tag entirely.

---

### **19.3 Internal Linking: Orphan Recovery (Measured) vs Anchor Invariant (Operational)**

Evidence and agency convention must be strictly partitioned:

1. **Measured Finding (Orphan-Page Recovery)**: Controlled experiments in the meta-study isolate internal link additions to orphaned or deeply nested pages as a verified positive ranking driver. Inlinking orphan pages is an empirical, tier-1 priority.
2. **Operational Convention (Anchor Text Consistency)**: The meta-study contains *no controlled split tests* isolating exact-match anchors against synonym variations. Standard agency practice favors descriptive keyword consistency over random synonym dispersion for core hub pages, but this is an unverified operational convention, not a measured controlled finding. Treat anchor variation as an off-page penalty avoidance tactic rather than a proven on-page optimization lever.

---

### **19.4 Footer Category Links: Gain Mechanism & Risk Governance**

Footer links function as structural crawl paths, but carry operational trade-offs:

1. **Controlled Organic Lift**: In one controlled test, adding homepage footer links pointing directly to category and subcategory pages **increased organic sessions by 5–10%**, functioning as an effective crawl and indexation bridge for deep category levels.
2. **PPC & Semantic Governance**: Despite the structural crawl benefit, caution is required in regulated or sensitive niches (e.g., healthcare, finance). Injecting high-volume commercial keyword anchors into sitewide footers can trigger automated Google Ads policy warnings or create unnatural sitewide anchor distributions.
3. **Architecture Guidance**: Use footer links intentionally to rescue deep categories from orphan status, but maintain primary topical routing through header navigation, breadcrumbs, and contextual body copy.

---

### **19.5 AEO / GEO Empirical Grounding**

Generative Engine Optimization (AEO/GEO) is heavily distorted by speculative claims:

- **The `LLMs.txt` Reality**: No controlled test of `llms.txt` exists anywhere in the 9,249-document corpus. It remains unproven and should never displace foundational semantic HTML.
- **The Verified Citation Drivers**: What actually drives AI Overviews, ChatGPT Search, and Perplexity retrieval are standard high-effort SEO structures:
  1. **Direct Declarative Answers in Opening Hook**: Placing direct answers in the opening paragraph drives a **+280% citation increase**.
  2. **Original Statistics**: Publishing first-party quantitative data drives a **+37% citation increase**.
  3. **Structured HTML Tables**: Pre-computed comparison matrices that are retrievable as a single coherent chunk.
  4. **Named Expert Attribution**: Quoting recognized domain authorities drives a **+22% to +41% citation lift**.
