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

### 2026-08-30 — IEEE 1584 (revision signal: active PAR confirmed for 3rd edition)
- **Change:** Status change (not yet a document change) — a distinct IEEE SA project page for **P1584** (standards.ieee.org/ieee/1584/12061/), separate from the published IEEE 1584-2018 page, is now confirmed active, corroborated by an IEEE SA Standards Board approval record dated 28 May 2025. This is a formal revision project that would supersede IEEE 1584-2018 with a 3rd edition. Prior runs (including last week) found no confirmed active PAR for 1584 itself — this is newly surfaced evidence, not previously reflected in the baseline.
- **Old version:** IEEE 1584-2018 (2nd ed.), recorded "current" with "no confirmed active PAR found"
- **New version:** IEEE 1584-2018 unchanged in substance and remains current/in force; baseline status updated to "revision-in-progress" to reflect the confirmed active P1584 project. No PAR scope or target completion date located yet — priority for next run.
- **Source:** https://standards.ieee.org/ieee/1584/12061/ (IEEE SA project page — surfaced via WebSearch indexing; direct WebFetch to standards.ieee.org returned EGRESS_BLOCKED this run) ; https://standards.ieee.org/about/sasb/sba/28may2025/ (IEEE SA Standards Board approval record, 28 May 2025)
- **Why it matters:** IEEE 1584 is the primary arc-flash hazard calculation standard used for arc-flash studies, PPE category selection, and incident-energy labelling. No action needed yet — the 2018 2nd edition remains authoritative — but this is now the standard in the tracker most likely to see a 3rd-edition draft surface next. A related informally-discussed guide, P1584.11 (DC arc-flash calculations), remains unconfirmed (no assigned PAR/project number found) and is not yet a tracked row.
- **Action:** No document action. Priority for next run: confirm P1584's PAR scope, sponsoring working group, and target completion date via a direct fetch of standards.ieee.org/ieee/1584/12061/ if egress allows, or via sagroups.ieee.org/1584/.

### 2026-08-16 — IEC 60909-0 (new 3rd edition published)
- **Change:** New edition published. IEC 60909-0:2026 (3rd edition) has replaced the 2016 2nd edition. This resolves the revision-in-progress signal tracked over the last several runs (BSI mirror project → IEC "Under development" project record → now published).
- **Old version:** IEC 60909-0:2016 (2nd ed.)
- **New version:** IEC 60909-0:2026 (3rd ed.), published 23 Jul 2026
- **Source:** https://webstore.iec.ch/en/publication/68454 (webstore record now returns the published title format "IEC 60909-0:2026 | IEC" with an explicit 23-Jul-2026 publication date, consistent across independent search results — surfaced via WebSearch snippets only; direct WebFetch to webstore.iec.ch remains blocked by the network egress proxy this run, so this is not yet a primary-source page read); preceded by CENELEC parallel draft prEN IEC 60909-0:2025 (standards.iteh.ai)
- **Why it matters:** IEC 60909-0 underpins short-circuit current calculations for HV design, switchboard fault-rating, and protection coordination. Designs currently referencing the 2016 edition should be reviewed once the 3rd edition's technical changes are confirmed (not yet independently verified — the front matter/changes could not be read directly due to the egress block). No AS-designated adoption tracks IEC 60909-0:2016 directly (see AS 60909-0 row); Standards Australia has not yet listed a 2026-dated edition, likely just publication lag.
- **Action:** Flag for HV/short-circuit design review once technical changes are confirmed. Priority for next run: obtain a direct primary-source read of webstore.iec.ch/en/publication/68454 if egress allows, to confirm scope of technical changes and close out the "moderate confidence" caveat. Also watch AS 60909-0 (Standards Australia Store) for adoption of the 2026 edition.

