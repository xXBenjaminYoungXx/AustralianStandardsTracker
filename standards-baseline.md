# Australian Standards Tracker — Baseline

Repo-backed memory for the Weekly Standards Watch routine. The routine reads this file at the start of each run, checks live status of every standard against the baseline column, flags anything newer, updates confirmed changes, and commits back to `main`. Do not store secrets here.

_Last updated: 2026-08-02_ | _Next scheduled run: 2026-08-09_

---

## HOW TO READ THIS TABLE
- **Current version (baseline)** = the version this routine last confirmed as current. When the routine confirms a newer version, it updates this column and bumps "Last confirmed".
- **Also track** = companion standards, parts, errata, or revision projects to check at the same time.
- **Status** = `current` | `revision-in-progress` | `superseded` (routine updates this).

---

## WIRING RULES & GENERAL INSTALLATION

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 3000** — Electrical installations (Wiring Rules) | 2018 ed. incl. Amd 1 (Jan 2020), Amd 2 (Apr 2021), Amd 3 (May 2023), Ruling 1 (May 2024) | 2026-08-02 | revision-in-progress | **Draft expected Q3 2026, new edition mid-2027** (project P-004717-01). No DR (draft-for-comment) released yet as of early Aug 2026 — Q3 2026 window still open, timeline unchanged (reconfirmed). Watch for DR AS/NZS 3000 release. |
| **AS/NZS 3008.1.1** — Cable selection, LV (Australian conditions) | 2025 ed. | 2026-08-02 | current | Supersedes 2017 ed. incl. Amd 1. No amendment found since. Part 1.2 (NZ conditions) remains 2017 ed.; watch for its revision. |
| **AS/NZS 3008.1.2** — Cable selection, LV (NZ conditions) | 2017 ed. | 2026-08-02 | current | See 3008.1.1 above. No revision signal found. |
| **AS/NZS 3017** — Verification by inspection and testing | 2022 ed. | 2026-08-02 | current | — |
| **AS/NZS 4836** — Safe working on/near LV and ELV electrical installations | 2023 ed. | 2026-08-02 | current | Superseded 2011 ed. No amendments found. |

---

## MINING & QUARRYING

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 3007** — Electrical equipment in mines and quarries (surface installations) | superseded 27 Jun 2025 by AS/NZS 5368:2025 | 2026-08-02 | superseded | Reconfirmed unchanged (4th consecutive run of convergent secondary evidence). **Root cause of persistent fetch failure now identified:** the proxy status endpoint confirms direct WebFetch to standards.org.au/store.standards.org.au is blocked by an organisation-level egress policy denial (403 at the gateway, same denial hit control domains like wikipedia.org/google.com) — this is a standing infrastructure constraint, not a per-run fluke or site-specific block, and won't resolve via retries. Treat this classification as settled at moderate-high confidence via secondary sources; only escalate if the egress policy changes. |
| **AS/NZS 4871 series** — Electrical equipment for mines and quarries, general requirements (Parts 1–6) | superseded 27 Jun 2025 by AS/NZS 5368:2025 | 2026-08-02 | superseded | Reconfirmed unchanged, same evidentiary basis and egress-policy caveat as AS/NZS 3007 above. |
| **AS/NZS 5368:2025** — Electrical equipment in mines and quarries | 2025 ed. (published 27 Jun 2025) | 2026-08-02 | current | Supersedes AS/NZS 3007:2013 and the full AS/NZS 4871 series (Parts 1–6) per foreword — broader amalgamation than previously recorded. Sets design, installation, and operation requirements. No amendments found since publication. |
| **SA/SNZ HB 119** — Mines and quarries electrical protection (Handbook) | 2019 ed. | 2026-08-02 | revision-in-progress | **Reconfirmed unchanged (2nd consecutive run):** HB 119:2019 remains listed on Standards New Zealand's "Aged Standards Proposed for Reconfirmation" consultation (committee EL-023), alongside AS/NZS 4641:2018 and AS/NZS 60079.35.1/.2. No decision (reconfirm as-is / revise / withdraw) has been published yet. Secondary/indexed evidence only (direct fetch to consultations.standards.govt.nz still blocked); confirm via primary source when access allows. Still guidance companion to AS/NZS 3007 (superseded), AS 2067, and AS/NZS 5368. |

---

