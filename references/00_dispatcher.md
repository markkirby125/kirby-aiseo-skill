# AI SEO Standard Operating Procedure (SOP) - Dispatcher

This skill acts as a dispatcher for the AI SEO protocol. The full 4000-line SOP has been modularized and optimized to minimize context load. 
When asked to perform AI SEO tasks, **do not guess**. Instead, review the module index below and read the specific module file(s) relevant to the task using your file-reading tools.

## 📚 Module Index

**Executive & Core Strategy**
- **Executive Threat Profile**: Scaled Content Abuse & Demotion Signals -> Read `./00_executive_summary.md`
- **Module 1**: Technical Infrastructure & Crawler Accessibility (Cloudflare, robots.txt, edge delivery, URL slug resets, Crawled vs Discovered router, harmonic centrality, CCBot plain-text standards, WAF/CDN AI-crawler audit, fresh-domain AI Overview quarantine, fan-out reasoning filter, search-grounding bot governance §1.22) -> Read `./module_1_technical_infrastructure_crawler_accessibility.md`

**Content & On-Page Engineering**
- **Module 2**: On-Page Semantic Architecture & Content Engineering (GEO retrieval multipliers incl. 9,249-study benchmarks, content structures, RAG chunking, SEO Rater Guidelines, SERP undertargeting, 4-question framework, 1-Hour SEO Update, short landing pages, credibility documents, dual topical maps, comparison 99%/1% rule, BM25 optimization, entity definition trinity, personal KG book-funnel, entity home invariant, KD 2–3 fan-out exception, Compact Keywords framework §2.46, deep technical product attributes §2.47, middle-of-funnel educational citation guides §2.48, Discount Transparency Block canonical specification §2.49) -> Read `./module_2_on_page_semantic_architecture_content_engineering.md`

**Other Modules**
- **Module 6**: Google Discover & Algorithmic Feed Optimization (including Discover Natural Language Feed Customization) -> Read `./module_6_google_discover_algorithmic_feed_optimization.md`
- **Module 8**: Vulnerable Footprints vs. Resilient Asset Architecture (Quick Reference) -> Read `./module_8_quick_reference_vulnerable_footprints_vs_resilient_asset_architecture.md`
- **Module 9**: Site-Specific Implementation Checklists -> Read `./module_9_site_specific_implementation_checklists.md`
- **Module 10**: Gap-Analysis Supplementary Protocols (Remaining September 2026 Research Updates) -> Read `./module_10_gap_analysis_supplementary_protocols_september_2026_research_update.md`
- **Module 14**: Defensive GEO & AI Reputation Management (ORM) (Mitigating negative AI Overviews, crisis management pre-planning, on-domain Reddit rebuttal architecture §14.4) -> Read `./module_14_defensive_geo_ai_orm_ann_smarty_ep_1186.md`
- **Module 15**: October 2026 Metadata Fact-Check Mandate & SRA Compliance Boundaries (per-surface metadata verification, Site Reputation Abuse boundary test, autonomous-agent publishing gate) -> Read `./module_15_october_2026_metadata_fact_check_sra_boundaries.md`
- **Module 16**: Post-Update Indexing Latency & Propagation Expectations (Illyes Oct 2026 benchmarks; 1-Hour SEO Update verdict windows, per-change-class propagation table) -> Read `./module_16_post_update_indexing_latency.md`
- **Module 17**: Scaled AI Content Collapse Autopsy & Quarantine Protocols (Grokipedia Case Study - Ep. 1197) -> Read `./module_17_scaled_ai_collapse_autopsy_and_quarantine_protocols.md`
- **Module 18**: The Anti-Slop Detection Boundary & Quality Raters Page Audit (Whitespark E48 & E50) -> Read `./module_18_ai_slop_detection_boundary_and_quality_raters_audit.md`
- **Module 19**: 9,249-Study Meta-Evidence, Controlled On-Page & Anchor Invariants (SearchPilot controlled title experiments, orphan inlinking measured findings, footer link gain mechanisms & PPC risk, AEO empirical grounding — Ep. 1191 audio / Ep. 1207 YouTube; Zenodo DOI: 10.5281/zenodo.22768160) -> Read `./module_19_9249_study_meta_evidence_controlled_onpage_and_anchor_invariants_ep_1207.md`

