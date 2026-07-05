# Australian Standards Tracker — Baseline

Repo-backed memory for the Weekly Standards Watch routine. The routine reads this file at the start of each run, checks live status of every standard against the baseline column, flags anything newer, updates confirmed changes, and commits back to `main`. Do not store secrets here.

_Last updated: 2026-07-05_ | _Next scheduled run: 2026-07-12_

---

## HOW TO READ THIS TABLE
- **Current version (baseline)** = the version this routine last confirmed as current. When the routine confirms a newer version, it updates this column and bumps "Last confirmed".
- **Also track** = companion standards, parts, errata, or revision projects to check at the same time.
- **Status** = `current` | `revision-in-progress` | `superseded` (routine updates this).

---

## WIRING RULES & GENERAL INSTALLATION

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 3000** — Electrical installations (Wiring Rules) | 2018 ed. incl. Amd 1 (Jan 2020), Amd 2 (Apr 2021), Amd 3 (May 2023), Ruling 1 (May 2024) | 2026-07-05 | revision-in-progress | **Draft expected Q3 2026, new edition mid-2027** (project P-004717-01). No DR (draft-for-comment) released yet as of Jul 2026 — timeline unchanged. Watch for DR AS/NZS 3000 release. |
| **AS/NZS 3008.1.1** — Cable selection, LV (Australian conditions) | 2025 ed. | 2026-07-05 | current | **NEW 2025 EDITION** — supersedes 2017 ed. incl. Amd 1. Part 1.2 (NZ conditions) remains 2017 ed.; watch for its revision. |
| **AS/NZS 3008.1.2** — Cable selection, LV (NZ conditions) | 2017 ed. | 2026-07-05 | current | See 3008.1.1 above. |
| **AS/NZS 3017** — Verification by inspection and testing | 2022 ed. | 2026-07-05 | current | — |
| **AS/NZS 4836** — Safe working on/near LV and ELV electrical installations | 2023 ed. | 2026-07-05 | current | Superseded 2011 ed. Watch for amendments. |

---

## MINING & QUARRYING

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 3007** — Electrical equipment in mines and quarries (surface installations) | 2013 ed. | 2026-07-05 | current | Watch for a revision — 2013 ed. is over 10 years old. Supplements AS/NZS 3000, AS 2067, AS 60204. **Open question (unconfirmed):** some secondary sources suggest AS/NZS 5368:2025's scope may amalgamate 3007 as well as the 4871 series, conflicting with reseller listings still showing 3007 as "[Current]". Not corroborated against the official catalogue or the 5368 foreword — verify next run. |
| **AS/NZS 4871.1** — Electrical equipment for mines and quarries, general requirements | superseded 27 Jun 2025 by AS/NZS 5368:2025 | 2026-07-05 | superseded | AS/NZS 5368:2025 consolidates and redesignates AS/NZS 4871.1:2012 (and related parts). Track AS/NZS 5368:2025 going forward. |
| **AS/NZS 5368:2025** — Electrical equipment in mines and quarries | 2025 ed. (published 27 Jun 2025) | 2026-07-05 | current | **NEW STANDARD** — supersedes AS/NZS 4871.1:2012. Amalgamates multiple 4871-series parts. Sets design, installation, and operation requirements. No amendments found since publication. |
| **SA/SNZ HB 119** — Mines and quarries electrical protection (Handbook) | 2019 ed. | 2026-07-05 | current | Guidance companion to AS/NZS 3007, AS 2067, and AS/NZS 5368. |

---

## LV SWITCHBOARD & SWITCHGEAR

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 61439.1** — LV switchgear assemblies, general rules | 2026 ed. (supersedes 2016 ed.) | 2026-07-05 | current | **NEW 2026 EDITION** — review designs referencing 2016 ed. |
| **AS/NZS 61439.2** — Power switchgear and controlgear assemblies | 2026 ed. (published 13 Feb 2026) | 2026-07-05 | current | **NEW 2026 EDITION** — supersedes 2016 ed. Published alongside AS/NZS 61439.1:2026. Review designs referencing 2016 ed. |
| **AS/NZS 61439.3** — Distribution boards | 2016 ed. | 2026-07-05 | current | IEC 61439-3:2024 Ed.2 available in Standards Australia Store but no AS/NZS 61439.3:2026 found — circumstantial signal (Parts 1/2 just updated) but no draft located; watch for local adoption. Confirmed other parts: AS/NZS 61439.4:2016 (construction-site assemblies) and AS/NZS 61439.6:2016 (busbar trunking) also still 2016 ed., no 61439.5 adopted in AU/NZ. |
| **IEC 60947-1** — LV switchgear, general rules | 2020 ed. (6th ed.) | 2026-07-05 | current | **Revision signal (moderate confidence):** a CENELEC draft "prEN IEC 60947-1:2026" is circulating per standards.iteh.ai, suggesting a full IEC revision (beyond the previously-watched Amendment 1) may be in committee. Not yet a published IEC edition — pending official IEC catalogue confirmation. |
| **IEC 60947-2** — LV circuit-breakers | 2024 ed. (6th ed.) | 2026-07-05 | current | **NEW 2024 EDITION** — supersedes 2016 ed. incl. Amd 1 & 2. Used for Icc, Ics, selectivity. |
| **IEC 60947-4-1** — Contactors and motor starters | 2023 ed. (5th ed.) + COR1:2026 | 2026-07-05 | current | **COR1:2026 (Mar 2026)** — technical corrigendum to 5th ed. now incorporated in baseline. Used for Type 1/2 coordination; obtain updated (post-COR1) copy for design reference. |

---

