# ASK LOCKE — DEEP FEATURE AND COMPETITOR REVIEW
### Research Companion's conversational research engine, assessed individually

**Evidence date:** November 13, 2026. **Source snapshot:** deployed commit `a05e53d886fda7ade46c67e76ebe6690a5ed5075`. This review is for software-development prospects and hiring managers who need concrete implementation evidence, not slogans about a chatbot.

## What Ask Locke actually does

Ask Locke accepts plain-English research questions inside an active case-file workspace. The drawer offers Quick and Source-Backed modes; a separate Legal Research screen also offers Deep Research. The system uses the selected U.S. jurisdiction and court system, retrieves documents and legal sources where appropriate, saves conversation history, and returns citations and follow-up navigation.

**The crucial November 12 change:** Quick answers stream, but source-backed answers **remain hidden until the citation audit finishes**. This protects users from seeing unaudited citations briefly before an answer is withdrawn.

### 1 — Context and continuity
Conversations are persisted in `research_runs` with a conversation ID. Prior turns are retrieved using the user's own firm and account context, and short follow-up searches can incorporate the previous user question so the retrieval query does not lose its subject.

### 2 — Legal retrieval and citation display
Source-backed research can retrieve CourtListener case law, federal law/bills through Congress.gov, federal regulations through eCFR, and **search-derived** state statutory links. Answers include matched sources, clickable authority citations, and explicit provider/coverage warnings. It does not have a proprietary citator equivalent to Shepard's/KeyCite.

### 3 — Private case documents
Selected case-file documents can be included as bounded private context. A `[D1]` marker is a **document** citation distinct from `[1]` for a retrieved authority. The user can open a cited uploaded document, but page-level pinpoint citations have not been implemented in the recorded chat design.

### 4 — UX and failure behavior
The drawer provides progress states, safe Markdown, citation chips, copy, New, History, and follow-up suggestions. When no valid source-backed answer survives the audit, the system withholds it rather than labeling it verified. The provider-routing layer has failover and usage accounting controls.

## All 49 individually examined behaviors

Key: **L** Lexis+ with Protégé; **C** CoCounsel Legal; **V** vLex Vincent; **B** Bloomberg Law; **P** Paxton. **●** broadly documented equivalent category; **≈** related capability; **?** exact implementation not publicly verified. No `?` claims the competitor lacks a feature.

