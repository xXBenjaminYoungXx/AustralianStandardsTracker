# Australian Standards Tracker — Baseline

Repo-backed memory for the Weekly Standards Watch routine. The routine reads this file at the start of each run, checks live status of every standard against the baseline column, flags anything newer, updates confirmed changes, and commits back to `main`. Do not store secrets here.

_Last updated: 2026-06-22_

---

## HOW TO READ THIS TABLE
- **Current version (baseline)** = the version this routine last confirmed as current. When the routine confirms a newer version, it updates this column and bumps "Last confirmed".
- **Also track** = companion standards, parts, errata, or revision projects to check at the same time.
- **Status** = `current` | `revision-in-progress` | `superseded` (routine updates this).

---

## WIRING RULES & GENERAL INSTALLATION

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 3000** — Electrical installations (Wiring Rules) | 2018 ed. incl. Amd 1 (Jan 2020), Amd 2 (Apr 2021), Amd 3 (May 2023), Ruling 1 (May 2024) | 2026-06-22 | revision-in-progress | **Draft expected Q3 2026, new edition mid-2027** (project P-004717-01). Watch for DR AS/NZS 3000 draft-for-comment release. |
| **AS/NZS 3008.1.1** — Cable selection, LV (Australian conditions) | 2017 ed. incl. Amd 1 | 2026-06-22 | current | Part 1.2 (NZ conditions) also 2017. Watch for a joint revision aligned with 3000 revision. |
| **AS/NZS 3008.1.2** — Cable selection, LV (NZ conditions) | 2017 ed. | 2026-06-22 | current | See 3008.1.1 above. |
| **AS/NZS 3017** — Verification by inspection and testing | 2022 ed. | 2026-06-22 | current | — |
| **AS/NZS 4836** — Safe working on/near LV and ELV electrical installations | 2023 ed. | 2026-06-22 | current | Superseded 2011 ed. Watch for amendments. |

---

## MINING & QUARRYING

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 3007** — Electrical equipment in mines and quarries (surface installations) | 2013 ed. | 2026-06-22 | current | Watch for a revision — 2013 ed. is over 10 years old. Supplements AS/NZS 3000, AS 2067, AS 60204. |
| **AS/NZS 4871.1** — Electrical equipment for coal mines (intro and design) | 2005 ed. (check for amendments) | 2026-06-22 | current | AS/NZS 4871 series: also check parts .2, .3, .4. Governs underground coal mine electrical equipment. |
| **SA/SNZ HB 119** — Mines and quarries electrical protection (Handbook) | Check current edition on Standards Australia catalogue | 2026-06-22 | current | Guidance companion to AS/NZS 3007 and AS 2067. |

---

## LV SWITCHBOARD & SWITCHGEAR

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 61439.1** — LV switchgear assemblies, general rules | 2026 ed. (supersedes 2016 ed.) | 2026-06-22 | current | **NEW 2026 EDITION** — review designs referencing 2016 ed. |
| **AS/NZS 61439.2** — Power switchgear and controlgear assemblies | Check — likely still 2016-era; confirm if 2026 revision covers this part | 2026-06-22 | current | Part of the 61439 series. |
| **AS/NZS 61439.3** — Distribution boards | Check — likely still 2016-era | 2026-06-22 | current | IEC 61439-3:2024 Ed.2 published — watch for AS/NZS adoption. |
| **IEC 60947-1** — LV switchgear, general rules | 2020 ed. (6th ed.) | 2026-06-22 | current | Watch for Amendment 1. |
| **IEC 60947-2** — LV circuit-breakers | 2016 ed. incl. Amd 1 (2019), Amd 2 (2022) | 2026-06-22 | current | Used for Icc, Ics, selectivity. Watch for new amendment or edition. |
| **IEC 60947-4-1** — Contactors and motor starters | 2018 ed. | 2026-06-22 | current | Used for Type 1/2 coordination. |

---

## HV INSTALLATIONS & SUBSTATIONS

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS 2067** — Substations and HV installations exceeding 1 kV a.c. | 2016 ed. | 2026-06-22 | current | Based on IEC 61936-1. Watch for revision — 10 years old. Also track IEC 61936-1 (parent). |
| **IEC 61936-1** — Power installations exceeding 1 kV a.c. | 2021 ed. (3rd ed.) | 2026-06-22 | current | Parent of AS 2067. Revision to this may trigger AS 2067 revision. |

---

## POWER SYSTEMS & SHORT-CIRCUIT

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEC 60909-0** — Short-circuit currents in three-phase AC systems | 2016 ed. | 2026-06-22 | current | Also track IEC 60909-1 (factors), IEC 60909-3 (currents in DC auxiliary systems). Watch for revision. |
| **AS 60909-0** — Australian adoption of IEC 60909-0 | Check Standards Australia catalogue for current adoption year | 2026-06-22 | current | May lag the IEC edition. |
| **IEEE 519** — Harmonic control in electric power systems | 2022 ed. | 2026-06-22 | current | Watch for amendment. Revision cycle typically 5–10 years. |
| **AS/NZS 61000.3.6** — Limits for harmonic disturbances (MV/HV/EHV) | Check current edition | 2026-06-22 | current | Part of the EMC series. |

---

## ARC FLASH

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEEE 1584** — Arc-flash hazard calculations | 2018 ed. (2nd ed.) | 2026-06-22 | current | Track errata. |
| **IEEE 1584.1** — Arc-flash hazard scope/deliverables | 2022 ed. | 2026-06-22 | current | Companion to IEEE 1584-2018. |
| **IEEE 1584.2** — Arc-flash data collection | 2025 ed. | 2026-06-22 | current | **RECENTLY PUBLISHED** — newest in the family. |

---

## PROTECTION & METERING

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **IEC 60255 series** — Measuring relays and protection equipment | Various parts 2010–2022 | 2026-06-22 | current | Check individual parts relevant to your relay work (e.g. 60255-151 overcurrent, 60255-187 transformer diff). |
| **AS 61850 series** — Communication networks and systems in substations | IEC 61850 adopted by Standards Australia; check current parts | 2026-06-22 | current | Active revision series — multiple parts updated regularly. |

---

## SOLAR / INVERTER / BATTERY (for completeness — less core to your work but adjacent)

| Standard | Current version (baseline) | Last confirmed | Status | Also track |
|---|---|---|---|---|
| **AS/NZS 4777.1** — Grid connection of energy systems via inverters | 2024 ed. (effective Feb 2025) | 2026-06-22 | current | **RECENTLY UPDATED** — mandatory from 23 Feb 2025. |
| **AS/NZS 4777.2** — Inverter requirements | 2020 ed. incl. Amd 2 (2024) | 2026-06-22 | current | — |

---

## TO ADD (rows to populate when you have confirmed editions)
| AS/NZS 3012 | Construction and demolition sites | — | — | — |
| AS/NZS 3001 | Transportable structures | — | — | — |
| AS 4100 | Steel structures (structural — not electrical but relevant to your work) | AS 4100:2020 incl. Amd 1 (2021) | 2026-06-22 | Watch for revision |

---

*Add more standards by inserting a row in the relevant section. Keep the designation exact (e.g. `AS/NZS 61439.1`, not `61439`) so the routine can search for it precisely.*