### 2026-08-09 — IEC 60909-0 (revision signal advanced: IEC project record now visible, still unpublished)
- **Change:** Not a document change — a revision-in-progress signal advanced. Previously the only evidence of a 3rd edition was a BSI mirror project (2021-00323, "BS EN IEC 60909-0 Ed.3.0"). This run found a distinct IEC Webstore project record — "IEC 60909-0:2026" (publication ID 68454, list price CHF 380) — separate from the current 2016 2nd-edition record (ID 24100), with catalogue status **"Under development"**. No reseller (AFNOR, ANSI, Accuristech, CSA, DIN) has it indexed yet, and no CDV/FDIS or publication date was found.
- **Old version:** IEC 60909-0:2016 (2nd ed.), current — revision signal known only via BSI mirror project
- **New version:** IEC 60909-0:2016 remains current and in force. Ed.3.0 (targeted "IEC 60909-0:2026") confirmed as an active, numbered IEC TC 73 project — status "Under development", not yet published.
- **Source:** https://webstore.iec.ch/en/publication/68454 (surfaced via WebSearch snippet only — direct WebFetch to webstore.iec.ch, and to essentially all external domains including non-standards-body sites, was blocked this run by the network egress proxy); https://standardsdevelopment.bsigroup.com/projects/2021-00323
- **Why it matters:** IEC 60909-0 underpins short-circuit current calculations for HV design, switchboard fault-rating, and protection coordination. No action needed yet — 2016 edition remains authoritative — but this is the standard most likely to next flip to "New" in the tracker; prioritise a direct catalogue check when egress allows.
- **Action:** No document action. Continue priority monitoring of webstore.iec.ch/en/publication/68454 for a status change from "Under development" to published.

### 2026-07-26 — SA/SNZ HB 119 (revision signal: reconfirmation review opened)
- **Change:** Status change (not yet a document change) — HB 119:2019 now appears on Standards New Zealand's "Aged Standards Proposed for Reconfirmation" consultation, under committee EL-023 (Electrical Equipment in Mines and Quarries), alongside AS/NZS 4641:2018 and AS/NZS 60079.35.1/.2. This is a routine periodic lifecycle review to decide whether to reconfirm as-is, revise, or withdraw — no outcome or timeline is public yet.
- **Old version:** HB 119:2019, recorded "current" with no revision/withdrawal signal
- **New version:** HB 119:2019 unchanged in substance; baseline status updated to "revision-in-progress" to reflect the open reconfirmation review
- **Source:** consultations.standards.govt.nz (Citizen Space) consultation listing, surfaced via WebSearch snippet — not yet independently confirmed by a direct fetch (standards.govt.nz direct access is currently blocked by an organisation-level egress policy denial, see note below)
- **Why it matters:** HB 119 is the companion guidance handbook for mines/quarries electrical protection design (alongside AS/NZS 3007 (superseded), AS 2067, and AS/NZS 5368). A reconfirmation review could lead to withdrawal, minor reconfirmation with no changes, or a full revision — worth watching, no action needed yet.
- **Action:** No action required this run. Re-check next run for consultation outcome or a formal revision project reference.

### 2026-07-26 — Infrastructure note: root cause of persistent direct-fetch failures identified (no standard content change)
- **Change:** Not a standards change — an operational note. This run confirmed via the outbound proxy's status endpoint that direct WebFetch to standards.org.au, store.standards.org.au, standards.govt.nz, webstore.iec.ch, standards.ieee.org and similar domains fails with a gateway-level 403 policy denial — and that the same denial also affects unrelated control domains (e.g. en.wikipedia.org, www.google.com). This is a standing environment/egress-policy constraint, not a per-site block or a transient failure, and will not resolve through retries.
- **Why it matters:** Explains why the several open "not yet primary-source-confirmed" items in this tracker (AS/NZS 3007→5368 supersession, AS/NZS 61000.3.6 correction, HB 119 signal above) have remained secondary-source-only across multiple runs. These should be treated as settled at their stated confidence level unless the egress policy or access path changes — future runs don't need to keep re-flagging the same fetch failure as if it were new information.
- **Action:** No document action. If a maintainer wants primary-source-fetch confirmation of the open items above, the egress policy would need to allow direct access to these standards-body domains.

