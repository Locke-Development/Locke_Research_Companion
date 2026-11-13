# Locke Research Companion — Feature-by-Feature Matrix (Part 1)

**Evidence snapshot:** private `Amishgangsta/Locke-Research-Companion-Official` at `a05e53d886fda7ade46c67e76ebe6690a5ed5075`, deployed November 12, 2026. Prepared November 13, 2026.

Every numbered line is a specific inspected source capability, **not** a newly executed E2E test or proof of superiority. `Not shipped` rows are deliberate, explicit exclusions. Competitor key: **L** Lexis+ with Protégé, **C** CoCounsel Legal, **V** vLex Vincent, **B** Bloomberg Law, **P** Paxton. `●` comparable published category, `≈` related category, `?` no verified exact counterpart. **None indicates absence.**

| Group | Count |
|---|---:|
| Legal research and source retrieval | 25 |
| Citation audit and honest sourcing | 21 |
| Ask Locke chat and continuity | 35 |
| Case files and tenancy | 21 |
| Document import and understanding | 28 |
| OCR job operations and review | 25 |
| Jurisdiction and court structure | 20 |


## Legal research and source retrieval (25)

**Source trace:** `routes/research.js`, `services/research_engine.js`, `services/legal_research.js`.

| # | Individual feature | Locke | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 1 | Quick research | Source-implemented | ● | ● | ● | ● | ● |
| 2 | Source-Backed research | Source-implemented | ● | ● | ● | ● | ● |
| 3 | Deep Research | Source-implemented | ● | ● | ● | ● | ● |
| 4 | Plain-English legal question | Source-implemented | ● | ● | ● | ● | ● |
| 5 | CourtListener case-law retrieval | Source-implemented | ● | ● | ● | ● | ● |
| 6 | Court opinion passage fetching | Source-implemented | ● | ● | ● | ● | ● |
| 7 | Congress.gov enacted-law retrieval | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 8 | Congress.gov bill retrieval | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 9 | eCFR regulatory retrieval | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 10 | Search-derived state statute retrieval | Source-implemented | ● | ● | ● | ● | ● |
| 11 | Concurrent source-provider queries | Source; runtime-dependent | ? | ? | ? | ? | ? |
| 12 | Deduplicated source results | Source-implemented | ● | ● | ● | ● | ● |
| 13 | Deep query decomposition | Source-implemented | ● | ● | ● | ● | ● |
| 14 | Multi-pass research | Source-implemented | ● | ● | ● | ● | ● |
| 15 | Bounded source excerpts | Source-implemented | ? | ? | ? | ? | ? |
| 16 | Stable source identifiers | Source-implemented | ● | ● | ● | ● | ● |
| 17 | Source URL rendering | Source-implemented | ● | ● | ● | ● | ● |
| 18 | Source title and citation | Source-implemented | ● | ● | ● | ● | ● |
| 19 | Uncited source visibility | Source-implemented | ● | ● | ● | ● | ● |
| 20 | Coverage warning on search-derived statutes | Source-implemented | ● | ● | ● | ● | ● |
| 21 | Actual provider-error warnings | Source; runtime-dependent | ? | ? | ? | ? | ? |
| 22 | State-statute skip disclosure | Source-implemented | ● | ● | ● | ● | ● |
| 23 | Jurisdiction scope in results | Source-implemented | ? | ? | ? | ? | ? |
| 24 | Court selection in results | Source-implemented | ● | ● | ● | ● | ● |
| 25 | Research history saving | Source-implemented | ● | ● | ● | ● | ● |

## Citation audit and honest sourcing (21)

**Source trace:** `services/citation_audit.js`, `services/research_engine.js`, `services/research_export_formats.js`.

