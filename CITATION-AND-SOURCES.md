# Locke Research Companion — Source Verification and Research Boundaries

**Reviewed November 13, 2026 · Source commit a05e53d886fda7ade46c67e76ebe6690a5ed5075**

## What the citation gate really checks

Locke retrieves selected legal material from CourtListener, Congress.gov, eCFR and state-statute search links. Source markers such as [1] are compared to retrieved item identifiers. The audit also detects reporter citations, statutory section references and some case names that are not matched to retrieved source metadata. For Source-Backed and Deep modes, a blocking audit causes the answer to be withheld before display.

| Verification stage | Source-implemented | Does not prove |
|---|---|---|
| Search CourtListener opinions | Source hits and bounded passages | Exhaustive or current coverage of all cases |
| Search Congress.gov and eCFR | Federal law, bills and regulations | Full editorial or citator analysis |
| Seek state statutes through web search | Links labeled search-derived | Independently maintained authoritative state-code corpus |
| Reconcile numbered citations | Marks matched to retrieved items | The cited authority supports the proposition in the answer |
| Compare reporter and statutory citation strings | Detect unmatched citations | Exact quotation, subsequent history, negative treatment or full semantic verification |
| Hold sourced answers pending audit | Avoid premature display of an answer failing the audit | Legal correctness or attorney validation |
| Reference private case documents separately | D1-style citations identify included uploaded documents | Passage-level pinpoints and independent evidence authentication |
| Export citation and coverage notes | Readers see audit limitations | Court-ready legal verification certificate |

## Competitive reality

Lexis+ with Protégé offers Shepard's citation treatment, CoCounsel Legal/Westlaw offers KeyCite and Deep Research Verify, and Bloomberg Law offers BCITE. These are deeper citator systems than Locke's current metadata-based source-matching audit. Vincent and Paxton also provide clickable, source-grounded legal research.

Vendor sources: [Lexis+ Protégé](https://www.lexisnexis.com/en-us/products/lexis-plus-protege.page) · [CoCounsel](https://legal.thomsonreuters.com/en/products/cocounsel-legal/features) · [Vincent AI](https://knowledge.vlex.com/en/vincent-ai) · [Bloomberg Law](https://pro.bloomberglaw.com/about/our-approach-to-ai/) · [Paxton](https://www.paxton.ai/legal-research).

## What makes the implementation worth showing

The November 12 design update stops source-backed output from appearing before its citation audit finishes. Quick-mode answers can still stream. Skipped state-statute retrieval is explained honestly instead of being labeled a provider outage, while actual retrieval failures receive their own warnings.

**Conclusion:** a concrete, inspectable trust boundary—not a demonstrated legal-accuracy ranking. See [Ask Locke](ASK-LOCKE.md), [complete comparison](COMPARISON.md), and [verification status](VERIFICATION-AND-STATUS.md).