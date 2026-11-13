# Research Companion — API and Operation Trace

**Private source:** `Amishgangsta/Locke-Research-Companion-Official`, deployed main commit `a05e53d886fda7ade46c67e76ebe6690a5ed5075`.

This traces each declared Express HTTP route across every `routes/` module. Paths are relative to their router mounts; dynamic public pages may share a handler. **A route declaration is not a claim of current entitlement, configured external services, or a newly executed request.**

## `routes/research.js` — 29 operations

| Method | Route | Source line |
|---|---|---:|
| GET | `/jurisdictions` | 51 |
| GET | `/jurisdictions/:code/courts` | 69 |
| GET | `/court-systems` | 96 |
| GET | `/surface` | 112 |
| GET | `/usage` | 125 |
| POST | `/check-usage` | 140 |
| GET | `/workspace` | 188 |
| PATCH | `/workspace` | 198 |
| POST | `/chat` | 290 |
| POST | `/chat/stream` | 328 |
| GET | `/documents/:id/ocr/:jobId` | 380 |
| GET | `/documents/:id/ocr/:jobId/review` | 397 |
| GET | `/documents/:id/ocr/review` | 414 |
| POST | `/documents/:id/ocr/:jobId/pages/:pageNumber/accept` | 431 |
| POST | `/documents/:id/ocr/:jobId/finalize` | 448 |
| POST | `/query` | 465 |
| POST | `/documents/upload` | 532 |
| POST | `/documents/:id/summarize` | 617 |
| POST | `/documents/:id/explain` | 651 |
| POST | `/documents/:id/questions` | 685 |
| POST | `/documents/:id/ocr` | 713 |
| GET | `/documents/:id` | 770 |
| DELETE | `/documents/:id` | 797 |
| GET | `/conversations` | 815 |
| GET | `/conversations/:id` | 831 |
| GET | `/history` | 846 |
| DELETE | `/history/:id` | 876 |
| POST | `/exports` | 915 |
| POST | `/ask` | 976 |

## `routes/research_companion.js` — 38 operations

| Method | Route | Source line |
|---|---|---:|
| GET | `/case-files` | 24 |
| GET | `/case-files/default` | 35 |
| POST | `/case-files` | 47 |
| GET | `/case-files/:id` | 69 |
| PATCH | `/case-files/:id` | 78 |
| POST | `/case-files/:id/archive` | 96 |
| POST | `/case-files/:id/restore` | 106 |
| DELETE | `/case-files/:id` | 120 |
| POST | `/documents/:id/attach-case-file` | 140 |
| GET | `/case-files/:id/documents` | 151 |
| GET | `/case-files/:id/timeline` | 165 |
| POST | `/case-files/:id/timeline` | 179 |
| PATCH | `/timeline/:id` | 201 |
| DELETE | `/timeline/:id` | 218 |
| POST | `/documents/:id/extract-dates` | 228 |
| POST | `/case-files/:id/timeline/add-selected` | 248 |
| GET | `/case-files/:id/issues` | 264 |
| POST | `/case-files/:id/issues` | 273 |
| GET | `/issues/:id` | 293 |
| PATCH | `/issues/:id` | 302 |
| DELETE | `/issues/:id` | 318 |
| POST | `/documents/:id/extract-issues` | 328 |
| GET | `/case-files/:id/facts` | 344 |
| POST | `/case-files/:id/facts` | 358 |
| PATCH | `/facts/:id` | 380 |
| DELETE | `/facts/:id` | 396 |
| POST | `/documents/:id/extract-facts` | 406 |
| GET | `/case-files/:id/attorney-prep` | 422 |
| POST | `/case-files/:id/attorney-prep` | 431 |
| GET | `/attorney-prep/:id` | 451 |
| GET | `/case-files/:id/reports` | 460 |
| POST | `/case-files/:id/reports` | 469 |
| GET | `/reports/:id` | 489 |
| GET | `/reports/:id/export/:format` | 498 |
| POST | `/case-files/:id/timeline/multi-document` | 541 |
| POST | `/case-files/:id/multi-document-review` | 575 |
| POST | `/case-files/:id/deep-review` | 607 |
| POST | `/case-files/:id/full-packet` | 637 |

## `routes/research_export.js` — 4 operations

| Method | Route | Source line |
|---|---|---:|
| GET | `/pdf` | 170 |
| POST | `/pdf` | 171 |
| GET | `/docx` | 172 |
| POST | `/docx` | 173 |

## `routes/auth.js` — 6 operations

| Method | Route | Source line |
|---|---|---:|
| POST | `/register` | 186 |
| POST | `/login` | 250 |
| POST | `/refresh` | 316 |
| POST | `/logout` | 404 |
| GET | `/dev-session` | 444 |
| GET | `/me` | 464 |

## `routes/admin.js` — 3 operations

| Method | Route | Source line |
|---|---|---:|
| GET | `/usage-report` | 15 |
| GET | `/health` | 26 |
| POST | `/purge-pending-documents` | 51 |

## `routes/administration.js` — 8 operations

| Method | Route | Source line |
|---|---|---:|
| POST | `/reauth` | 31 |
| GET | `/overview` | 34 |
| GET | `/users` | 35 |
| POST | `/users/:userId/revoke-sessions` | 36 |
| GET | `/operations` | 37 |
| POST | `/operations/purge-pending-documents` | 38 |
| GET | `/audit` | 39 |
| GET | `/audit/export` | 40 |

## `routes/public_jurisdictions.js` — 4 operations

| Method | Route | Source line |
|---|---|---:|
| GET | `/jurisdictions/` | 67 |
| GET | `/jurisdictions` | 69 |
| GET | `/jurisdictions/:code/` | 75 |
| GET | `/jurisdictions/:code` | 86 |

## `routes/public_pages.js` — 10 operations

| Method | Route | Source line |
|---|---|---:|
| GET | `/` | 41 |
| GET | `${path}/` | 44 |
| GET | `/jurisdictions/` | 53 |
| GET | `/jurisdictions` | 54 |
| GET | `/jurisdictions/:slug/` | 56 |
| GET | `/robots.txt` | 88 |
| GET | `/sitemap.xml` | 93 |
| GET | `/jurisdictions/:slug/courts/` | 98 |
| GET | `/jurisdictions/:slug/courts` | 104 |
| GET | `/jurisdictions/:slug` | 113 |

## Totals

**102 source-declared operations across 8 router modules.** Domain services and internal helper functions are inventoried separately in the [381-line feature register](FEATURE-MATRIX.md). No protected API was invoked during this comparison.

[Main portfolio](README.md) · [Sources](METHODOLOGY.md).