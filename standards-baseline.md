# Australian Standards Tracker — Baseline

Repo-backed memory for the Weekly Standards Watch routine. The routine reads this file at the start of each run, checks live status of every standard against the baseline column, flags anything newer, updates confirmed changes, and commits back to `main`. Do not store secrets here.

_Last updated: 2026-10-04_ | _Next scheduled run: 2026-10-11_

---

## HOW TO READ THIS TABLE
- **Current version (baseline)** = the version this routine last confirmed as current. When the routine confirms a newer version, it updates this column and bumps "Last confirmed".
- **Also track** = companion standards, parts, errata, or revision projects to check at the same time.
- **Status** = `current` | `revision-in-progress` | `superseded` (routine updates this).

---

## WIRING RULES & GENERAL INSTALLATION

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 3000** — Electrical installations (Wiring Rules) | 2018 ed. incl. Amd 1 (Jan 2020), Amd 2 (Apr 2021), Amd 3 (May 2023), Ruling 1 (May 2024) | 2026-10-04 | revision-in-progress | **Draft expected Q3 2026, new edition mid-2027** (project P-004717-01). No DR (draft-for-comment) released yet as of 27 Sep 2026 — reconfirmed again this run (11th+ consecutive run) via industry secondary sources (ECA WA, cccengineering), still describing the Q3 2026 draft as a target/aim, not a completed release. Expected scope: EV charging, solar/battery integration, RCD updates, alignment with AS/NZS 3008:2025. Note: the Q3 2026 (Jul–Sep) window now closes within days (~30 Sep 2026) with still no DR sighted — either an imminent release or a slipped target. **2026-10-04 run:** window has now closed — search still shows only the "Q3 2026 draft / mid-2027 final" target, no DR sighted, so the Q3 target appears missed (unconfirmed; direct fetch to standards.org.au/flagship-projects/wiring-rules remained blocked (egress policy) this run too — priority direct check next run). |
| **AS/NZS 3008.1.1** — Cable selection, LV (Australian conditions) | 2025 ed. | 2026-10-04 | current | Supersedes 2017 ed. incl. Amd 1. No amendment found since (reconfirmed). Mandatory-use date 19 Jun 2026 is an implementation deadline, not a revision. Part 1.2 (NZ conditions) remains 2017 ed.; watch for its revision. |
| **AS/NZS 3008.1.2** — Cable selection, LV (NZ conditions) | 2017 ed. | 2026-10-04 | current | Reconfirmed unchanged again this run — explicitly checked for a "2025 edition" and found none; the 2025 update applies only to Part 1.1 (AU conditions), confirming the recurring false-positive/conflation pattern for this row. No real 2025 edition of Part 1.2 exists. |
| **AS/NZS 3017** — Verification by inspection and testing | 2022 ed. | 2026-10-04 | current | Reconfirmed unchanged. Cited unchanged in NZ's Electricity (Safety) Amendment Regulations 2025 (12-month transition to 12 Nov 2026) — a regulatory-citation matter, not a standard revision. |
| **AS/NZS 4836** — Safe working on/near LV and ELV electrical installations | 2023 ed. | 2026-10-04 | current | Superseded 2011 ed. No amendments found. Reconfirmed unchanged; also cited in NZ's 2025 electricity safety regulation amendments (compliance deadline 13 Nov 2026, regulatory-citation only). |

---

## MINING & QUARRYING

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 3007** — Electrical equipment in mines and quarries (surface installations) | superseded 27 Jun 2025 by AS/NZS 5368:2025 | 2026-10-04 | superseded | Reconfirmed unchanged (11th consecutive run of convergent secondary evidence). Standing egress-policy constraint on direct WebFetch to standards.org.au/store.standards.org.au remains settled — not re-flagged as new each run. |
| **AS/NZS 4871 series** — Electrical equipment for mines and quarries, general requirements (Parts 1–6) | superseded 27 Jun 2025 by AS/NZS 5368:2025 | 2026-10-04 | superseded | Reconfirmed unchanged, same evidentiary basis as AS/NZS 3007 above. |
| **AS/NZS 5368:2025** — Electrical equipment in mines and quarries | 2025 ed. (published 27 Jun 2025) | 2026-10-04 | current | Supersedes AS/NZS 3007:2013 and the full AS/NZS 4871 series (Parts 1–6) per foreword. Sets design, installation, and operation requirements. No amendments found since publication (reconfirmed). |
| **SA/SNZ HB 119** — Mines and quarries electrical protection (Handbook) | 2019 ed. | 2026-10-04 | revision-in-progress | **Still unresolved (9th consecutive run):** HB 119:2019 remains associated with Standards New Zealand's "Aged Standards Proposed for Reconfirmation" consultation (committee EL-023). This run located the specific consultation page — consultations.standards.govt.nz/draft-standards/copy-of-copy-of-aged-catalogue-el-041-reconfirmati/ ("Aged Standards - Electrical Equipment in Mines and Quarries (EL-023) Standards Proposed for Reconfirmation") — but direct fetch remained blocked (egress policy), so the outcome (reconfirm as-is / revise / withdraw) still could not be confirmed. No news/industry source has reported a closure. Treat as genuinely unresolved, not a confirmed change. Priority for next run: direct fetch of that specific URL. Still guidance companion to AS/NZS 3007 (superseded), AS 2067, and AS/NZS 5368. |