| # | Individual behavior | Locke | L | C | V | B | P | Comparative finding |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|---|
| 1 | Ask an open-ended question | **Source ✓** | ● | ● | ● | ● | ● | Category tie |
| 2 | Choose Quick orientation mode | **Source ✓** | ● | ● | ● | ● | ● | All five offer AI question answering; speed semantics differ |
| 3 | Choose Source-Backed mode | **Source ✓** | ● | ● | ● | ● | ● | All five retrieve legal materials; same guarantee not implied |
| 4 | Choose Deep Research mode | **Source ✓** | ● | ● | ● | ● | ● | Many peers also support deep or multistep work |
| 5 | Source-Backed default in drawer | **Source ✓** | ≈ | ≈ | ≈ | ≈ | ≈ | Locke UX setting verified |
| 6 | Use active case jurisdiction | **Source ✓** | ● | ● | ● | ● | ● | Peer jurisdiction-aware research is documented |
| 7 | Use selected court system | **Source ✓** | ≈ | ≈ | ≈ | ≈ | ≈ | Specific Locke scope binding demonstrated |
| 8 | Persist chat turns to database | **Source ✓** | ● | ● | ● | ● | ● | Competitors preserve histories |
| 9 | Reuse conversation ID | **Source ✓** | ≈ | ≈ | ≈ | ≈ | ≈ | Locke continuity mechanism inspected |
| 10 | Resume prior conversation | **Source ✓** | ● | ● | ● | ● | ● | History and workspace continuity are widespread |
| 11 | Use prior-turn context in new question | **Source ✓** | ● | ● | ● | ● | ● | Multi-turn conversation is category standard |
| 12 | Heuristically expand follow-up search using earlier question | **Source ✓** | ≈ | ≈ | ≈ | ≈ | ≈ | Specific implementation verified; peer matching unknown |
| 13 | Guard prior-turn retrieval by firm and user | **Source ✓** | ? | ? | ? | ? | ? | Internal tenancy rules not comparable publicly |
| 14 | Default legal research response grounded in retrieval | **Source ✓** | ● | ● | ● | ● | ● | Tie in broad legal retrieval |
| 15 | Retrieve CourtListener opinions | **Source ✓** | ≈ | ≈ | ≈ | ≈ | ≈ | Specific public-data connection rather than proprietary citator |
| 16 | Retrieve Congress.gov federal law and bills | **Source ✓** | ● | ● | ● | ● | ● | Primary federal law availability across peers |
| 17 | Retrieve eCFR regulations | **Source ✓** | ● | ● | ● | ● | ● | Regulatory research standard |
| 18 | Retrieve state statutes via search-derived links | **Source ✓** | ● | ● | ● | ● | ● | More fragile than authoritative ingested citation datasets |
| 19 | Disclose intentionally skipped statute search | **Source ✓** | ? | ? | ? | ? | ? | Specific transparency control |
| 20 | Distinguish actual retrieval failure from deliberate skip | **Source ✓** | ? | ? | ? | ? | ? | Specific implementation check |
| 21 | Include stable [1]-style source marker | **Source ✓** | ● | ● | ● | ● | ● | Citation links common |
| 22 | Render clickable legal source citation | **Source ✓** | ● | ● | ● | ● | ● | Tie on clickable sources |
| 23 | Detect out-of-range source marker | **Source ✓** | ≈ | ≈ | ≈ | ≈ | ≈ | Specific marker-integrity check |
| 24 | Detect unmatched reported citation strings | **Source ✓** | ● | ● | ● | ● | ● | Peers offer more extensive verification systems |
| 25 | Audit citations against retrieved metadata | **Source ✓** | ● | ● | ● | ● | ● | Not full legal treatment verification |
| 26 | Withhold Source-Backed output until audit completes | **Source ✓** | ≈ | ≈ | ≈ | ≈ | ≈ | Specific safeguard implemented |
| 27 | Withhold Deep output until audit completes | **Source ✓** | ≈ | ≈ | ≈ | ≈ | ≈ | Specific safeguard implemented |
| 28 | Stream Quick text updates | **Source ✓** | ● | ● | ● | ● | ● | Category tie on streaming interaction |
| 29 | Avoid streamed unaudited sourced answer | **Source ✓** | ≈ | ≈ | ≈ | ≈ | ≈ | Explicit design decision |
| 30 | Show progress while retrieving sources | **Source ✓** | ● | ● | ● | ● | ● | Research progress widely available |
| 31 | Show progress while auditing answer | **Source ✓** | ≈ | ≈ | ≈ | ≈ | ≈ | Specific implementation |
| 32 | Render formatted headings, lists and emphasis | **Source ✓** | ● | ● | ● | ● | ● | Basic UX tie |
| 33 | Escape embedded HTML from untrusted model output | **Source ✓** | ? | ? | ? | ? | ? | Internal safety implementation |
| 34 | Return up to three follow-up question chips | **Source ✓** | ● | ● | ● | ● | ● | Comparable conversational prompts |
| 35 | Send a follow-up chip as question | **Source ✓** | ● | ● | ● | ● | ● | Tie at workflow category |
| 36 | Copy answer text | **Source ✓** | ● | ● | ● | ● | ● | Category standard |
| 37 | Link [D1] documentary citation to uploaded case file | **Source ✓** | ● | ● | ● | ● | ● | Competitors also cite uploaded documents |
| 38 | Check cited document was included in model context | **Source ✓** | ≈ | ≈ | ≈ | ≈ | ≈ | Specific label validation |
| 39 | Display research scope and retrieval warnings | **Source ✓** | ● | ● | ● | ● | ● | Peers expose scope and uncertainty |
| 40 | Provider/model provenance on saved run | **Source ✓** | ≈ | ≈ | ≈ | ≈ | ≈ | Locke implementation detail |
| 41 | Account for streaming usage | **Source ✓** | ? | ? | ? | ? | ? | Operational rather than user superiority |
| 42 | Fail over provider before partial answer is shown | **Source ✓** | ? | ? | ? | ? | ? | Specific reliability policy |
| 43 | Create new thread | **Source ✓** | ● | ● | ● | ● | ● | Tie |
| 44 | Open History and resume | **Source ✓** | ● | ● | ● | ● | ● | Tie |
| 45 | Attach document from in-drawer button | **Not shipped** | ? | ? | ? | ? | ? | **Not implemented in current drawer** |
| 46 | Change jurisdiction from in-drawer picker | **Not shipped** | ? | ? | ? | ? | ? | **Not implemented in current drawer** |
| 47 | Regenerate prior answer with one click | **Not shipped** | ? | ? | ? | ? | ? | **Not implemented** |
| 48 | Persist follow-up chips on re-opened thread | **Not shipped** | ? | ? | ? | ? | ? | **Not implemented** |
| 49 | Validate legal proposition against full opinion and subsequent treatment | **Not shipped** | ● | ● | ● | ● | ● | **Not implemented as dedicated verification in Locke; Lexis/Westlaw have advanced citators** |

## Competitor-specific countercheck

**Lexis+ with Protégé:** conversational legal research, linked citations, Shepard's signals, external document Vault, deeper research and integrated drafting. It is inaccurate to claim Locke is more authoritative or more fully verified.

**CoCounsel Legal / Westlaw:** Westlaw and Practical Law source integration, agentic Deep Research, citation and legal-proposition verification, Word drafting, matter Workspaces and litigation analysis. Locke's source matching is narrower.

**vLex Vincent AI:** cited global-law research and memos, matter/knowledge collections, jurisdiction comparison, case analysis, document workflows and timeline generation. Locke's case-organization integration is a concrete project example but not exclusive.

**Bloomberg Law:** AI assistant, Deep Research, BCITE, Brief Analyzer, legal news/dockets, litigation analytics and authoritative legal research. Its coverage and professional research ecosystem are larger than this independent product's known source set.

**Paxton AI:** research in the AI Assistant, clickable source citations, document review, legal drafting, file analysis, medical chronology, and AI citator. Locke's documented Quick/source-backed gate is inspectable, but Paxton also has sourced conversational AI.

## Limitations acknowledged in the current source

- Full source-text/legal-proposition verification and case-negative-treatment analysis are not equivalent to the current citation-marker audit.
- State statutes remain search-derived; there is no fully maintained independent statute corpus.
- No in-drawer file attach or jurisdiction picker; those controls exist elsewhere in the workspace.
- Answer regeneration, feedback controls and persistent follow-up chips are not implemented.
- Document citation pills reference the uploaded document, without verified page-level pinpoints.
- Live AI output remains probabilistic and requires professional source review.

**Sources inspected:** `public/lr-chat-drawer.js`, `services/locke_research_service.js`, `services/research_engine.js`, `services/chat_answer_parts.js`, `services/citation_audit.js`, `services/legal_research.js`, `routes/research.js`, and November 12 handoff reports. Official comparator links and verification method are in [METHODOLOGY.md](METHODOLOGY.md).

[Full feature audit](FEATURE-MATRIX.md) · [Comparison](COMPARISON.md) · [Citation/sourcing boundaries](CITATION-AND-SOURCES.md) · [Original video demo](DEMO.md)