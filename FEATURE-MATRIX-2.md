# Locke Research Companion — Feature-by-Feature Matrix (Part 2)

**Companion to [Part 1](FEATURE-MATRIX.md).** Source snapshot `a05e53d886fd` (November 12, 2026). Comparisons are based on official vendor offerings and do not imply exact parity or absence.

Key: **L** Lexis+ with Protégé; **C** CoCounsel Legal; **V** vLex Vincent; **B** Bloomberg Law; **P** Paxton. `●` broadly comparable published category; `≈` related capability; `?` exact counterpart not verified. Each Locke row is source-inspected, not separately rerun against live production.

## Chronology and timeline (16)

**Evidence:** `services/locke_research_companion.js`, `routes/research_companion.js`.

| # | Individual feature | Locke status | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 176 | List timeline events | Source-implemented | ● | ● | ● | ● | ● |
| 177 | Create manual event | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 178 | Edit event date | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 179 | Edit event time | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 180 | Edit event description | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 181 | Delete event | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 182 | Record event source type | Source-implemented | ● | ● | ● | ● | ● |
| 183 | Record event confidence | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 184 | Mark event verification | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 185 | Extract candidate dates from document | Source-implemented | ● | ● | ● | ● | ● |
| 186 | Review candidate timeline events | Source-implemented | ● | ● | ● | ● | ● |
| 187 | Add selected proposed events | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 188 | Compare chronology across documents | Source-implemented | ● | ● | ● | ● | ● |
| 189 | Connect event to source document IDs | Source-implemented | ● | ● | ● | ● | ● |
| 190 | Flag conflicting dates | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 191 | Require correct case ownership on mutation | Source-implemented | ● | ● | ● | ● | ● |

## Issues and facts (21)

**Evidence:** `services/locke_research_companion.js`, `routes/research_companion.js`.

| # | Individual feature | Locke status | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 192 | Create issue | Source-implemented | ● | ● | ● | ● | ● |
| 193 | List case issues | Source-implemented | ● | ● | ● | ● | ● |
| 194 | Open issue detail | Source-implemented | ● | ● | ● | ● | ● |
| 195 | Edit issue title | Source-implemented | ● | ● | ● | ● | ● |
| 196 | Edit issue description | Source-implemented | ● | ● | ● | ● | ● |
| 197 | Set issue priority | Source-implemented | ● | ● | ● | ● | ● |
| 198 | Set issue status | Source-implemented | ● | ● | ● | ● | ● |
| 199 | Delete issue | Source-implemented | ● | ● | ● | ● | ● |
| 200 | Extract suggested issues from uploaded document | Source-implemented | ● | ● | ● | ● | ● |
| 201 | Create fact | Source-implemented | ● | ● | ● | ● | ● |
| 202 | List facts by case | Source-implemented | ● | ● | ● | ● | ● |
| 203 | Filter facts by issue | Source-implemented | ● | ● | ● | ● | ● |
| 204 | Update fact text | Source-implemented | ● | ● | ● | ● | ● |
| 205 | Set fact verified status | Source-implemented | ● | ● | ● | ● | ● |
| 206 | Store fact confidence | Source-implemented | ● | ● | ● | ● | ● |
| 207 | Store fact source text | Source-implemented | ● | ● | ● | ● | ● |
| 208 | Link fact to issue | Source-implemented | ● | ● | ● | ● | ● |
| 209 | Delete fact | Source-implemented | ● | ● | ● | ● | ● |
| 210 | Extract suggested facts from document | Source-implemented | ● | ● | ● | ● | ● |
| 211 | Validate issue/fact status values | Source-implemented | ● | ● | ● | ● | ● |
| 212 | Restrict cross-tenant issue and fact updates | Source-implemented | ? | ? | ? | ? | ? |

## Evidence board and case context (11)

**Evidence:** `ui-preview/src/pages/EvidenceBoardPage.tsx`, `ui-preview/src/services/routeWorkflow.ts`, `services/locke_research_companion.js`.

| # | Individual feature | Locke status | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 213 | Render evidence board page | Source-implemented | ● | ● | ● | ● | ● |
| 214 | Display case-linked documents | Source-implemented | ● | ● | ● | ● | ● |
| 215 | Display facts alongside issues | Source-implemented | ● | ● | ● | ● | ● |
| 216 | Expose source-linked records | Source-implemented | ● | ● | ● | ● | ● |
| 217 | Show items requiring verification | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 218 | Use documentary excerpts in synthesis | Source-implemented | ● | ● | ● | ● | ● |
| 219 | Navigate evidence to file | Source-implemented | ● | ● | ● | ● | ● |
| 220 | Recognize missing evidence | Source-implemented | ● | ● | ● | ● | ● |
| 221 | Keep evidence within selected case | Source-implemented | ● | ● | ● | ● | ● |
| 222 | Show source document for a timeline event | Source-implemented | ● | ● | ● | ● | ● |
| 223 | Avoid treating prior AI output as source evidence | Source-implemented | ● | ● | ● | ● | ● |