### 2026-07-19 — AS/NZS 61000.3.6 (baseline correction: superseded by AS/NZS TR IEC 61000.3.6:2012)
- **Change:** Baseline correction — resolves the open question flagged in the 2026-07-05 and 2026-07-12 runs. The baseline's "AS/NZS 61000.3.6:2001, current" entry was outdated: live current-product listings on both the Standards Australia store and the Standards NZ shop show AS/NZS TR IEC 61000.3.6:2012 (a Technical Report aligned with IEC/TR 61000-3-6 Ed.2.0:2008) as the standard now in force, with scope wording ("connection of distorting installations to MV, HV and EHV power systems") matching the 2008 IEC TR rather than the narrower 2001-edition scope.
- **Old version:** AS/NZS 61000.3.6:2001 (based on IEC 61000-3-6:1996) — recorded "current"
- **New version:** AS/NZS TR IEC 61000.3.6:2012 (based on IEC/TR 61000-3-6 Ed.2.0:2008)
- **Source:** https://store.standards.org.au/product/tr-iec-61000-3-6-2012 ; https://www.standards.govt.nz/shop/asnzs-tr-iec-61000-3-62012 (both surfaced via WebSearch snippets — direct WebFetch to standards.org.au/standards.govt.nz has failed with HTTP 403 at the proxy/session level for three consecutive runs, so this rests on convergent secondary-source evidence, not a live catalogue page fetch)
- **Why it matters:** AS/NZS 61000.3.6 sets harmonic-disturbance emission limits for connections to MV/HV/EHV power systems — relevant to HV design and power-quality studies. Project documentation citing AS/NZS 61000.3.6:2001 should be reviewed against the 2012 Technical Report.
- **Action:** Update project specifications referencing AS/NZS 61000.3.6:2001. **Confidence caveat:** high-confidence but not fully closed — no run has yet achieved a direct primary-source catalogue fetch (persistent 403s); the exact supersession date is also unconfirmed (one low-confidence source cited 26-06-2021). Re-attempt direct catalogue verification when WebFetch access to standards.org.au/standards.govt.nz is available.

### 2026-07-12 — AS/NZS 3007 and AS/NZS 4871 series (baseline correction: full absorption into AS/NZS 5368:2025)
- **Change:** Baseline correction — resolves the open question flagged in the 2026-07-05 run. AS/NZS 3007:2013 and the *full* AS/NZS 4871 series (Parts 1–6), not just Part 1, were jointly revised, amalgamated and redesignated as AS/NZS 5368:2025, effective 27 Jun 2025. The baseline previously showed AS/NZS 3007 as separately "current" and only AS/NZS 4871.1 as superseded.
- **Old version:** AS/NZS 3007:2013 (recorded "current"); AS/NZS 4871.1:2012 (recorded superseded, other 4871 parts not flagged)
- **New version:** Both superseded 27 Jun 2025 by AS/NZS 5368:2025
- **Source:** AS/NZS 5368:2025 foreword (via repeated, independently-worded WebSearch queries converging on consistent foreword text quoted at https://store.standards.org.au/product/as-nzs-5368-2025); reseller listings (accuristech, Intertek Inform) still tag AS/NZS 3007 "[Current]" — judged stale/lagging metadata, not authoritative.
- **Why it matters:** AS/NZS 3007 was a primary reference for surface mine/quarry electrical installations; project documentation still citing AS/NZS 3007 or the 4871 series should be updated to reference AS/NZS 5368:2025.
- **Action:** Update project specifications and procurement documents referencing AS/NZS 3007 or any AS/NZS 4871 part. **Confidence caveat:** direct WebFetch to standards.org.au / store.standards.org.au was unavailable for every research agent this run (proxy-level 403, tool-wide outage, not a site-specific block) — this finding rests on converging search-engine-indexed snippets of the official foreword text, not a live catalogue fetch. Treat as high-confidence but not fully closed; prioritise a direct catalogue confirmation next run.

### 2026-07-05 — AS 4100 (baseline correction: Amendment 2:2024)
- **Change:** Baseline correction — Amendment 2:2024 to AS 4100:2020 had already been published but was missing from the tracked baseline (Amd 1:2021 only). Confirmed current in-force document is AS 4100:2020 incl. Amd 1 (2021) and Amd 2 (2024).
- **Old version:** AS 4100:2020 incl. Amd 1 (2021) [as recorded in baseline]
- **New version:** AS 4100:2020 incl. Amd 1 (2021) and Amd 2 (2024)
- **Source:** https://store.standards.org.au/product/as-4100-2020-amd-1-2021 ; https://www.steel.org.au/news-and-events/events/new-proposed-fire-provisions-as-4100/
- **Why it matters:** Amendment 2 tightens non-destructive testing (NDT) requirements and adds ISO 3834-3 workshop certification requirements for higher construction categories — relevant to structural steelwork sign-off for switchrooms/substations adjacent to electrical scope of work.
- **Action:** Update project specifications referencing AS 4100:2020 to note Amd 2:2024. Also watch for a full new edition — see note below; a wide-ranging AS 4100 re-write (most extensive since the standard's inception) closed public comment 9 Jun 2026 and is pending publication.

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
