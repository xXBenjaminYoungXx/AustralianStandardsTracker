# Australian Standards Tracker — Baseline

Repo-backed memory for the Weekly Standards Watch routine. The routine reads this file at the start of each run, checks live status of every standard against the baseline column, flags anything newer, updates confirmed changes, and commits back to `main`. Do not store secrets here.

_Last updated: 2026-08-16_ | _Next scheduled run: 2026-08-23_

---

## HOW TO READ THIS TABLE
- **Current version (baseline)** = the version this routine last confirmed as current. When the routine confirms a newer version, it updates this column and bumps "Last confirmed".
- **Also track** = companion standards, parts, errata, or revision projects to check at the same time.
- **Status** = `current` | `revision-in-progress` | `superseded` (routine updates this).

---

## WIRING RULES & GENERAL INSTALLATION

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 3000** — Electrical installations (Wiring Rules) | 2018 ed. incl. Amd 1 (Jan 2020), Amd 2 (Apr 2021), Amd 3 (May 2023), Ruling 1 (May 2024) | 2026-08-16 | revision-in-progress | **Draft expected Q3 2026, new edition mid-2027** (project P-004717-01). No DR (draft-for-comment) released yet as of 16 Aug 2026 — Q3 2026 window still open, timeline unchanged (reconfirmed). **Amendment date discrepancy resolved this run:** a stray search snippet suggested "Amd 3 (2025)"; confirmed via Standards Australia's own store SKU (`as-nzs-3000-2018-amd-3-2023`) that Amd 3 was published May 2023 as recorded — the "2025" figure is NZ's regulatory citation-update date (Electricity (Safety) Regulations, in force 13 Nov 2025), not a new amendment. No document change. Watch for DR AS/NZS 3000 release. |
| **AS/NZS 3008.1.1** — Cable selection, LV (Australian conditions) | 2025 ed. | 2026-08-16 | current | Supersedes 2017 ed. incl. Amd 1. No amendment found since. Mandatory-use date 19 Jun 2026 is an implementation deadline, not a revision. Part 1.2 (NZ conditions) remains 2017 ed.; watch for its revision. |
| **AS/NZS 3008.1.2** — Cable selection, LV (NZ conditions) | 2017 ed. | 2026-08-16 | current | **Reconfirmed unchanged this run** — a secondary source (GlobalSpec) incorrectly suggested a 2025 edition; directly checked store.standards.org.au search listings, which show only `as-nzs-3008-1-2-2017` and `as-nzs-3008-1-2-1998` product pages, no 2025 edition exists. Treat the "2025 edition" claim as a stale/incorrect secondary source. |
| **AS/NZS 3017** — Verification by inspection and testing | 2022 ed. | 2026-08-16 | current | — |
| **AS/NZS 4836** — Safe working on/near LV and ELV electrical installations | 2023 ed. | 2026-08-16 | current | Superseded 2011 ed. No amendments found. |

---

## MINING & QUARRYING

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 3007** — Electrical equipment in mines and quarries (surface installations) | superseded 27 Jun 2025 by AS/NZS 5368:2025 | 2026-08-16 | superseded | Reconfirmed unchanged (6th consecutive run of convergent secondary evidence). **Root cause of persistent fetch failure now identified:** the proxy status endpoint confirms direct WebFetch to standards.org.au/store.standards.org.au is blocked by an organisation-level egress policy denial (403 at the gateway, same denial hit control domains like wikipedia.org/google.com) — this is a standing infrastructure constraint, not a per-run fluke or site-specific block, and won't resolve via retries. Treat this classification as settled at moderate-high confidence via secondary sources; only escalate if the egress policy changes. |
| **AS/NZS 4871 series** — Electrical equipment for mines and quarries, general requirements (Parts 1–6) | superseded 27 Jun 2025 by AS/NZS 5368:2025 | 2026-08-16 | superseded | Reconfirmed unchanged, same evidentiary basis and egress-policy caveat as AS/NZS 3007 above. |
| **AS/NZS 5368:2025** — Electrical equipment in mines and quarries | 2025 ed. (published 27 Jun 2025) | 2026-08-16 | current | Supersedes AS/NZS 3007:2013 and the full AS/NZS 4871 series (Parts 1–6) per foreword — broader amalgamation than previously recorded. Sets design, installation, and operation requirements. No amendments found since publication. |
| **SA/SNZ HB 119** — Mines and quarries electrical protection (Handbook) | 2019 ed. | 2026-08-16 | revision-in-progress | **Reconfirmed unchanged (4th consecutive run):** HB 119:2019 remains associated with Standards New Zealand's "Aged Standards Proposed for Reconfirmation" consultation (committee EL-023), alongside AS/NZS 1972:2006 and AS/NZS 4641:2018. This run could not determine whether the consultation has closed with a published decision (reconfirm as-is / revise / withdraw) — search snippets only reproduce the committee's proposal-stage wording ("endorsed to be reconfirmed as they are valid, technically correct..."), and direct fetch to consultations.standards.govt.nz remains blocked. Treat as unresolved, not a confirmed change. Still guidance companion to AS/NZS 3007 (superseded), AS 2067, and AS/NZS 5368. |

