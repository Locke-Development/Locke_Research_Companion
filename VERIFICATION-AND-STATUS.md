# Locke Research Companion — Verified Source Status

**Source:** Amishgangsta/Locke-Research-Companion-Official, main commit a05e53d886fda7ade46c67e76ebe6690a5ed5075 (November 12, 2026).

**Production:** Railway Research-Companion-Official successfully deployed that exact commit to lockeresearchcompanion.com. GitHub CI reports success at that commit. November 12 handoff documents record 629 passing tests with one intentional skip; no tests were rerun for this portfolio review.

| Surface | Current evidence | Qualification |
|---|---|---|
| Quick/Source-Backed/Deep legal research | Source implemented | Provider and retrieval availability vary |
| Case law and federal law | CourtListener, Congress.gov, eCFR connectors in source | Not a licensed comprehensive citator library |
| State statutes | Search-derived source links | No maintained primary state-law text index |
| Source-backed citation audit | Matches citation strings and markers to retrieved source metadata | Not full quotation, holding, subsequent-history verification |
| Source-backed output gate | Failed-audit answers withheld before display | Quick answers may stream without source verification |
| Ask Locke chat memory | Database-stored conversations and scoped history | Account/firm boundaries apply |
| Follow-ups, Markdown and document pills | Source and regression coverage | Follow-ups not persisted across resumed threads |
| Case files, chronology, issues and facts | Individual services, UI and API operations | Models' suggested content requires review |
| Document extraction, scanned OCR | PDF/DOCX/text and local OCR paths | Quality, file format and runtime dependencies apply |
| Attorney preparation, reports, full case packet | Source-present generation pipelines | Output not independently verified legal work product |
| Export PDF/DOCX | Renderers, quotas and idempotency in source | Export labels are not professional accuracy certifications |
| Commercial price | Product catalog displays 'Pricing not set' | Internal numeric constants are not published quotations |
| Chat drawer file attachment, picker, regenerate and feedback | Not shipped per current handoff | Workflows elsewhere can attach documents |
| Independent third-party security certification | Cannot verify from available sources | Source red-team and CI are distinct from external certification |

**Production status distinction:** successful deployment confirms the code version is serving, not every external provider or authenticated workflow passing a new independent run.

## November 12 remediation record

Current code and later handoff indicate the source red-team remediations were merged and deployed; earlier same-day documents that say changes remained on a branch are historical snapshots. The public portfolio does not reproduce exploitable technical details.

## Scope of this portfolio audit

Two [feature-register files](FEATURE-MATRIX.md) enumerate **381 individual entries** across 18 areas, including explicitly unshipped ones. [Route trace](ROUTE-TRACE.md) lists **102 declared API operations** in eight modules. [Ask Locke](ASK-LOCKE.md) records **49 individual behaviors**. [Competitive comparison](COMPARISON.md) checks 51 market-relevant rows.

[Research evidence](METHODOLOGY.md) · [Citation limitations](CITATION-AND-SOURCES.md) · [Portfolio](README.md)