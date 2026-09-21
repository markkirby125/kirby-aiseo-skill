# AI SEO Standard Operating Procedure (SOP) - Dispatcher

This skill acts as a dispatcher for the AI SEO protocol. The full 4000-line SOP has been modularized and optimized to minimize context load. 
When asked to perform AI SEO tasks, **do not guess**. Instead, review the module index below and read the specific module file(s) relevant to the task using your file-reading tools.

## 📚 Module Index

**Executive & Core Strategy**
- **Executive Threat Profile**: Scaled Content Abuse & Demotion Signals -> Read `./00_executive_summary.md`
- **Module 1**: Technical Infrastructure & Crawler Accessibility (Cloudflare, robots.txt, edge delivery, URL slug resets, Crawled vs Discovered router) -> Read `./module_1_technical_infrastructure_crawler_accessibility.md`

**Content & On-Page Engineering**
- **Module 2**: On-Page Semantic Architecture & Content Engineering (GEO retrieval multipliers, content structures, RAG chunking, SEO Rater Guidelines, SERP undertargeting, 4-question framework, 1-Hour SEO Update, short landing pages) -> Read `./module_2_on_page_semantic_architecture_content_engineering.md`

**Other Modules**
- **Module 6**: Google Discover & Algorithmic Feed Optimization (including Discover Natural Language Feed Customization) -> Read `./module_6_google_discover_algorithmic_feed_optimization.md`
- **Module 8**: Vulnerable Footprints vs. Resilient Asset Architecture (Quick Reference) -> Read `./module_8_quick_reference_vulnerable_footprints_vs_resilient_asset_architecture.md`
- **Module 9**: Site-Specific Implementation Checklists -> Read `./module_9_site_specific_implementation_checklists.md`
- **Module 10**: Gap-Analysis Supplementary Protocols (Remaining September 2026 Research Updates) -> Read `./module_10_gap_analysis_supplementary_protocols_september_2026_research_update.md`

## When to Use
- You need to optimize content for AI search engines (ChatGPT, Perplexity, Gemini).
- You are auditing a site for "Scaled Content Abuse", "Mount AI" demotions, or general SEO drops.
- You are conducting keyword research, auditing SERP undertargeting across the 4 anchor spots, prioritizing keywords with the 4-question framework, or diagnosing content type nuances (Module 2 §2.29). Telemetry extraction filter is `kirby-seo-telemetry` §5.15.
- You are executing the 1-Hour SEO Update to elevate GSC queries in positions 5–20 and 20–50 into `<title>`, `<h1>`, and opening hooks (Module 2 §2.19).
- You are architecting high-converting short SEO landing pages (200–600 words) instead of bloated 3,000-word blog posts (Module 2 §2.35).
- You are diagnosing which GSC queries a URL ranks for without mentioning them, deciding between lexical write-back and new content, or judging whether a page sits on the exact-match, phrase-match, or broad-match rung (Module 2 §2.36). Do not confuse this with LLM fan-out harvesting (§2.16 / §2.28).
- You are deciding whether a query becomes a dedicated URL or an on-page `<h2>` (Module 2 §2.37 SERP-overlap test). Apply the order: §2.37 overlap → §2.29F authority capability → `kirby-local-seo` §3.9B/§3.9E volume and competition gating.
- You are harvesting `site:` operator results to discover pre-indexed topical authority and internal-link donors, deploying section `#anchor` bridges, enforcing natural anchor variation and funnel-tier link budgets, or staging hub-page keywords (Module 10 §10.11).
- For 1st-party Direct Trust Overrides in AI Overviews, Google AI Mode, and Preferred Sources SDK: route to `kirby-preferred-sources`.
- You are troubleshooting crawl-depth failures or category/hub `noindex` traps (Module 1 §1.15). Social/video indexation plays belong in `kirby-off-page-seo` Module 15.
- You are diagnosing `Crawled - currently not indexed` vs `Discovered - currently not indexed`, or an indexed-then-pulled location/template URL (Module 1 §1.16). GSC coverage measurement and template fail-rate slope: `kirby-seo-telemetry` Module 8. Location-page rewrite order: `kirby-local-seo` §3.6.2.
- You are executing a 30-day content pruning sprint to consolidate entity authority (Module 2 §2.34). Off-page Wikidata/social corroboration is `kirby-off-page-seo` Module 16.
- First-party “Best X” / comparison pages: Module 2 §2.16. Third-party listicle *insertions* and competitive link-gap outreach: `kirby-off-page-seo` Module 18 (do not invent outreach here).
- GBP, Ask Maps, and review velocity: use `kirby-local-seo`. Do not handle them in this skill.
- Editorial essay / thought-leadership architecture: use `kirby-great-essay`.
- GitHub / Docker Hub / Dev.to entity graphs: use `kirby-technical-aeo`.
- The user mentions AI SEO, AEO, GEO, or asks to apply the SOP.

## How It Works
1. Identify the specific domain or optimization requested by the user.
2. Read the corresponding module(s) from the `./` directory.
3. Apply the rules exactly as written in the module. Do not rationalize or ignore the rules.

## ✅ Pre-Deploy Checklist
- Always explicitly mention which Module you are reading and applying.
- Validate that your output adheres strictly to the constraints in the chosen Module.