## HV INSTALLATIONS & SUBSTATIONS

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS 2067** — Substations and HV installations exceeding 1 kV a.c. | 2016 ed. | 2026-07-05 | revision-in-progress | **DR AS 61936.1:2025** — public comment period closed 21 Apr 2026; still in post-comment finalisation as of Jul 2026, no publication date announced yet. Will replace AS 2067 when published. Also track IEC 61936-1 (parent, 2021 ed., unchanged). |
| **IEC 61936-1** — Power installations exceeding 1 kV a.c. | 2021 ed. (3rd ed.) | 2026-07-05 | current | Parent of AS 2067. Revision to this may trigger AS 2067 revision. |

---

## POWER SYSTEMS & SHORT-CIRCUIT

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEC 60909-0** — Short-circuit currents in three-phase AC systems | 2016 ed. | 2026-07-05 | current | **Revision signal (moderate confidence):** BSI standards-development tracker shows an active project "BS EN IEC 60909-0 Ed.3.0" (ref. 2021-00323, open since 2021) implying a 3rd IEC edition in development. Not yet reflected in the IEC Webstore catalogue (still 2016 ed.) — pending official IEC TC 73 confirmation. Also track IEC 60909-1 (factors), IEC 60909-3 (DC auxiliary systems). |
| **AS 60909-0** — Australian adoption of IEC 60909-0 | IEC 60909-0:2016 sold directly via Standards Australia Store; no separate AS-designated adoption found | 2026-07-05 | current | Australia appears to use IEC 60909-0:2016 directly. If IEC moves to a 3rd edition, check whether this direct-reference arrangement carries over. |
| **IEEE 519** — Harmonic control in electric power systems | 2022 ed. | 2026-07-05 | current | No active PAR or announced revision found. Watch for amendment. Revision cycle typically 5–10 years. |
| **AS/NZS 61000.3.6** — Limits for harmonic disturbances (MV/HV/EHV) | 2001 ed. (based on IEC 61000-3-6:1996) | 2026-07-05 | current | Part of the EMC series. No newer AS/NZS edition found. IEC parent has since moved to IEC TR 61000-3-6 Ed.2.0 (2008, a Technical Report) — long-standing edition gap, reconfirmed still present. |

---

## ARC FLASH

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEEE 1584** — Arc-flash hazard calculations | 2018 ed. (2nd ed.) | 2026-07-05 | current | No confirmed active PAR for a 3rd edition found. Track errata. |
| **IEEE 1584.1** — Arc-flash hazard scope/deliverables | 2022 ed. | 2026-07-05 | current | Companion to IEEE 1584-2018. |
| **IEEE 1584.2** — Arc-flash data collection | 2025 ed. | 2026-07-05 | current | Newest in the family (board approved 28 May 2025, published 19 Sep 2025). |

---

## PROTECTION & METERING

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEC 60255 series** — Measuring relays and protection equipment | Various parts 2010–2025 | 2026-07-05 | current | No new parts found since IEC TS 60255-216-1:2025. Core parts checked unchanged: 60255-1:2022, 60255-151:2009, 60255-187-1:2021+COR1:2023, 60255-26:2023. Source: https://webstore.iec.ch/en/publication/77735 |
| **AS 61850 series** — Communication networks and systems in substations | IEC 61850 adopted by Standards Australia; latest 2025 additions noted | 2026-07-05 | revision-in-progress | **Significant IEC-level restructuring in progress:** TC57 issued 7 CDV documents (Feb 2026) splitting the 61850-7-4 logical-node model into 61850-7-4 Ed.3 plus new parts 7-40, 7-43, 7-44, 7-400, 7-401, 7-440; comment period closed 10 Apr 2026, not yet published. Also a New Work Item Proposal for 61850-8-3 (RTI v2). New catalogue entries IEC TR 61850-1-1:2026 and IEC TR 61850-80-5:2026 noted (medium confidence, pending direct webstore confirmation). AS-side adoption unchanged — most recent AS designation is AS IEC 61850.4:2025, predates this baseline; no AU adoption yet of the 2025/2026 IEC additions. |

---

## SOLAR / INVERTER / BATTERY (for completeness — less core to your work but adjacent)

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 4777.1** — Grid connection of energy systems via inverters | 2024 ed. (effective Feb 2025) | 2026-07-05 | current | Mandatory since 23 Feb 2025 (compliance-date milestone, not a document change). No new amendment found. |
| **AS/NZS 4777.2** — Inverter requirements | 2020 ed. incl. Amd 2 (2024) | 2026-07-05 | current | Amd 2:2024 transition period ended 23 Aug 2025 (compliance-date milestone). No Amd 3 or new edition found. |

---

## STRUCTURAL (ADJACENT)

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS 4100** — Steel structures | 2020 ed. incl. Amd 1 (2021) and Amd 2 (2024) | 2026-07-05 | revision-in-progress | **Baseline correction:** previous baseline had missed the already-published Amendment 2:2024 (stricter NDT requirements, ISO 3834-3 workshop certification for higher construction categories). **Full re-write in progress:** the most wide-ranging revision since the standard's inception (advanced analysis provisions, new connection modelling, expanded fire engineering) went to public comment 7 Apr – 9 Jun 2026; not yet published as of this check — watch closely for the new edition. Structural standard adjacent to electrical scope (switchroom/substation structural steelwork). |

---

## TO ADD (rows to populate when you have confirmed editions)
| Standard | Description | Current version (baseline) | Last confirmed | Status |
|---|---|---|---|---|
| AS/NZS 3012 | Construction and demolition sites | — | — | — |
| AS/NZS 3001 | Transportable structures | — | — | — |

---

*Add more standards by inserting a row in the relevant section. Keep the designation exact (e.g. `AS/NZS 61439.1`, not `61439`) so the routine can search for it precisely.*