## LV SWITCHBOARD & SWITCHGEAR

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 61439.1** — LV switchgear assemblies, general rules | 2026 ed. (supersedes 2016 ed.) | 2026-08-02 | current | Application date 2027-02-20. No amendments/errata found since publication. |
| **AS/NZS 61439.2** — Power switchgear and controlgear assemblies | 2026 ed. (published 13 Feb 2026) | 2026-08-02 | current | Application date 2027-02-13. Published alongside AS/NZS 61439.1:2026. No amendments/errata found. |
| **AS/NZS 61439.3** — Distribution boards | 2016 ed. | 2026-08-02 | current | Still no AS/NZS 61439.3:2026 found despite Parts 1/2 updating — reconfirmed unchanged. Confirmed other parts: AS/NZS 61439.4:2016 (construction-site assemblies), AS/NZS 61439.5 (public networks), AS/NZS 61439.6:2016 (busbar trunking), AS/NZS 61439.7 (marina/camping) — none show 2026 updates. |
| **IEC 60947-1** — LV switchgear, general rules | 2020 ed. (6th ed.) | 2026-08-02 | current | **Priority check next run — still unresolved, now over 3.5 months post-CDV:** IEC project 121A/710/CDV (SC 121A) — CDV circulated 2026-01-23, voting closed 2026-04-17. No FDIS or new (7th) edition found yet; Webstore still shows 2020 ed. as current. A related prEN IEC 60947-1:2026 CENELEC draft exists, consistent with post-CDV committee work but not proof of FDIS. Still the standard in the tracker most likely to flip status soon — check webstore.iec.ch/en/publication/26973 and the SC121A dashboard directly each run until resolved. |
| **IEC 60947-2** — LV circuit-breakers | 2024 ed. (6th ed.) | 2026-08-02 | current | Supersedes 2016 ed. incl. Amd 1 & 2. No amendments/corrigenda found since. Used for Icc, Ics, selectivity. |
| **IEC 60947-4-1** — Contactors and motor starters | 2023 ed. (5th ed.) + COR1:2026 | 2026-08-02 | current | No further corrigenda/amendments found since COR1:2026. Used for Type 1/2 coordination; obtain updated (post-COR1) copy for design reference. |

---

## HV INSTALLATIONS & SUBSTATIONS

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS 2067** — Substations and HV installations exceeding 1 kV a.c. | 2016 ed. | 2026-08-02 | revision-in-progress | **DR AS 61936.1:2025** — public comment period closed 21 Apr 2026; still in post-comment finalisation as of early Aug 2026 (now over 3.5 months post-comment-close), no publication date, ballot outcome, or FDIS announced (reconfirmed, unchanged since last run). Will replace AS 2067 when published. Also track IEC 61936-1 (parent, 2021 ed., unchanged — only a CENELEC-regional amendment EN IEC 61936-1:2021/A11:2025 found, not an IEC-level revision). |
| **IEC 61936-1** — Power installations exceeding 1 kV a.c. | 2021 ed. (3rd ed.) | 2026-08-02 | current | Parent of AS 2067. No new IEC edition; only a CENELEC regional national-annex doc (EN IEC 61936-1:2021/A11:2025-26) found, not an IEC-level revision. |

---

## POWER SYSTEMS & SHORT-CIRCUIT

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEC 60909-0** — Short-circuit currents in three-phase AC systems | 2016 ed. | 2026-08-02 | current | **Revision signal reconfirmed (moderate confidence):** BSI project 2021-00323 "BS EN IEC 60909-0 Ed.3.0" still listed as an open IEC TC 73 development project, no CDV/FDIS found yet. Not yet reflected in the IEC Webstore catalogue (still 2016 ed.). Also track IEC 60909-1 (factors), IEC 60909-3 (DC auxiliary systems). |
| **AS 60909-0** — Australian adoption of IEC 60909-0 | IEC 60909-0:2016 sold directly via Standards Australia Store; no separate AS-designated adoption found | 2026-08-02 | current | Reconfirmed on SA Store as the IEC publication itself; no AS/NZS-prefixed adoption exists. If IEC moves to a 3rd edition, check whether this direct-reference arrangement carries over. |
| **IEEE 519** — Harmonic control in electric power systems | 2022 ed. | 2026-08-02 | current | No active PAR found. IEEE SA Harmonics Working Group active but current visible work is the separate P519.1 application guide, not a 519 revision. |
| **AS/NZS 61000.3.6** — Limits for harmonic disturbances (MV/HV/EHV) | AS/NZS TR IEC 61000.3.6:2012 (based on IEC/TR 61000-3-6 Ed.2.0:2008) — supersedes AS/NZS 61000.3.6:2001 | 2026-08-02 | current | **Baseline correction reconfirmed (4th consecutive run of convergent evidence, still not primary-source-fetch-confirmed):** live current-product listings for TR IEC 61000.3.6:2012 exist on both the Standards Australia store and the Standards NZ shop, scope matching IEC/TR 61000-3-6 Ed.2.0:2008. The 26-06-2021 supersession date now has two independent indexed corroborations (up from one). **Root cause of persistent fetch failure identified:** confirmed via the proxy status endpoint to be an organisation-level egress policy denial (403 at the gateway, not site-specific — same denial hits unrelated control domains) — a standing infrastructure constraint that won't resolve via retries. Treat as settled at moderate confidence; only escalate if egress policy changes or an alternate access path becomes available. |