---

## LV SWITCHBOARD & SWITCHGEAR

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 61439.1** — LV switchgear assemblies, general rules | 2026 ed. (supersedes 2016 ed.) | 2026-10-04 | current | Application date 2027-02-20. No amendments/errata found since publication (reconfirmed). |
| **AS/NZS 61439.2** — Power switchgear and controlgear assemblies | 2026 ed. (published 13 Feb 2026) | 2026-10-04 | current | Application date 2027-02-13. Published alongside AS/NZS 61439.1:2026. No amendments/errata found (reconfirmed). |
| **AS/NZS 61439.3** — Distribution boards | 2016 ed. | 2026-10-04 | current | Still no AS/NZS 61439.3:2026 or draft found despite Parts 1/2 updating — reconfirmed unchanged. Note: Standards Australia's public-comment portal appears to have moved from the now-defunct sapc.standards.org.au to **comment.standards.org.au** — found via search this run, but direct fetch was blocked (egress policy), so an open Part 3 draft listing there could not be positively ruled in or out. Priority for next run: direct-check comment.standards.org.au for a Part 3 draft. Other parts: AS/NZS 61439.4:2016 (construction-site assemblies), AS/NZS 61439.5 (public networks), AS/NZS 61439.6:2016 (busbar trunking), AS/NZS 61439.7 (marina/camping) — none show 2026 updates. |
| **IEC 60947-1** — LV switchgear, general rules | 2020 ed. (6th ed.) + COR1:2022 + COR2:2024 | 2026-10-04 | revision-in-progress | **NEW 2026-10-04: ED7 has advanced past CDV — project at stage 40.99, "DIS approved for registration as FDIS" (24 Apr 2026); next stage FDIS decision (DECFDIS) target 16 Oct 2026 (source: genorma.com/en/standards/iec-60947-1-ed7, IEC project data). Publication of 7th edition plausible late 2026/early 2027. Previously:** IEC project 121A/710/CDV (SC 121A), ED7 — CDV circulated 2026-01-23, voting closed 2026-04-17, proposed stability date 2030. No FDIS or new (7th) edition found yet this run either; CENELEC's parallel prEN IEC 60947-1:2026 draft still shows pre-FDIS status — no evidence of advancement to FDIS/Enquiry. Pending scope (not yet in force): smaller-conductor-size scope extension, new CoPI test, AWG sizing, reorganised tables/annexes. Note: a separate CENELEC-only amendment track, EN IEC 60947-1:2021/prAA:2023, also exists — unrelated to the ED7 core revision, don't conflate. Still the standard in the tracker most likely to flip status soon — CDV→FDIS is now well overdue by typical timelines; check webstore.iec.ch/en/publication/26973 directly each run until resolved. |
| **IEC 60947-2** — LV circuit-breakers | 2024 ed. (6th ed.) | 2026-10-04 | current | Supersedes 2016 ed. incl. Amd 1 & 2. No amendments/corrigenda found since (reconfirmed). Used for Icc, Ics, selectivity. CENELEC adopted as EN IEC 60947-2:2025 (identical text, national implementation deadline 2026-02-28) — a regional adoption, not a new IEC edition. |
| **IEC 60947-4-1** — Contactors and motor starters | 2023 ed. (5th ed.) + COR1:2026 | 2026-10-04 | current | No further corrigenda/amendments found since COR1:2026 (reconfirmed). Used for Type 1/2 coordination; obtain updated (post-COR1) copy for design reference. Note: a COR1:2026 also exists for the *neighbouring* Part 4-2 (contactors for non-electric equipment) — do not confuse with this Part 4-1 corrigendum. |