| # | Individual feature | Locke | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 26 | Source-marker reconciliation | Source-implemented | ● | ● | ● | ● | ● |
| 27 | Unresolved marker detection | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 28 | Inline reporter citation detection | Source-implemented | ● | ● | ● | ● | ● |
| 29 | Statutory section reference detection | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 30 | Citation normalization | Source-implemented | ● | ● | ● | ● | ● |
| 31 | Compare citations with retrieved metadata | Source-implemented | ● | ● | ● | ● | ● |
| 32 | Flag unmatched citations | Source-implemented | ● | ● | ● | ● | ● |
| 33 | Block ungrounded sourced answer | Source-implemented | ● | ● | ● | ● | ● |
| 34 | Hold Source-Backed output until audit | Source-implemented | ● | ● | ● | ● | ● |
| 35 | Hold Deep output until audit | Source-implemented | ● | ● | ● | ● | ● |
| 36 | Log withheld audit verdict | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 37 | Clickable legal citation markers | Source-implemented | ● | ● | ● | ● | ● |
| 38 | Navigate to cited legal source | Source-implemented | ● | ● | ● | ● | ● |
| 39 | Keep document-source labels distinct | Source-implemented | ● | ● | ● | ● | ● |
| 40 | Include citations in exports | Source-implemented | ● | ● | ● | ● | ● |
| 41 | Include uncited sources in exports | Source-implemented | ● | ● | ● | ● | ● |
| 42 | Research verification notices | Source-implemented | ● | ● | ● | ● | ● |
| 43 | Separate skipped lookup from failed lookup | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 44 | No independent proposition verification (not implemented) | Not shipped | ? | ? | ? | ? | ? |
| 45 | No built-in Shepard’s/KeyCite citator (not implemented) | Not shipped | ? | ? | ? | ? | ? |
| 46 | No complete in-house primary statute index (not implemented) | Not shipped | ? | ? | ? | ? | ? |

## Ask Locke chat and continuity (35)

**Source trace:** `public/lr-chat-drawer.js`, `services/locke_research_service.js`, `services/chat_answer_parts.js`.

| # | Individual feature | Locke | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 47 | Open chat drawer | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 48 | Ask free-text question | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 49 | Quick/Source-Backed toggle | Source-implemented | ● | ● | ● | ● | ● |
| 50 | Default to Source-Backed mode | Source-implemented | ● | ● | ● | ● | ● |
| 51 | Start new conversation | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 52 | Open conversation history | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 53 | Resume past conversation | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 54 | Persist conversation ID | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 55 | Save chat turns to PostgreSQL | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 56 | Bound previous-turn context | Source-implemented | ? | ? | ? | ? | ? |
| 57 | Protect conversation tenant scope | Source-implemented | ? | ? | ? | ? | ? |
| 58 | Carry earlier question into short follow-up search | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 59 | Offer next-question suggestions | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 60 | Send follow-up suggestion | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 61 | Copy answer text | Source-implemented | ● | ● | ● | ● | ● |
| 62 | Render safe Markdown headings | Source-implemented | ? | ? | ? | ? | ? |
| 63 | Render safe Markdown lists | Source-implemented | ? | ? | ? | ? | ? |
| 64 | Render safe emphasis | Source-implemented | ? | ? | ? | ? | ? |
| 65 | Escape untrusted model HTML | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 66 | Render legal-citation pills | Source-implemented | ● | ● | ● | ● | ● |
| 67 | Render case-document pills | Source-implemented | ● | ● | ● | ● | ● |
| 68 | Open cited case document | Source-implemented | ● | ● | ● | ● | ● |
| 69 | Show jurisdiction scope | Source-implemented | ? | ? | ? | ? | ? |
| 70 | Show partial retrieval warning | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 71 | Show searching-sources state | Source-implemented | ● | ● | ● | ● | ● |
| 72 | Show citation-audit progress | Source-implemented | ● | ● | ● | ● | ● |
| 73 | Stream Quick-mode tokens | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 74 | Do not stream unchecked sourced answer | Source-implemented | ● | ● | ● | ● | ● |
| 75 | Retain usage for streaming | Source-implemented | ? | ? | ? | ? | ? |
| 76 | Provider-failure handling | Source; runtime-dependent | ? | ? | ? | ? | ? |
| 77 | No in-chat file attach control (not implemented) | Not shipped | ? | ? | ? | ? | ? |
| 78 | No in-chat jurisdiction override (not implemented) | Not shipped | ? | ? | ? | ? | ? |
| 79 | No answer-regeneration button (not implemented) | Not shipped | ? | ? | ? | ? | ? |
| 80 | No saved follow-up chips in resumed threads (not implemented) | Not shipped | ? | ? | ? | ? | ? |
| 81 | No reaction/feedback controls (not implemented) | Not shipped | ? | ? | ? | ? | ? |

