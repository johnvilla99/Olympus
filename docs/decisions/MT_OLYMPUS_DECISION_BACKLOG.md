# Olympus — Decision Backlog

## Purpose

This backlog captures unresolved questions that should become formal decisions only when ready. It prevents exploratory questions from becoming accidental authority or architecture.

---

## Established Foundation Guidance

| Topic | Current Guidance | Authority Source |
|---|---|---|
| Official ecosystem name | **Olympus** | GDR-002 — Approved / Canonical |
| Display alias | “Mt. Olympus” is permitted as a display or narrative alias, not a separate ecosystem | GDR-008 — Approved / Canonical |
| Olympus conceptual capability model | Olympus is the ecosystem; Mnemosyne is memory; Metis is judgment; Muses are durable domain lenses | GDR-003 — Approved / Canonical |
| Eunomia | Ecosystem librarian and collection-stewardship role; defined but not instantiated | GDR-004 — Approved / Canonical |
| Formal identifiers | Stable prefix-based, three-digit identifiers | GDR-001 — Approved / Canonical |
| Metadata semantics | Status, Authority Level, and Canonical Source are independent dimensions | GDR-005 — Approved / Governing |
| Authority resolution | One governing Olympus authority hierarchy; lower-authority assets reference it | GDR-006 — Approved / Governing |
| Active durable repository | `e7-jvillasenor/Olympus` on `main`; `johnvilla99/Olympus` is historical migration context | GDR-007 — Approved / Canonical |
| Knowledge Asset procedure | Current lifecycle, metadata, placement, and promotion guidance | OLY-GOV-002 — Approved / Advisory |
| Decision-record procedure | Decision lifecycle, approval capture, and backlog discipline | OLY-GOV-003 — Approved / Governing |
| Agent discovery | Authority-aware discovery and safe consumption; Phase 1 validation recorded | OLY-GOV-005 — Approved / Advisory; RNO-002 |
| Operating roles | John, Hermes, Hephaestus; Eunomia not instantiated | OPM-001 — Approved / Advisory |
| Knowledge capture | Current capture and routing workflow | OPM-002 — Approved / Advisory |
| Promotion and approval | Current decision-promotion and approval workflow | OPM-003 — Approved / Advisory |
| Product-to-Architecture sequencing | Foundation closure precedes product; application governance precedes architecture | OPM-004 — Approved / Advisory |

---

## Open Decisions

| ID | Question | Layer | Status | Notes |
|---|---|---|---|---|
| OLY-DB-008 | What must every participating repository expose? | Application Governance | Open | Required before Architecture if participating-project onboarding is in product scope. |
| OLY-DB-010 | How should institutional knowledge be audited? | Application Governance | Open | Required before Architecture; define governance expectations before technical design. |

---

## Partially Addressed

| ID | Question | Layer | Status | Notes |
|---|---|---|---|---|
| OLY-DB-003 | What constitutes a Knowledge Asset? | Governance / Product | Working answer retained | OLY-GOV-002 and the Knowledge Asset Model remain the Phase 2 working basis. Stronger-authority promotion is optional and deferred. |
| OLY-DB-009 | How should agents discover authoritative knowledge? | Operating Model | Validated working answer; promotion decision pending | OLY-GOV-005 is Approved / Advisory and RNO-002 records four Phase 1 validation cases. Further promotion or closure requires a separate decision. |

---

## Resolved / Promoted

| ID | Question | Resolution | Source |
|---|---|---|---|
| OLY-DB-001 | Official ecosystem name | Resolved: **Olympus** | GDR-002 |
| OLY-DB-002 | Relationship among Olympus, Mnemosyne, Metis, and Muses | Resolved through the conceptual capability model | GDR-003 |
| OLY-DB-004 | What Status and Authority semantics should Knowledge Assets use? | Resolved: independent Status, Authority Level, and Canonical Source dimensions | GDR-005 |
| OLY-DB-005 | What is Curator? | Resolved: retired working term replaced by Eunomia | GDR-004 |
| OLY-DB-007 | Which project participates first? | Resolved: premise retired; Olympus and Hobby Brain are separate | GDR-002 |
| OLY-DB-017 | Formal promotion of ID convention | Resolved: official stable identifiers | GDR-001 |
| Authority hierarchy drift | Which hierarchy controls? | Resolved: GDR-006 is the single Governing authority source | GDR-006 |
| Active repository location | Which repository is durable? | Resolved: `e7-jvillasenor/Olympus` on `main` | GDR-007 |
| Display alias | Is “Mt. Olympus” a separate identity? | Resolved: display alias only | GDR-008 |

---

## Deferred and Roadmap-Routed

| ID | Question | Layer | Earliest OPM-004 Phase | Notes |
|---|---|---|---|---|
| OLY-DB-006 | Should knowledge relationships become graph-based? | Architecture | Phase 5 | Compare viable relationship models before selection. |
| OLY-DB-011 | Should formal assets remain GitHub-first or become app-first? | Product / Architecture | Phase 2 / Phase 5 | Product requirements precede storage and synchronization decisions. |
| OLY-DB-012 | Should decisions be a separate database table or Knowledge Asset specialization? | Architecture | Phase 5 | Requires approved product and application-governance inputs. |
| OLY-DB-013 | How much of Metis is deterministic policy versus LLM reasoning? | Product / Architecture | Phase 3 / Phase 5 | Human-control and authority rules precede technical allocation. |
| OLY-DB-014 | Portfolio-wide versus project-specific asset scope | Application Governance | Phase 3 | Must be resolved before broad project onboarding. |
| OLY-DB-015 | Experience Note interim artifact type | Operations | After Phase 1 | Continue using handoffs, logs, lessons, and candidate assets. |
| OLY-DB-016 | Standalone evidence packet template | Operations | After repeated gate reviews | Existing handoff and gate sections remain sufficient. |

---

## Decision Discipline

- Do not answer open or roadmap-routed questions prematurely.
- Use [[OPM-004_OLYMPUS_PRODUCT_TO_ARCHITECTURE_ROADMAP|OPM-004]] for sequencing and gate ownership.
- Use [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]] for metadata semantics and GDR-006 for authority resolution.
- Promote only when a decision unblocks meaningful work and consequences are understood.
- Commit or push is not approval.
- Completion of a phase artifact does not authorize progression without explicit Founder gate approval.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-25 | John S. Villasenor | Aligned backlog with approved foundation decisions and OPM-004 roadmap. |
| 2026-07-27 | Hermes under explicit Founder direction | Resolved OLY-DB-004, authority hierarchy, repository location, and display alias; recorded OLY-DB-009 validation status and routed remaining governance questions. |