---

## HV INSTALLATIONS & SUBSTATIONS

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS 2067** — Substations and HV installations exceeding 1 kV a.c. | 2016 ed. | 2026-10-04 | revision-in-progress | **DR AS 61936.1:2025** — public comment period closed 21 Apr 2026; still in post-comment finalisation as of 27 Sep 2026 (now over 5 months post-comment-close), no publication date, ballot outcome, or FDIS announced (reconfirmed, unchanged since last run — no reseller/tracking site has picked up a new AS 61936.1 designation yet). Will replace AS 2067 when published. Also track IEC 61936-1 (parent, 2021 ed., unchanged). |
| **IEC 61936-1** — Power installations exceeding 1 kV a.c. | 2021 ed. (3rd ed.) | 2026-10-04 | current | Parent of AS 2067. No new IEC edition (reconfirmed). A CENELEC-only regional amendment (EN IEC 61936-1:2021/A11:2025, with a further regional SIST adoption in 2026) exists but is a European EN-adoption amendment, not an IEC-level revision — does not change this row's status. |

---

## POWER SYSTEMS & SHORT-CIRCUIT

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEC 60909-0** — Short-circuit currents in three-phase AC systems | 2026 ed. (3rd ed., published 23 Jul 2026) — supersedes 2016 ed. (2nd ed.) | 2026-10-04 | current | Reconfirmed unchanged. No corrigendum/errata found against the 2026 3rd edition. Also track IEC 60909-1 (factors), IEC 60909-3 (DC auxiliary systems). |
| **AS 60909-0** — Australian adoption of IEC 60909-0 | IEC 60909-0:2016 sold directly via Standards Australia Store; no separate AS-designated adoption found | 2026-10-04 | current | Reconfirmed unchanged again this run — SA Store search results still show only `iec-60909-0-2016`, no 2026 SKU found, in contrast to other IEC 2026 editions (e.g. AS/NZS 62368.1:2026) that clearly have been added — a real lag, not a broken feed. Check next run whether the AU store updates to the 2026 edition. |
| **IEEE 519** — Harmonic control in electric power systems | 2022 ed. | 2026-10-04 | current | Active revision project P519 reconfirmed this run (PES Harmonics Working Group), still no confirmed change to the ~December 2028 target. Canonical project URL reconfirmed again at standards.ieee.org/ieee/519/11811/. Published 2022 edition remains current and in force; no near-term document change expected. |
| **AS/NZS 61000.3.6** — Limits for harmonic disturbances (MV/HV/EHV) | AS/NZS TR IEC 61000.3.6:2012 (based on IEC/TR 61000-3-6 Ed.2.0:2008) — supersedes AS/NZS 61000.3.6:2001 | 2026-10-04 | current | Reconfirmed unchanged (10th consecutive run of convergent evidence). No project/draft activity found at either the AU/NZ or IEC level. Root cause of persistent direct-fetch failure remains a standing organisation-level egress policy denial (not site-specific, settled). |

---