## Case files and tenancy (21)

**Source trace:** `routes/research_companion.js`, `services/locke_research_case_files.js`.

| # | Individual feature | Locke | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 82 | Create case file | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 83 | List case files | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 84 | Default case file | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 85 | Change active case | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 86 | Load case dashboard | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 87 | Rename case | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 88 | Edit case description | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 89 | Save case jurisdiction | Source-implemented | ● | ● | ● | ● | ● |
| 90 | Save case court choice | Source-implemented | ● | ● | ● | ● | ● |
| 91 | Associate research with case | Source-implemented | ● | ● | ● | ● | ● |
| 92 | Archive case file | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 93 | Restore archived case file | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 94 | Title-confirmed permanent delete | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 95 | Transactional case metadata erasure | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 96 | Restrict mutations on archived case | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 97 | Firm-scoped case access | Source-implemented | ? | ? | ? | ? | ? |
| 98 | User-scoped case access | Source-implemented | ? | ? | ? | ? | ? |
| 99 | Get case counts | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 100 | Attach existing document to case | Source-implemented | ● | ● | ● | ● | ● |
| 101 | List documents within case | Source-implemented | ● | ● | ● | ● | ● |
| 102 | Keep issues/facts in same case | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |

## Document import and understanding (28)

**Source trace:** `routes/research.js`, `services/locke_research_documents.js`.

| # | Individual feature | Locke | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 103 | Upload PDF | Source-implemented | ● | ● | ● | ● | ● |
| 104 | Upload DOCX | Source-implemented | ● | ● | ● | ● | ● |
| 105 | Upload TXT | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 106 | Upload Markdown | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 107 | Validate allowed extension | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 108 | Validate content type | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 109 | Bound upload byte size | Source-implemented | ? | ? | ? | ? | ? |
| 110 | Sanitize file name | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 111 | Store document for owner | Source-implemented | ● | ● | ● | ● | ● |
| 112 | Extract text-bearing PDF | Source-implemented | ● | ● | ● | ● | ● |
| 113 | Extract DOCX XML | Source-implemented | ● | ● | ● | ● | ● |
| 114 | Guard compressed DOCX expansion | Source-implemented | ? | ? | ? | ? | ? |
| 115 | Extract text file | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 116 | Read page count | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 117 | Detect weak PDF text layer | Source-implemented | ● | ● | ● | ● | ● |
| 118 | Mark scan for OCR | Source; runtime-dependent | ● | ● | ● | ● | ● |
| 119 | Show extraction status | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 120 | Get document details | Source-implemented | ● | ● | ● | ● | ● |
| 121 | List case documents | Source-implemented | ● | ● | ● | ● | ● |
| 122 | Search case documents | Source-implemented | ● | ● | ● | ● | ● |
| 123 | Summarize uploaded file | Source-implemented | ● | ● | ● | ● | ● |
| 124 | Explain uploaded document in plain English | Source-implemented | ● | ● | ● | ● | ● |
| 125 | Generate attorney questions from document | Source-implemented | ● | ● | ● | ● | ● |
| 126 | Supply bounded documents as AI context | Source-implemented | ? | ? | ? | ? | ? |
| 127 | Exclude private document content from public searches | Source-implemented | ● | ● | ● | ● | ● |
| 128 | Soft-delete document | Source-implemented | ● | ● | ● | ● | ● |
| 129 | Purge document artifacts | Source-implemented | ● | ● | ● | ● | ● |
| 130 | Retry pending purge | Source-implemented | ? | ? | ? | ? | ? |

## OCR job operations and review (25)

**Source trace:** `services/ocr_engine.js`, `services/locke_research_ocr_jobs.js`, `routes/research.js`.