---

## LV SWITCHBOARD & SWITCHGEAR

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 61439.1** — LV switchgear assemblies, general rules | 2026 ed. (supersedes 2016 ed.) | 2026-08-16 | current | Application date 2027-02-20. No amendments/errata found since publication. |
| **AS/NZS 61439.2** — Power switchgear and controlgear assemblies | 2026 ed. (published 13 Feb 2026) | 2026-08-16 | current | Application date 2027-02-13. Published alongside AS/NZS 61439.1:2026. No amendments/errata found. |
| **AS/NZS 61439.3** — Distribution boards | 2016 ed. | 2026-08-16 | current | Still no AS/NZS 61439.3:2026 found despite Parts 1/2 updating — reconfirmed unchanged; directly checked, only `as-nzs-61439-3-2016` product page exists, no 2026 SKU. Confirmed other parts: AS/NZS 61439.4:2016 (construction-site assemblies), AS/NZS 61439.5 (public networks), AS/NZS 61439.6:2016 (busbar trunking), AS/NZS 61439.7 (marina/camping) — none show 2026 updates. |
| **IEC 60947-1** — LV switchgear, general rules | 2020 ed. (6th ed.) + COR1:2022 + COR2:2024 | 2026-08-16 | current | **Priority check next run — still unresolved, now ~4 months post-CDV:** IEC project 121A/710/CDV (SC 121A), ED7 — CDV circulated 2026-01-23, voting closed 2026-04-17. No FDIS or new (7th) edition found yet; the current "IEC 60947:2026 SER" series pack still lists 60947-1 as the 2020 edition, confirming no supersession. A related prEN IEC 60947-1:2026 CENELEC draft (and a further prAA:2026 amendment-to-draft ballot) exists, consistent with post-CDV committee work but not proof of FDIS. Pending scope (not yet in force): smaller-conductor-size scope extension, new CoPI test, AWG sizing, reorganised tables/annexes. Still the standard in the tracker most likely to flip status soon — check webstore.iec.ch/en/publication/26973 and the SC121A dashboard directly each run until resolved. |
| **IEC 60947-2** — LV circuit-breakers | 2024 ed. (6th ed.) | 2026-08-16 | current | Supersedes 2016 ed. incl. Amd 1 & 2. No amendments/corrigenda found since. Used for Icc, Ics, selectivity. |
| **IEC 60947-4-1** — Contactors and motor starters | 2023 ed. (5th ed.) + COR1:2026 | 2026-08-16 | current | No further corrigenda/amendments found since COR1:2026. Used for Type 1/2 coordination; obtain updated (post-COR1) copy for design reference. Note: a COR1:2026 also exists for the *neighbouring* Part 4-2 (contactors for non-electric equipment) — do not confuse with this Part 4-1 corrigendum. |

---

