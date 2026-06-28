# Standards Change Log

Append-only log of confirmed changes found by the weekly routine. Newest entries at top. The routine writes here when it confirms a standard has changed; you can also add manual entries.

_Do not delete past entries._

---

## Format
```
### YYYY-MM-DD — [Standard designation]
- **Change:** [new edition / amendment / errata / withdrawal]
- **Old version:** [previous designation]
- **New version:** [new designation]
- **Source:** [official catalogue URL]
- **Why it matters:** [one line on practical impact — affects arc-flash inputs / switchboard design / cable sizing / etc.]
- **Action:** [e.g. "Review open designs referencing old edition" / "No immediate action — minor errata" / "Update baseline"]
```

---

## Log

### 2026-06-28 — AS 61850 series (IEC 61850) — new 2025–2026 parts confirmed
- **Change:** Four additional publications confirmed in the active IEC 61850 series, not captured in the 2026-06-22 baseline: IEC 61850-10:2012+AMD1:2025 (conformance testing amendment), IEC TR 61850-90-30:2025 (SCL extensions), IEC TR 61850-1-1:2026 (new TR), IEC TR 61850-80-5:2026 (new edition)
- **Old version:** Baseline noted IEC TS 61850-6-3:2025 and IEC TR 61850-90-21:2025 as the most recent additions
- **New version:** Additionally confirmed: IEC 61850-10:2012+AMD1:2025, IEC TR 61850-90-30:2025, IEC TR 61850-1-1:2026, IEC TR 61850-80-5:2026
- **Source:** https://webstore.iec.ch/en/publication/6028 (IEC 61850:2026 SER); https://webstore.iec.ch/en/publication/108858 (IEC 61850-10+AMD1:2025)
- **Why it matters:** IEC 61850-10:2012+AMD1:2025 updates conformance test procedures for IEC 61850 devices (client, server, sampled values, engineering tools, GOOSE performance) — directly relevant for device specification, procurement, and factory acceptance testing in digital substations. IEC TR 61850-80-5:2026 replaces the 2024 edition for Modbus/IEC 61850 gateway mapping. TR 61850-1-1:2026 and TR 61850-90-30:2025 provide updated architectural and SCL function-specification guidance.
- **Action:** Review IEC 61850-10:2012+AMD1:2025 when specifying or testing IEC 61850-compliant protection and automation devices. Update reference library with the 2026 TR editions. Note IEC TR 61850-80-5:2026 if any legacy Modbus/IEC 61850 gateway projects are in scope.

### 2026-06-22 — IEC 60947-4-1:2023/COR1:2026
- **Change:** Technical Corrigendum 1 published March 2026 to the 5th edition (2023)
- **Old version:** IEC 60947-4-1:2023 (5th ed.) — no corrigendum
- **New version:** IEC 60947-4-1:2023 (5th ed.) + COR1:2026
- **Source:** https://webstore.iec.ch/en/publication/111823
- **Why it matters:** Corrects technical errors in the electromechanical contactors and motor-starters standard used for LV switchboard Type 1/Type 2 coordination; any design referenced against the uncorrected 2023 edition should be reviewed against the corrected copy.
- **Action:** Obtain the updated (post-COR1) copy of IEC 60947-4-1:2023. Review any LV switchboard designs finalised against the uncorrected 2023 edition.

### 2026-06-22 — AS/NZS 5368:2025 (supersedes AS/NZS 4871.1)
- **Change:** New consolidated standard published, superseding AS/NZS 4871.1:2012
- **Old version:** AS/NZS 4871.1:2012 (and related 4871-series parts)
- **New version:** AS/NZS 5368:2025 (effective 27 June 2025)
- **Source:** https://store.standards.org.au/product/as-nzs-5368-2025 / https://webstore.ansi.org/standards/sai/nzs53682025
- **Why it matters:** Replaces the principal design and installation standard for electrical equipment in mines and quarries. Any project referencing AS/NZS 4871.1 must now use AS/NZS 5368:2025.
- **Action:** Update project specifications and procurement documents that reference AS/NZS 4871.1. Add AS/NZS 5368 to tracked standards list.