---

## ARC FLASH

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEEE 1584** — Arc-flash hazard calculations | 2018 ed. (2nd ed.) | 2026-08-02 | current | No confirmed active PAR for a 3rd edition found; no new working-group activity. Track errata. |
| **IEEE 1584.1** — Arc-flash hazard scope/deliverables | 2022 ed. | 2026-08-02 | current | Companion to IEEE 1584-2018. No revision PAR found. |
| **IEEE 1584.2** — Arc-flash data collection | 2025 ed. | 2026-08-02 | current | Newest in the family (board approved 28 May 2025, published 19 Sep 2025). No further edition/errata activity found. |

---

## PROTECTION & METERING

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEC 60255 series** — Measuring relays and protection equipment | Various parts 2010–2025 | 2026-08-02 | current | No new parts found since IEC TS 60255-216-1:2025. Core parts reconfirmed unchanged: 60255-1:2022, 60255-151:2009, 60255-187-1:2021+COR1:2023, 60255-26:2023. Only new items found are national CENELEC transpositions of existing editions (not new IEC-level revisions). Source: https://webstore.iec.ch/en/publication/77735 |
| **AS 61850 series** — Communication networks and systems in substations | IEC 61850 adopted by Standards Australia; latest 2025 additions noted | 2026-08-02 | revision-in-progress | **IEC-level restructuring progressing but still not published:** the 61850-7-4 Ed.3 split (7-40, 7-43, 7-44, 7-400, 7-401, 7-440) advanced to CDV stage — TC57/WG10 circulated seven CDV documents 2026-02-13, vote closed ~2026-05-08 — but no FDIS or publication found yet; the current IEC 61850 SER package still lists the legacy monolithic 61850-7-4:2010+AMD1:2020 as the active part. Re-check with priority next run for FDIS/publication. **61850-8-3 (RTI v2, WebSocket/JSON mapping):** NWIP 57/2866/NP confirmed approved (~Dec 2025); Task Force confirmed to have begun specification work in May 2026, no Committee Draft circulated yet — realistic CD timeline late 2026–2027, unconfirmed. AS-side adoption: most recent AS designations remain AS IEC 61850.4:2025 and AS IEC 61850.6:2025 (published 19 Dec 2025) — no 2026 AS designation found. |

---

## SOLAR / INVERTER / BATTERY (for completeness — less core to your work but adjacent)

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 4777.1** — Grid connection of energy systems via inverters | 2024 ed. (effective Feb 2025) | 2026-08-02 | current | Mandatory since 23 Feb 2025 (compliance-date milestone, not a document change). No new amendment found. |
| **AS/NZS 4777.2** — Inverter requirements | 2020 ed. incl. Amd 2 (2024) | 2026-08-02 | current | Amd 2:2024 transition period ended 23 Aug 2025 (compliance-date milestone). No Amd 3 or new edition found. |

---

## STRUCTURAL (ADJACENT)

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS 4100** — Steel structures | 2020 ed. incl. Amd 1 (2021) and Amd 2 (2024) | 2026-08-02 | revision-in-progress | **Full re-write (DR AS 4100:2026) still in progress, unchanged since last run:** public comment closed 9 Jun 2026 (now ~2 months ago); comment resolution/committee ballot would typically take several more months — no publication date, ballot outcome, or timeline announced by Standards Australia or the Australian Steel Institute as of this check. Structural standard adjacent to electrical scope (switchroom/substation structural steelwork). |

---

## TO ADD (rows to populate when you have confirmed editions)
| Standard | Description | Current version (baseline) | Last confirmed | Status |
|---|---|---|---|---|
| AS/NZS 3012 | Construction and demolition sites | — | — | — |
| AS/NZS 3001 | Transportable structures | — | — | — |

---

*Add more standards by inserting a row in the relevant section. Keep the designation exact (e.g. `AS/NZS 61439.1`, not `61439`) so the routine can search for it precisely.*
