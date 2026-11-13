# Locke Research Companion — Audit Method and Primary Sources

**Audit date:** November 13, 2026. **Purpose:** public engineering portfolio for future development clients and employers.

## Locke's own current evidence

- Private source: Amishgangsta/Locke-Research-Companion-Official; inspected main SHA a05e53d886fda7ade46c67e76ebe6690a5ed5075.
- Railway: Research-Companion-Official, successful production deployment of identical commit on November 12, 2026.
- Application modules inspected: services/research_engine.js, legal_research.js, citation_audit.js, chat_answer_parts.js, locke_research_service.js, locke_research_case_files.js, locke_research_companion.js, locke_research_documents.js, locke_research_ocr_jobs.js, locke_research_courts.js, locke_research_jurisdiction.js, locke_research_guard.js, model_router.js, llm_stream.js, research_export_formats.js, and others.
- User experience inspected: public/lr-chat-drawer.js, services/public_pages.js, ui-preview/src/pages, UI navigation definitions, and product demo integration.
- Declared routes inspected: routes/research.js, research_companion.js, research_export.js, auth.js, admin.js, administration.js, public_jurisdictions.js, public_pages.js.
- November 12 handoff and red-team records inspected read-only. Existing CI status verified; no new tests or provider benchmarking.

## Primary competitor sources

| Vendor (current 2026 name) | Vendor-maintained documentation |
|---|---|
| Lexis+ with Protégé (renamed from Lexis+ AI in February 2026) | [Official product](https://www.lexisnexis.com/en-us/products/lexis-plus-protege.page), [AI legal research](https://www.lexisnexis.com/en-us/products/lexis-plus-protege/legal-research.page) |
| Thomson Reuters CoCounsel Legal / Westlaw Advantage | [CoCounsel features](https://legal.thomsonreuters.com/en/products/cocounsel-legal/features), [Westlaw Advantage](https://legal.thomsonreuters.com/en/products/westlaw-advantage/features), [August 2026 launch](https://www.thomsonreuters.com/en/press-releases/2026/august/thomson-reuters-launches-next-generation-of-cocounsel-legal-the-ai-ecosystem-built-for-legal-professionals) |
| vLex Vincent AI | [Workflow list](https://knowledge.vlex.com/en/vincent-ai), [Source-cited research](https://knowledge.vlex.com/en/features/vincent/ask-a-research-question) |
| Bloomberg Law | [Legal research product](https://pro.bloomberglaw.com/products/legal-research-and-software/legal-research/), [AI and BCITE](https://pro.bloomberglaw.com/about/our-approach-to-ai/), [2026 Deep Research](https://bna.content.cirrus.bloomberg.com/blaw2023/insights/legal-solutions/can-ai-handle-complex-legal-research/) |
| Paxton AI | [Legal research product](https://www.paxton.ai/legal-research), [Research in Assistant](https://www.paxton.ai/post/introducing-drafting-and-answering-with-legal-research-in-assistant) |

## What the symbols mean

**Source-implemented:** specific inspected code exists. **Conditional:** feature needs an enabled plan, AI provider, accepted file or running background service. **Not shipped / not configured:** current source does not establish availability. **●:** a competitor publicly documents a comparable broad feature category. **≈:** a related competitor capability exists, exact parity unknown. **?:** exact match cannot be verified in public sources. **? never means absence**.

The detailed 381-item matrix uses **category-level competitor mappings**, not independently tested results for all 1,905 competitor-feature permutations; the 51-row executive matrix adds more nuanced market context. No peer source repository or customer account was inspected.

## Material caveats

- Citation checks match markers, case and statute references against retrieved source records, not an independent Shepard's/KeyCite authority review.
- State statutes are search-derived rather than an authoritative ingested complete state-code corpus.
- Uploaded private documents may be summarized/analysed, but model answers remain probabilistic.
- No current publicly established subscription pricing: source catalog says 'Pricing not set'; internal planning numeric values must not be quoted.
- No performance benchmarks, independent legal-accuracy study, legal outcomes, security certification or proof of superior library breadth.
- Successful production deployment and recorded CI do not prove every user journey works in all environments.

## Protected materials

The public repository contains descriptions, provenance and approved branding assets only. It contains no proprietary server code, legal content corpus, API secrets, customer records or internal security exploit instructions.

[Brochure](BROCHURE.md) · [Research source limits](CITATION-AND-SOURCES.md) · [Full feature matrix](FEATURE-MATRIX.md) · [Status](VERIFICATION-AND-STATUS.md)