## Attorney preparation and case packets (15)

**Evidence:** `services/locke_research_companion.js`, `routes/research_companion.js`.

| # | Individual feature | Locke status | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 224 | Generate attorney-preparation packet | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 225 | Collect case chronology | Source-implemented | ● | ● | ● | ● | ● |
| 226 | Collect issues and facts | Source-implemented | ● | ● | ● | ● | ● |
| 227 | Include relevant case documents | Source-implemented | ● | ● | ● | ● | ● |
| 228 | Develop questions for counsel | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 229 | List saved attorney packets | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 230 | Open a saved attorney packet | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 231 | Associate packet to selected case | Source-implemented | ? | ? | ? | ? | ? |
| 232 | Generate deep whole-case review | Source-implemented | ● | ● | ● | ● | ● |
| 233 | Generate multi-document review | Source-implemented | ● | ● | ● | ● | ● |
| 234 | Build multi-document chronology | Source-implemented | ● | ● | ● | ● | ● |
| 235 | Generate full case packet | Source-implemented | ● | ● | ● | ● | ● |
| 236 | Build packet appendix | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 237 | Identify unreadable source documents | Source-implemented | ● | ● | ● | ● | ● |
| 238 | Record source context in work product | Source-implemented | ● | ● | ● | ● | ● |

## Reports and exports (21)

**Evidence:** `services/locke_research_companion.js`, `services/research_export_formats.js`, `routes/research_export.js`.

| # | Individual feature | Locke status | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 239 | Create case report | Source-implemented | ● | ● | ● | ● | ● |
| 240 | List case reports | Source-implemented | ● | ● | ● | ● | ● |
| 241 | Retrieve report by ID | Source-implemented | ● | ● | ● | ● | ● |
| 242 | Export case report | Source; conditional | ● | ● | ● | ● | ● |
| 243 | Build research PDF | Source-implemented | ● | ● | ● | ● | ● |
| 244 | Build research DOCX | Source-implemented | ● | ● | ● | ● | ● |
| 245 | Export saved research record | Source; conditional | ● | ● | ● | ● | ● |
| 246 | Export bounded ad-hoc text | Source; conditional | ? | ? | ? | ? | ? |
| 247 | Add jurisdiction header to export | Source; conditional | ● | ● | ● | ● | ● |
| 248 | Include legal source list | Source-implemented | ● | ● | ● | ● | ● |
| 249 | Include citations and warnings | Source-implemented | ? | ? | ? | ? | ? |
| 250 | Include uncited source appendix | Source-implemented | ? | ? | ? | ? | ? |
| 251 | Report research verification notes | Source-implemented | ● | ● | ● | ● | ● |
| 252 | Bound export text size | Source; conditional | ? | ? | ? | ? | ? |
| 253 | Preflight export quota | Source; conditional | ● | ● | ● | ● | ● |
| 254 | Atomic export usage charge | Source; conditional | ? | ? | ? | ? | ? |
| 255 | Idempotent export request | Source; conditional | ● | ● | ● | ● | ● |
| 256 | Check retry input fingerprint | Source-implemented | ? | ? | ? | ? | ? |
| 257 | Prevent cross-tenant export access | Source; conditional | ? | ? | ? | ? | ? |
| 258 | Retain export history | Source; conditional | ● | ● | ● | ● | ● |
| 259 | No independently validated legal certification (not implemented) | Not established / not shipped | ? | ? | ? | ? | ? |

## History, conversations and continuity (15)

**Evidence:** `services/locke_research_service.js`, `routes/research.js`.

| # | Individual feature | Locke status | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 260 | Save research question | Source-implemented | ● | ● | ● | ● | ● |
| 261 | Save generated answer | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 262 | Save provider/model metadata | Source; conditional | ? | ? | ? | ? | ? |
| 263 | Save cited sources | Source-implemented | ? | ? | ? | ? | ? |
| 264 | Save token counts | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 265 | Group messages into conversation threads | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 266 | List past conversations | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 267 | Read conversation transcript | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 268 | Resume prior thread | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 269 | Bound restored transcript by tenant | Source-implemented | ? | ? | ? | ? | ? |
| 270 | List all research runs | Source-implemented | ● | ● | ● | ● | ● |
| 271 | Filter history by case | Source-implemented | ● | ● | ● | ● | ● |
| 272 | Hide or delete history item | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 273 | Maintain connection between research and evidence | Source-implemented | ● | ● | ● | ● | ● |
| 274 | Open previous work from history | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |

## AI provider and streaming infrastructure (19)

**Evidence:** `services/research_llm.js`, `services/model_router.js`, `services/llm_stream.js`, `services/locke_research_routing.js`.

| # | Individual feature | Locke status | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 275 | Route AI model by task | Source; conditional | ● | ● | ● | ● | ● |
| 276 | Quick-mode model lane | Source; conditional | ≈ | ≈ | ≈ | ≈ | ≈ |
| 277 | Deep research model lane | Source; conditional | ● | ● | ● | ● | ● |
| 278 | Whole-case deeper model lane | Source; conditional | ● | ● | ● | ● | ● |
| 279 | Keep raw provider model choices internal | Source; conditional | ? | ? | ? | ? | ? |
| 280 | OpenAI model connector | Source; conditional | ● | ● | ● | ● | ● |
| 281 | OpenRouter model connector | Source; conditional | ≈ | ≈ | ≈ | ≈ | ≈ |
| 282 | Provider failover before disclosure | Source; conditional | ? | ? | ? | ? | ? |
| 283 | Timeout outbound AI requests | Source-implemented | ? | ? | ? | ? | ? |
| 284 | Bound provider response tokens | Source; conditional | ? | ? | ? | ? | ? |
| 285 | Estimate request cost | Source-implemented | ? | ? | ? | ? | ? |
| 286 | Conservative cost on unknown model | Source; conditional | ? | ? | ? | ? | ? |
| 287 | Record actual provider usage | Source; conditional | ? | ? | ? | ? | ? |
| 288 | Track model and provider provenance | Source; conditional | ? | ? | ? | ? | ? |
| 289 | Handle provider failure safely | Source; conditional | ? | ? | ? | ? | ? |
| 290 | Stream permitted Quick text | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 291 | Account for partial stream failure | Source-implemented | ● | ● | ● | ● | ● |
| 292 | Reject unsupported provider configuration | Source; conditional | ? | ? | ? | ? | ? |
| 293 | Avoid silent fallback after partial streamed output | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |

## Usage entitlements and accounting (19)

**Evidence:** `services/locke_research_guard.js`, `services/usage_ledger.js`, `services/locke_research_catalog.js`.

| # | Individual feature | Locke status | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 294 | Check research entitlement | Source-implemented | ● | ● | ● | ● | ● |
| 295 | Use one active research plan | Source-implemented | ● | ● | ● | ● | ● |
| 296 | Classify standard action | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 297 | Classify premium action | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 298 | Classify OCR page action | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 299 | Classify document page action | Source-implemented | ● | ● | ● | ● | ● |
| 300 | Classify export action | Source; conditional | ● | ● | ● | ● | ● |
| 301 | Preflight usage limit | Source-implemented | ? | ? | ? | ? | ? |
| 302 | Reserve usage transactionally | Source-implemented | ? | ? | ? | ? | ? |
| 303 | Record usage events | Source-implemented | ? | ? | ? | ? | ? |
| 304 | Reconcile actual usage | Source-implemented | ? | ? | ? | ? | ? |
| 305 | Report monthly usage | Source-implemented | ? | ? | ? | ? | ? |
| 306 | Report daily usage | Source-implemented | ? | ? | ? | ? | ? |
| 307 | Report OCR consumption | Source-implemented | ● | ● | ● | ● | ● |
| 308 | Report export consumption | Source; conditional | ● | ● | ● | ● | ● |
| 309 | Apply hosting file-size safety limits | Source-implemented | ? | ? | ? | ? | ? |
| 310 | Reject unavailable premium action | Source-implemented | ● | ● | ● | ● | ● |
| 311 | Avoid accounting bypass via alternate path | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 312 | No final public subscription price (not configured) | Not established / not shipped | ? | ? | ? | ? | ? |

## Authentication and firm isolation (20)

**Evidence:** `routes/auth.js`, `middleware/auth.js`, `services/login_attempt_limiter.js`.

| # | Individual feature | Locke status | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 313 | Register authorized account | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 314 | Password hashing | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 315 | Sign in | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 316 | Issue JWT access credential | Source-implemented | ? | ? | ? | ? | ? |
| 317 | Refresh session | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 318 | Rotate refresh credential | Source-implemented | ? | ? | ? | ? | ? |
| 319 | Sign out | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 320 | Read authenticated user profile | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 321 | Protect research endpoints with auth | Source-implemented | ● | ● | ● | ● | ● |
| 322 | Validate user scope | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 323 | Validate firm scope | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 324 | Limit login attempts per IP | Source-implemented | ? | ? | ? | ? | ? |
| 325 | Limit repeat failures per account | Source-implemented | ? | ? | ? | ? | ? |
| 326 | Use generic error on bad login | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 327 | Reduce account-enumeration timing clues | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 328 | Reject cross-tenant document access | Source-implemented | ? | ? | ? | ? | ? |
| 329 | Reject cross-tenant timeline mutation | Source-implemented | ? | ? | ? | ? | ? |
| 330 | Restrict archived-case edits | Source-implemented | ● | ● | ● | ● | ● |
| 331 | Refuse local test auth in production | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 332 | Cap default JSON request body | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |

