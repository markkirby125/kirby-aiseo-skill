# Module 20: Pre-Publication Semantic Drift Gate ("Before You Publish")

*Source: Kasra Dash breakdown of the Nov 2026 Core Update (second-hand, single-source, unverified against Google docs). `siteFocusScore` / `siteRadius` are names from leaked-attribute commentary; the live values are NOT observable. Never report a numeric score for them. This gate is a pass/fail proxy.*

**Premise (directional):** publishing off-axis pages (e.g., a trade site posting recipes or crypto) may widen the domain's semantic radius and dilute site focus. Extends Module 2 §2.25 (hop-distance rule) from "is this topic near my entity?" to "does it fit what this site already has?". Does not replace Module 2 §2.32B (Information-Gain acid test): run this gate FIRST, §2.32B second.

## 20.1 Inputs (no tool = `[Pending Connection]`)
1. Candidate list: keyword + intended page type, from the user or [`kirby-grounded-seo-auditor`](../../kirby-grounded-seo-auditor/SKILL.md).
2. Inventory: indexed URLs and titles from the sitemap, GSC Pages export, or `site:` harvest (Module 10 §10.11A). Core entity/service statement from Module 2 §2.42 Who/What/Why.

## 20.2 Per-candidate tests (all discrete)
| # | Test | Fail action |
|---|---|---|
| 1 | Hop distance to the core entity ≤ 2 logical questions (Module 2 §2.25B) | REJECT |
| 2 | Nearest existing URL on the same entity-attribute pair? | Yes → run Module 2 §2.37 overlap test; update that page, do not publish a new one |
| 3 | Fits an existing topical cluster/map (Module 2 §2.39 Map 1)? | No → REWORK as a spoke of a cluster, or REJECT |
| 4 | Supports a conversion path (service, quote, booking, proof)? | No → REJECT unless it passes the Module 2 §2.25B foundational-science rule |
| 5 | Commercial intent matches the site's page-type mix (Module 2 §2.35 vs informational)? | Mismatch → REWORK |

## 20.3 Output
Write `publish-gate.md`: candidate | tests failed | verdict (ACCEPT / REWORK / REJECT) | nearest URL. Draft ONLY ACCEPTed rows. List rejected terms so they are not re-proposed.

## 20.4 Boundaries
- Existing off-axis legacy pages: prune per Module 2 §2.34 / [`kirby-seo-deployment`](../../kirby-seo-deployment/SKILL.md) Module 7 §7.12; never mid-core-rollout (`../../kirby-seo-telemetry/SKILL.md` Module 16 §16.2 / Module 16 §16.2 rule 6 here).
- Truly separate topics or vertical pivots: subdomain chunking (Module 1 §1.12E), not the main hub.
- Examples: a local trade directory publishing general DIY/lifestyle news, or a regional B2B IT MSP publishing hospitality food-wholesale ERP audits on its main domain.