| # | Individual feature | Locke | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 131 | Rasterize scanned PDF | Source-implemented | ● | ● | ● | ● | ● |
| 132 | Tesseract OCR worker | Source; runtime-dependent | ? | ? | ? | ? | ? |
| 133 | Reuse OCR worker | Source; runtime-dependent | ? | ? | ? | ? | ? |
| 134 | Page-count safety cap | Source-implemented | ? | ? | ? | ? | ? |
| 135 | DPI safety cap | Source-implemented | ? | ? | ? | ? | ? |
| 136 | Language configuration | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 137 | Create durable OCR job | Source; runtime-dependent | ● | ● | ● | ● | ● |
| 138 | Dedupe OCR by document fingerprint | Source; runtime-dependent | ? | ? | ? | ? | ? |
| 139 | Reserve OCR usage | Source; runtime-dependent | ? | ? | ? | ? | ? |
| 140 | Claim OCR job | Source; runtime-dependent | ● | ● | ● | ● | ● |
| 141 | Renew worker claim | Source-implemented | ? | ? | ? | ? | ? |
| 142 | Record OCR page result | Source; runtime-dependent | ● | ● | ● | ● | ● |
| 143 | Distinguish recognized/empty/failed page | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 144 | View OCR job status | Source; runtime-dependent | ● | ● | ● | ● | ● |
| 145 | View OCR correction interface | Source; runtime-dependent | ? | ? | ? | ? | ? |
| 146 | Accept corrected page text | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 147 | Finalize accepted OCR job | Source; runtime-dependent | ● | ● | ● | ● | ● |
| 148 | Cancel running OCR job | Source; runtime-dependent | ● | ● | ● | ● | ● |
| 149 | Retry OCR job | Source; runtime-dependent | ? | ? | ? | ? | ? |
| 150 | Recover stale claim | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 151 | Preserve original scan fingerprint | Source-implemented | ? | ? | ? | ? | ? |
| 152 | Keep corrected and accepted versions | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 153 | Guard OCR access by firm | Source; runtime-dependent | ? | ? | ? | ? | ? |
| 154 | Time out slow page processing | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 155 | Attach accepted OCR text to document | Source; runtime-dependent | ● | ● | ● | ● | ● |

## Jurisdiction and court structure (20)

**Source trace:** `services/locke_research_jurisdiction.js`, `services/locke_research_courts.js`, `services/locke_research_scope.js`.

| # | Individual feature | Locke | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 156 | All 50 U.S. state options | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 157 | District of Columbia option | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 158 | Federal jurisdiction option | Source-implemented | ● | ● | ● | ● | ● |
| 159 | Normalize state abbreviation | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 160 | Canonical jurisdiction codes | Source-implemented | ● | ● | ● | ● | ● |
| 161 | Federal appellate groups | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 162 | Federal district-court groups | Source-implemented | ● | ● | ● | ● | ● |
| 163 | State supreme-court groups | Source-implemented | ● | ● | ● | ● | ● |
| 164 | Intermediate appeal groups | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 165 | General trial court groups | Source-implemented | ● | ● | ● | ● | ● |
| 166 | Limited-jurisdiction court groups | Source-implemented | ● | ● | ● | ● | ● |
| 167 | State-specific structural overrides | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 168 | Validate selected court in jurisdiction | Source-implemented | ● | ● | ● | ● | ● |
| 169 | Reject invalid court ID | Source-implemented | ● | ● | ● | ● | ● |
| 170 | Store default court per case | Source-implemented | ● | ● | ● | ● | ● |
| 171 | Display court hierarchy labels | Source-implemented | ● | ● | ● | ● | ● |
| 172 | Publish public jurisdiction directory | Source-implemented | ● | ● | ● | ● | ● |
| 173 | Publish court hierarchy pages | Source-implemented | ● | ● | ● | ● | ● |
| 174 | Carry scope into answer | Source-implemented | ? | ? | ? | ? | ? |
| 175 | Identify unverified structure instead of inventing a court | Source-implemented | ? | ? | ? | ? | ? |

**Verification distinctions:** `Source-Backed` citation matching is not a validated legal-proposition citator. Case-law and state-statute coverage are provider-/retrieval-dependent; state statutes are search-derived. [Part 2](FEATURE-MATRIX-2.md) covers the remaining platform and workflow capabilities.

[Five competitors](COMPARISON.md) · [Ask Locke](ASK-LOCKE.md) · [Sources and limitations](METHODOLOGY.md).