## Administration, audit, release safeguards (21)

**Evidence:** `routes/admin.js`, `routes/administration.js`, `services/administration_service.js`, `services/release_readiness.js`.

| # | Individual feature | Locke status | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 333 | Admin overview | Source-implemented | ? | ? | ? | ? | ? |
| 334 | Search admin-visible users | Source-implemented | ? | ? | ? | ? | ? |
| 335 | Reauthenticate before sensitive action | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 336 | Revoke another user's sessions | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 337 | View operational work | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 338 | Retry pending document purges | Source-implemented | ● | ● | ● | ● | ● |
| 339 | View administrative audit log | Source-implemented | ? | ? | ? | ? | ? |
| 340 | Filter audit events | Source-implemented | ? | ? | ? | ? | ? |
| 341 | Export audit CSV | Source; conditional | ? | ? | ? | ? | ? |
| 342 | Track admin action context | Source-implemented | ? | ? | ? | ? | ? |
| 343 | Enforce admin permissions | Source-implemented | ? | ? | ? | ? | ? |
| 344 | Check admin recency proof | Source-implemented | ? | ? | ? | ? | ? |
| 345 | Generate usage report | Source-implemented | ? | ? | ? | ? | ? |
| 346 | Service health endpoint | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 347 | Sanitize 500 error responses | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 348 | Validate production configuration | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 349 | Refuse mock mode in production | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 350 | Require provider for legal research | Source; conditional | ? | ? | ? | ? | ? |
| 351 | CI with PostgreSQL service | Source-implemented | ? | ? | ? | ? | ? |
| 352 | Source-backed answer withholding regression | Source-implemented | ● | ● | ● | ● | ● |
| 353 | No external penetration certification supplied (not verified) | Not established / not shipped | ? | ? | ? | ? | ? |

## Public website and operator experience (28)

**Evidence:** `services/public_pages.js`, `ui-preview/src/app/ProfessionalShell.tsx`, `ui-preview/src/app/navigation.ts`.

| # | Individual feature | Locke status | L | C | V | B | P |
|---:|---|---|:-:|:-:|:-:|:-:|:-:|
| 354 | Homepage with product explanation | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 355 | Methodology page | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 356 | Trust explanation | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 357 | Source-backed explainer | Source-implemented | ● | ● | ● | ● | ● |
| 358 | Jurisdiction index | Source-implemented | ● | ● | ● | ● | ● |
| 359 | State and federal jurisdiction hubs | Source-implemented | ● | ● | ● | ● | ● |
| 360 | Court hierarchy public pages | Source-implemented | ● | ● | ● | ● | ● |
| 361 | Sitemap | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 362 | Robots crawler rules | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 363 | Canonical site URL metadata | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 364 | Accessible product navigation | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 365 | Case dashboard view | Source-implemented | ● | ● | ● | ● | ● |
| 366 | Documents view | Source-implemented | ● | ● | ● | ● | ● |
| 367 | Evidence board view | Source-implemented | ● | ● | ● | ● | ● |
| 368 | Issues and facts view | Source-implemented | ● | ● | ● | ● | ● |
| 369 | Attorney preparation view | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 370 | Research view | Source-implemented | ● | ● | ● | ● | ● |
| 371 | Timeline view | Source-implemented | ● | ● | ● | ● | ● |
| 372 | Reports view | Source-implemented | ● | ● | ● | ● | ● |
| 373 | Exports view | Source; conditional | ● | ● | ● | ● | ● |
| 374 | History view | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 375 | Usage view | Source-implemented | ? | ? | ? | ? | ? |
| 376 | Settings view | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 377 | Administration view | Source-implemented | ? | ? | ? | ? | ? |
| 378 | Light/dark theme | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 379 | Responsive navigation | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 380 | Authentication redirect | Source-implemented | ≈ | ≈ | ≈ | ≈ | ≈ |
| 381 | Official demo video embedded | Source-implemented | ? | ? | ? | ? | ? |

## Audit total

**381 individually itemized capabilities** across Parts 1 and 2. 8 source route files are traced separately in [ROUTE-TRACE.md](ROUTE-TRACE.md). Features explicitly marked not shipped, not configured or not independently verified are **not advertised as complete**.

[Competitive interpretation](COMPARISON.md) · [Ask Locke deep dive](ASK-LOCKE.md) · [Citation audit limits](CITATION-AND-SOURCES.md).