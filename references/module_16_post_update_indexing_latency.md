# Module 16: Post-Update Indexing Latency & Propagation Expectations (Illyes Oct 2026)

*Source: Google's official processing-pipeline benchmarks (Gary Illyes, Search Central Live Deep Dive Europe, Barcelona, Oct 2, 2026; analyzed by Edward Sturm, Ep. E1192). Benchmark Matrix, confidence tiers, and forecast math live in `../../kirby-seo-timing-benchmarks/SKILL.md` — this module aligns this skill's execution protocols to Google's measured refresh reality. Do not duplicate the Matrix here.*

## 16.1 The Latency Alignment Problem

This skill's flagship protocols are fast by design — the 1-Hour SEO Update (§2.19) executes title/`<h1>`/opening-hook changes in an hour. Google's side of that transaction is not fast in the same unit: **title and snippet changes refresh in SERPs 1–2 days typical — and only after the page is recrawled, which runs on a ~30-day default cadence.** Misaligned expectations produce false-negative verdicts (declaring an update failed while propagation is still in flight) and resubmission spam (which cannot accelerate anything).

## 16.2 The Propagation Timeline (per change class)

| Change (this skill's protocol) | Agent-side effort | Google-side typical refresh | Governing gate | Verdict window |
|---|---|---|---|---|
| `<title>` / meta description / `<h1>` / opening hook (§2.19 1-Hour SEO Update) | ~1 hour | 1–2 days SERP refresh | ~30-day recrawl of the edited page | Measure at 4–6 weeks |
| JSON-LD / schema changes | Hours | Recrawl + re-processing | Recrawl cadence | 4–6 weeks (rich-result status may lag further) |
| Canonical / consolidation changes | Hours | 1–3 weeks convergence | Signal cleanliness (internal links, sitemap, 301 conflicts extend to months) | 8 weeks |
| New URLs (new content per §2.37 SERP-overlap test) | Days | ~20h discovery + from ~1.5h index pipeline | Scheduler priority | Indexed-or-classified by Day 14–21 |
| Snippet re-optimization (§2.22B) | Hours | 1–2 days post-recrawl | Recrawl cadence | 4–6 weeks |

**Rules:**
1. **Never book a verdict inside the verdict window.** A 1-Hour SEO Update's GSC delta is read at week 4–6 minimum; the existing 14–21 day QDF cooldown for query-augmentation write-backs (§2.36F discipline, `../../kirby-seo-telemetry/SKILL.md` Module 9) is a floor, not the ceiling, for title/snippet-bearing changes.
2. **Never re-edit on top of in-flight propagation.** Serial §2.19 passes on the same URL inside the recrawl window confound attribution — the SERP may reflect neither, either, or a blend.
3. **Hot-path exemption:** pages linked from frequently crawled surfaces (homepage, hub donors per §10.11) refresh faster than the ~30d default; the sanctioned compression levers are in `../../kirby-seo-timing-benchmarks/SKILL.md` Reference 05 (internal-link re-pointing, GSC URL Inspection within quota — never bulk resubmission).
4. **Slow-tail classification:** a title/snippet change not reflected ~60 days post-deploy, with clean crawl capacity, is a crawl-deprioritization or quality signal — route to the triage protocol (`../../kirby-seo-timing-benchmarks/SKILL.md` Reference 03 §3.4), not another edit pass.

## 16.3 Protocol Touch-Points (alignment, not duplication)

- **§2.19 (1-Hour SEO Update):** execution unchanged; add the propagation annex to client/internal reporting — "executed in 1 hour, visible in SERPs 1–2 days after Google's next recrawl (~30-day default), measured at week 4–6."
- **§2.36F (query-augmentation write-back) & Module 9 cooldown discipline:** verdict windows per the table above; telemetry instrumentation of the watch thresholds is `../../kirby-seo-telemetry/SKILL.md` Module 12.
- **§1.16 (Crawled/Discovered - not indexed router):** the benchmark-backed stall boundaries (T2: 14 days undiscovered; 60 days in Crawled-not-indexed) sharpen that router's escalation timing; diagnosis doctrine is `../../kirby-seo-timing-benchmarks/SKILL.md` Reference 03.
- **§1.20 (fresh-domain AI Overview quarantine):** unchanged; orthogonal to organic-indexing latency.

## 16.4 Routing Map
*   Benchmark table, confidence tiers, forecasting math → `../../kirby-seo-timing-benchmarks/SKILL.md` Reference 01–02.
*   Stall instrumentation (T1/T2 thresholds, stage-chained alerts) → `../../kirby-seo-telemetry/SKILL.md` Module 12.
*   Deployment-side verification gates for meta changes (CI asserting on-page correctness at deploy, SERP-reflection deferred) → `../../kirby-seo-deployment/SKILL.md` Module 20 §20.3.
*   Client-facing SLA language and expectation scripts → `../../kirby-seo-timing-benchmarks/SKILL.md` Reference 04.