## ARC FLASH

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEEE 1584** — Arc-flash hazard calculations | 2018 ed. (2nd ed.) | 2026-10-04 | revision-in-progress | **Confirmed 2026-10-04 (confidence now high):** IEEE SA project page shows P1584 as Active PAR, PAR approved 2025-05-28, supersedes IEEE 1584-2018, committee IAS/PCI, WG chair Daleep Mohla, PM Michael Kipness (standards.ieee.org/ieee/1584/12061/ via search index). Prior notes: the P1584 revision project (tracked via .../ieee/1584/12061/) persists in search-index results, but this run confirmed the egress block against standards.ieee.org and sagroups.ieee.org is domain-wide (all paths refused, not just this specific page) — and web.archive.org is now also unreachable from this network, closing off the archived-copy workaround too. No PAR number, scope, or target date obtained. Published 2018 2nd edition remains current and in force either way; no document change. **P1584.11:** still at PAR-under-consideration stage, unchanged watch item (not yet a tracked row). Priority for next run unchanged: a direct primary-source fetch (or IEEE SA myProject access) would resolve this — flag to a maintainer that this network's egress policy, not IEEE's access controls, is the limiting factor. |
| **IEEE 1584.1** — Arc-flash hazard scope/deliverables | 2022 ed. | 2026-10-04 | current | Companion to IEEE 1584-2018. No revision PAR found (reconfirmed). |
| **IEEE 1584.2** — Arc-flash data collection | 2025 ed. | 2026-10-04 | current | Newest in the family (project #11030, board approved 28 May 2025, published 19 Sep 2025). No further edition/errata activity found (reconfirmed). |

---

## PROTECTION & METERING

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEC 60255 series** — Measuring relays and protection equipment | Various parts 2010–2025 | 2026-10-04 | current | No new parts found since IEC TS 60255-216-1:2025 (reconfirmed). Core parts reconfirmed unchanged: 60255-1:2022, 60255-151:2009, 60255-187-1:2021+COR1:2023, 60255-26:2023, 60255-27:2025 (Ed.3, product safety; national CENELEC implementation deadline 2026-04-30 is a transposition milestone, not a new edition). Note: CENELEC/BSI/DIN listings showing regional-endorsement dates (e.g. "DIN EN IEC 60255-27 - 2026-04") are adoptions of the same existing IEC text, not new IEC editions. Source: https://webstore.iec.ch/en/publication/77735 |
| **AS 61850 series** — Communication networks and systems in substations | IEC 61850 adopted by Standards Australia; latest 2025 additions noted | 2026-10-04 | revision-in-progress | **IEC-level restructuring progressing but still not published:** the 61850-7-4 Ed.3 split (7-40, 7-43, 7-44, 7-400, 7-401, 7-440) — CDV comment period closed 2026-04-10, and per this run's project-card snippets the CDV vote itself closed 8 May 2026, now sitting at IEC stage 40.60 ("close of voting / results established" — forwarded to committee). This is incremental progress (post-CDV) but none of the seven parts have reached FDIS or appear in the current IEC 61850 SER package yet — still pre-publication. **61850-8-3 (RTI v2):** still pre-CD (NWIP approved ~Mar 2026, task force drafting since May 2026), consistent with baseline. **New 61850-family publications (reconfirmed, no AS adoption yet):** IEC 61850-7-410:2026 and IEC TR 61850-80-5:2026. AS-side adoption: most recent AS designations remain AS IEC 61850.4:2025 and AS IEC 61850.6:2025 (published 19 Dec 2025) — no 2026 AS designation found for any of the above yet. |

---

## SOLAR / INVERTER / BATTERY (for completeness — less core to your work but adjacent)

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 4777.1** — Grid connection of energy systems via inverters | 2024 ed. (effective Feb 2025) | 2026-10-04 | current | Mandatory since 23 Feb 2025 (compliance-date milestone, not a document change). No new amendment found (reconfirmed). NZ's amended Electricity (Safety) Regulations cite this standard with a 12 Nov 2026 compliance date — a regulatory-citation deadline, not a document revision. |
| **AS/NZS 4777.2** — Inverter requirements | 2020 ed. incl. Amd 2 (2024) | 2026-10-04 | current | Amd 2:2024 transition period ended 23 Aug 2025 (compliance-date milestone). No Amd 3 or new edition found (reconfirmed). |

---

## STRUCTURAL (ADJACENT)

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS 4100** — Steel structures | 2020 ed. incl. Amd 1 (2021) and Amd 2 (2024) | 2026-10-04 | revision-in-progress | **Full re-write (DR AS 4100:2026) still in progress, unchanged since last run:** public comment ran 7 Apr – 9 Jun 2026 (now ~16 weeks post-close); no publication date, ballot outcome, or timeline announced by Standards Australia or the Australian Steel Institute as of this check. Structural standard adjacent to electrical scope (switchroom/substation structural steelwork). Flagged as the standard most likely to have unreported/unannounced ballot movement — worth a direct store.standards.org.au / steel.org.au check when egress allows. |

---

## TO ADD (rows to populate when you have confirmed editions)
| Standard | Description | Current version (baseline) | Last confirmed | Status |
|---|---|---|---|---|
| AS/NZS 3012 | Construction and demolition sites | — | — | — |
| AS/NZS 3001 | Transportable structures | — | — | — |

---

*Add more standards by inserting a row in the relevant section. Keep the designation exact (e.g. `AS/NZS 61439.1`, not `61439`) so the routine can search for it precisely.*