## HV INSTALLATIONS & SUBSTATIONS

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS 2067** — Substations and HV installations exceeding 1 kV a.c. | 2016 ed. | 2026-08-16 | revision-in-progress | **DR AS 61936.1:2025** — public comment period closed 21 Apr 2026; still in post-comment finalisation as of 16 Aug 2026 (now ~4 months post-comment-close), no publication date, ballot outcome, or FDIS announced (reconfirmed, unchanged since last run — Standards Australia does not always publicise interim ballot stages, so absence of news isn't conclusive). Will replace AS 2067 when published. Also track IEC 61936-1 (parent, 2021 ed., unchanged). |
| **IEC 61936-1** — Power installations exceeding 1 kV a.c. | 2021 ed. (3rd ed.) | 2026-08-16 | current | Parent of AS 2067. No new IEC edition. Two adjacent-but-distinct items found, neither a new edition: a CENELEC regional national-annex doc (SIST EN IEC 61936-1:2021/A11:2026) and an IEC "Commented Version" companion product (explanatory comments alongside the 2021 3rd ed., not a revision). |

---

## POWER SYSTEMS & SHORT-CIRCUIT

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEC 60909-0** — Short-circuit currents in three-phase AC systems | 2026 ed. (3rd ed., published 23 Jul 2026) — supersedes 2016 ed. (2nd ed.) | 2026-08-16 | current | **NEW EDITION CONFIRMED THIS RUN:** IEC 60909-0:2026 (3rd ed.) published 23 Jul 2026, publication ID 68454 — the webstore record previously tracked as "Under development" now consistently returns with the published title format "IEC 60909-0:2026 \| IEC" and an explicit 23-Jul-2026 publication date across independent search results. A CENELEC parallel draft (prEN IEC 60909-0:2025) preceded it, consistent with a CDV/parallel-vote stage before publication. Moderate confidence — not yet independently verified via a direct primary-source page read (webstore.iec.ch fetch still blocked); no reseller/AU adoption yet reflects the 2026 ed. Also track IEC 60909-1 (factors), IEC 60909-3 (DC auxiliary systems). |
| **AS 60909-0** — Australian adoption of IEC 60909-0 | IEC 60909-0:2016 sold directly via Standards Australia Store; no separate AS-designated adoption found | 2026-08-16 | current | Reconfirmed on SA Store as the IEC publication itself; no AS/NZS-prefixed adoption exists. **IEC has now moved to a 3rd edition (IEC 60909-0:2026, see row above) — Standards Australia has not yet listed/adopted it (expected lag given publication was only ~3-4 weeks before this check). Check next run whether the AU store updates to the 2026 edition.** |
| **IEEE 519** — Harmonic control in electric power systems | 2022 ed. | 2026-08-16 | current | **Active revision project confirmed this run:** IEEE SA project P519 (revision of IEEE 519) is active/approved, reported target completion ~December 2028 (moderate confidence, from search-snippet summary of the SA project page, not directly fetched). Distinct from the separate P519.1 application guide project. Published 2022 edition remains current and in force; no near-term document change expected given the ~2028 target. |
| **AS/NZS 61000.3.6** — Limits for harmonic disturbances (MV/HV/EHV) | AS/NZS TR IEC 61000.3.6:2012 (based on IEC/TR 61000-3-6 Ed.2.0:2008) — supersedes AS/NZS 61000.3.6:2001 | 2026-08-16 | current | **Baseline correction reconfirmed (6th consecutive run of convergent evidence):** live current-product listings for TR IEC 61000.3.6:2012 exist on both the Standards Australia store and the Standards NZ shop, scope matching IEC/TR 61000-3-6 Ed.2.0:2008. Further corroborated this run: IEC's own current "IEC 61000-3:2026 SER" series bundle still includes IEC TR 61000-3-6:2008 as the constituent part, confirming no change at the international level either. Root cause of persistent direct-fetch failure remains a standing organisation-level egress policy denial (not site-specific). Treat as settled at moderate-high confidence. |

---

## ARC FLASH

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEEE 1584** — Arc-flash hazard calculations | 2018 ed. (2nd ed.) | 2026-08-16 | current | No confirmed active PAR for a 3rd edition found; no new working-group activity. Only known errata remains the 30-Aug-2019 sheet (predates baseline). |
| **IEEE 1584.1** — Arc-flash hazard scope/deliverables | 2022 ed. | 2026-08-16 | current | Companion to IEEE 1584-2018. No revision PAR found. |
| **IEEE 1584.2** — Arc-flash data collection | 2025 ed. | 2026-08-16 | current | Newest in the family (board approved 28 May 2025, published 19 Sep 2025). No further edition/errata activity found. |

---

## PROTECTION & METERING

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEC 60255 series** — Measuring relays and protection equipment | Various parts 2010–2025 | 2026-08-16 | current | No new parts found since IEC TS 60255-216-1:2025. Core parts reconfirmed unchanged: 60255-1:2022, 60255-151:2009, 60255-187-1:2021+COR1:2023, 60255-26:2023, 60255-27:2025 (Ed.3, product safety; national CENELEC implementation deadline 2026-04-30 is a transposition milestone, not a new edition). Only new items found are national CENELEC transpositions of existing editions (not new IEC-level revisions). Source: https://webstore.iec.ch/en/publication/77735 |
| **AS 61850 series** — Communication networks and systems in substations | IEC 61850 adopted by Standards Australia; latest 2025 additions noted | 2026-08-16 | revision-in-progress | **IEC-level restructuring progressing but still not published (reconfirmed):** the 61850-7-4 Ed.3 split (7-40, 7-43, 7-44, 7-400, 7-401, 7-440) remains at CDV stage — this run's research corroborates in more detail: IEC TC57/WG10 finalised the reorganisation package at a Seville meeting (week of 8 Feb 2026), producing seven CDV documents (57/2870–57/2876), comment period closed 2026-04-10, purely a document-restructuring exercise (no LN definition changes). No FDIS or publication found for any of the seven parts as of 16 Aug 2026. A related new document, IEC TR 61850-1-1:2026 (overview/scope TR, published Feb 2026, replacing the 2013-era TR), is separate from the split and doesn't indicate stage advancement. **61850-8-3 (RTI v2, WebSocket/JSON mapping):** still pre-Committee-Draft — NWIP-stage/Task Force specification work ongoing, no CD number or circulation date found. AS-side adoption: most recent AS designations remain AS IEC 61850.4:2025 and AS IEC 61850.6:2025 (published 19 Dec 2025) — no 2026 AS designation found. |

---

## SOLAR / INVERTER / BATTERY (for completeness — less core to your work but adjacent)

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 4777.1** — Grid connection of energy systems via inverters | 2024 ed. (effective Feb 2025) | 2026-08-16 | current | Mandatory since 23 Feb 2025 (compliance-date milestone, not a document change). No new amendment found. NZ's amended Electricity (Safety) Regulations cite this standard with a 12 Nov 2026 compliance date — a regulatory-citation deadline, not a document revision. |
| **AS/NZS 4777.2** — Inverter requirements | 2020 ed. incl. Amd 2 (2024) | 2026-08-16 | current | Amd 2:2024 transition period ended 23 Aug 2025 (compliance-date milestone). No Amd 3 or new edition found. |

---

## STRUCTURAL (ADJACENT)

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS 4100** — Steel structures | 2020 ed. incl. Amd 1 (2021) and Amd 2 (2024) | 2026-08-16 | revision-in-progress | **Full re-write (DR AS 4100:2026) still in progress, unchanged since last run:** public comment closed 9 Jun 2026 (now ~10 weeks ago); no publication date, ballot outcome, or timeline announced by Standards Australia or the Australian Steel Institute as of this check (searches targeting July/Aug 2026 news returned nothing new). Standards Australia's product page reportedly still flags AS 4100:2020 as "Pending Revision". Structural standard adjacent to electrical scope (switchroom/substation structural steelwork). Flagged as the standard most likely to have unreported/unannounced ballot movement — worth a direct store.standards.org.au check when egress allows. |

---

## TO ADD (rows to populate when you have confirmed editions)
| Standard | Description | Current version (baseline) | Last confirmed | Status |
|---|---|---|---|---|
| AS/NZS 3012 | Construction and demolition sites | — | — | — |
| AS/NZS 3001 | Transportable structures | — | — | — |

---

*Add more standards by inserting a row in the relevant section. Keep the designation exact (e.g. `AS/NZS 61439.1`, not `61439`) so the routine can search for it precisely.*