## When to Use
- You need to optimize content for AI search engines (ChatGPT, Perplexity, Gemini).
- You are developing defensive GEO strategies or mitigating negative AI Overviews (Module 14).
- You are auditing a site for "Scaled Content Abuse", "Mount AI" demotions, or general SEO drops.
- You are fact-checking AI-assisted metadata (titles, meta descriptions, JSON-LD, alt text) under the Oct 1, 2026 mandate, judging SRA compliance boundaries for third-party syndication, or gating autonomous-agent publishing (Module 15).
- You are conducting keyword research, auditing SERP undertargeting across the 4 anchor spots, prioritizing keywords with the 4-question framework, or diagnosing content type nuances (Module 2 §2.29). Telemetry extraction filter is `kirby-seo-telemetry` §5.15.
- You are executing the 1-Hour SEO Update to elevate GSC queries in positions 5–20 and 20–50 into `<title>`, `<h1>`, and opening hooks (Module 2 §2.19).
- You are architecting high-converting short SEO landing pages (200–600 words) instead of bloated 3,000-word blog posts (Module 2 §2.35).
- You are diagnosing which GSC queries a URL ranks for without mentioning them, deciding between lexical write-back and new content, or judging whether a page sits on the exact-match, phrase-match, or broad-match rung (Module 2 §2.36). Do not confuse this with LLM fan-out harvesting (§2.16 / §2.28).
- You are deciding whether a query becomes a dedicated URL or an on-page `<h2>` (Module 2 §2.37 SERP-overlap test). Apply the order: §2.37 overlap → §2.29F authority capability → `kirby-local-seo` §3.9B/§3.9E volume and competition gating.
- You are harvesting `site:` operator results to discover pre-indexed topical authority and internal-link donors, deploying section `#anchor` bridges, enforcing natural anchor variation and funnel-tier link budgets, or staging hub-page keywords (Module 10 §10.11).
- For 1st-party Direct Trust Overrides in AI Overviews, Google AI Mode, and Preferred Sources SDK: route to `kirby-preferred-sources`.
- You are troubleshooting crawl-depth failures or category/hub `noindex` traps (Module 1 §1.15). Social/video indexation plays belong in `kirby-off-page-seo` Module 15.
- You are evaluating link authority via harmonic centrality / seed-graph distance, auditing Common Crawl (CCBot) accessibility, unblocking AI crawlers at the WAF/CDN layer, or timing fresh-domain AI Overview measurement (Module 1 §1.17–§1.20).
- You are defining or standardizing an entity (KG ID, Knowledge Panel, semantic triples) with the Who/What/Why trinity (Module 2 §2.42). Tender/procurement gating applications of this doctrine live in `kirby-decision-engine-optimization` Module 3.
- You are hardening About/Privacy/Returns trust documents (Module 2 §2.38), architecting dual topical maps (§2.39), replacing listicles with 99%/1% comparison pages (§2.40), or running BM25 lexical optimization (§2.41).
- You are executing the personal Knowledge Panel book-funnel (Google Books → KG MID, Module 2 §2.43), building the entity home with the `/about-[name]` slug invariant and sameAs wrapping (§2.44), or assessing why an entity loses the 15→4–5 fan-out reasoning cut (Module 1 §1.21).
- You are evaluating the KD 2–3 fan-out long-tail exception — scoped carve-out from §2.16A, audit-confirmed only (Module 2 §2.45).
- You are auditing a lead-gen/affiliate business against the middleman-extinction thesis or assembling the three-layer digital moat (entity/utility/engagement — Module 8).
- You are diagnosing `Crawled - currently not indexed` vs `Discovered - currently not indexed`, or an indexed-then-pulled location/template URL (Module 1 §1.16). GSC coverage measurement and template fail-rate slope: `kirby-seo-telemetry` Module 8. Location-page rewrite order: `kirby-local-seo` §3.6.2.
- You are executing a 30-day content pruning sprint to consolidate entity authority (Module 2 §2.34). Off-page Wikidata/social corroboration is `kirby-off-page-seo` Module 16.
- First-party “Best X” / comparison pages: Module 2 §2.16. Third-party listicle *insertions* and competitive link-gap outreach: `kirby-off-page-seo` Module 18 (do not invent outreach here).
- GBP, Ask Maps, and review velocity: use `kirby-local-seo`. Do not handle them in this skill.
- Editorial essay / thought-leadership architecture: use `kirby-great-essay`.
- GitHub / Docker Hub / Dev.to entity graphs: use `kirby-technical-aeo`.
- The user mentions AI SEO, AEO, GEO, or asks to apply the SOP.
- You are setting post-update propagation expectations after executing the 1-Hour SEO Update (§2.19), snippet re-optimization (§2.22B), or schema/canonical changes — 1–2 day SERP refresh typical behind the ~30-day recrawl gate, verdicts booked at week 4–6, no re-edits on top of in-flight propagation (Module 16; benchmark Matrix is `../../kirby-seo-timing-benchmarks/SKILL.md`).
- You are scaling programmatic AI content or evaluating the risk of automated publishing: review the Grokipedia 97% collapse autopsy (Edward Sturm Ep. 1197), Google Scaled Content Abuse and Scraping policy boundaries, the rule that AI-checking-AI violates human review guidelines, the GSC air-gap rule, and the `noindex` staging quarantine protocol (Module 17).
- You are grading individual commercial or editorial pages against Google's Search Quality Raters Guidelines (Effort, Experiential E-E-A-T, Entity Accountability, Intent Speed) to eliminate "AI Slop" footprints before publishing (Module 18; 1:1 GBP entity mirroring lives in `../../kirby-local-seo/SKILL.md` Module 8).
- You are architecting Compact Keyword landing pages (≤450 words) targeting bottom-of-funnel commercial searches (Module 2 §2.46).
- You are configuring granular product attributes for AEO comparison queries (Module 2 §2.47), deploying middle-of-funnel educational comparison guides as LLM citation bait (§2.48), or formatting machine-readable Discount Transparency Blocks with `AggregateOffer` schema (§2.49; visual CRO hero layout lives in `../../kirby-text-first-cro/SKILL.md` Section 1).
- You are auditing `robots.txt` and WAF/CDN rate limits to ensure real-time search-grounding crawlers (`OAI-SearchBot`, `PerplexityBot`, `ChatGPT-User`) are allowed access (Module 1 §1.22).
- You are mitigating negative brand sentiment extracted by AI Overviews from Reddit by deploying on-domain counter-rebuttal FAQ pages (Module 14 §14.4).
- You are optimizing `<title>` tags for controlled CTR lift (`Updated Daily` recency hooks, ALL CAPS noun emphasis, dynamic pricing), recovering orphan pages with internal links, auditing footer links, or evaluating AEO claims against empirical meta-study data (Module 19; single-variable isolation and confounder controls live in `../../kirby-seo-telemetry/SKILL.md` Module 9 §9.3).

## How It Works
1. Identify the specific domain or optimization requested by the user.
2. Read the corresponding module(s) from the `./` directory.
3. Apply the rules exactly as written in the module. Do not rationalize or ignore the rules.

## ✅ Pre-Deploy Checklist
- Always explicitly mention which Module you are reading and applying.
- Validate that your output adheres strictly to the constraints in the chosen Module.