### 2026-06-22 — IEC 60947-4-1
- **Change:** New 5th edition published
- **Old version:** IEC 60947-4-1:2018 (4th ed.)
- **New version:** IEC 60947-4-1:2023 (5th ed.)
- **Source:** https://webstore.iec.ch/en/publication/74487
- **Why it matters:** Governs electromechanical contactors and motor-starters; used for Type 1/Type 2 coordination in LV switchboards. New edition may change test requirements or ratings.
- **Action:** Check current switchboard designs against 2023 edition requirements; update specifications.

### 2026-06-22 — IEC 60947-2
- **Change:** New 6th edition published
- **Old version:** IEC 60947-2:2016 incl. Amd 1 (2019), Amd 2 (2022)
- **New version:** IEC 60947-2:2024 (6th ed.)
- **Source:** https://webstore.iec.ch/en/publication/66277
- **Why it matters:** Core standard for LV circuit-breakers (Icc, Ics ratings, selectivity). New edition supersedes both the 2016 base and its amendments; switchboard design documents referencing the 2016 edition should be reviewed.
- **Action:** Review open switchboard projects for compliance against 2024 edition. Update specification templates.

### 2026-06-22 — AS/NZS 61439.2
- **Change:** New 2026 edition published
- **Old version:** AS/NZS 61439.2:2016
- **New version:** AS/NZS 61439.2:2026
- **Source:** https://store.standards.org.au/product/as-nzs-61439-2-2026
- **Why it matters:** Specific rules for power switchgear and controlgear assemblies (MCC panels, power boards). Published alongside AS/NZS 61439.1:2026; designs referencing the 2016 edition need review.
- **Action:** Review open MCC and power-board designs. Confirm which clauses changed before updating project documents.

### 2026-06-22 — AS/NZS 3008.1.1
- **Change:** New 2025 edition published
- **Old version:** AS/NZS 3008.1.1:2017 incl. Amd 1
- **New version:** AS/NZS 3008.1.1:2025
- **Source:** https://store.standards.org.au/product/as-nzs-3008-1-1-2025
- **Why it matters:** The primary Australian cable-selection standard for LV systems — current-carrying capacity, voltage drop, short-circuit ratings, correction factors. A new edition may revise tables or correction factors used in cable sizing calculations.
- **Action:** Obtain new edition; compare key tables against 2017 ed. Review open cable selection calculations for any impact. Note: AS/NZS 3008.1.2 (NZ conditions) remains at 2017 ed.

### 2026-06-22 — AS 2067 (revision-in-progress)
- **Change:** Active draft (DR AS 61936.1:2025) confirmed; public comment period closed April 2026
- **Old version:** AS 2067:2016 (remains current until replaced)
- **New version:** (pending — DR AS 61936.1:2025 in finalisation)
- **Source:** https://www.standards.org.au/news/standards-australia-calls-on-industry-to-help-shape-high-voltage-safety
- **Why it matters:** AS 2067 is the primary HV installation standard in Australia. The replacement standard (based on IEC 61936-1:2021) will update earthing, fire risk management, and protection requirements. Monitor for publication date.
- **Action:** Flag for HV substation design projects. No action on current designs yet — AS 2067:2016 remains in force until final publication.

### 2026-06-22 — AS/NZS 61439.1
- **Change:** New edition published
- **Old version:** AS/NZS 61439.1:2016
- **New version:** AS/NZS 61439.1:2026
- **Source:** standards.org.au standards catalogue
- **Why it matters:** General rules for LV switchgear assemblies — affects switchboard design and verification methodology under clause 10.11.4 and related clauses.
- **Action:** Review open switchboard designs and specs referencing 2016 edition. Confirm which clauses changed before updating project documents.

### 2026-06-22 — IEEE 1584.2
- **Change:** New companion standard published
- **Old version:** (did not previously exist)
- **New version:** IEEE 1584.2-2025
- **Source:** IEEE Standards Association
- **Why it matters:** Data-collection companion to IEEE 1584-2018 arc-flash model. Defines how to collect field data for arc-flash studies.
- **Action:** Review against current arc-flash study data-collection practice.

### 2026-06-22 — AS/NZS 4777.1
- **Change:** New edition, mandatory from 23 Feb 2025
- **Old version:** AS/NZS 4777.1:2016
- **New version:** AS/NZS 4777.1:2024
- **Source:** Standards Australia / Energy Networks Australia
- **Why it matters:** Inverter installation requirements — affects grid-connect solar and battery inverter designs.
- **Action:** Ensure any inverter installation work references 2024 edition.

---
