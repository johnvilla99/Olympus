# Mt. Olympus — Decision Backlog

## Purpose

This backlog captures unresolved questions that should become formal decisions only when they are ready.

It prevents exploratory questions from becoming accidental architecture.

---

## Established Foundation Guidance

The following guidance has been reviewed and accepted for current Olympus use. Status and Authority Level remain distinct: Approved / Advisory artifacts are active guidance but are not Canonical or Governing unless explicitly stated.

| Topic | Current Guidance | Authority Source |
|---|---|---|
| Official ecosystem name | **Olympus** | **GDR-002 — Approved / Canonical** |
| Olympus / Hobby Brain relationship | Olympus and Hobby Brain are separate projects; neither is a subproject of the other | **GDR-002 — Approved / Canonical** |
| Olympus conceptual capability model | Olympus is the ecosystem; Mnemosyne preserves memory; Metis provides judgment; Muses are domain lenses and stewards; human owners remain accountable | **GDR-003 — Approved / Canonical** |
| Eunomia ecosystem stewardship role | Eunomia is the Olympus ecosystem librarian and collection-stewardship role; it is defined but not yet instantiated as an active agent or application component | **GDR-004 — Approved / Canonical** |
| Formal Knowledge Asset ID convention | Prefix-based, three-digit stable identifiers | **GDR-001 — Approved / Canonical** |
| ADR/PDR/GDR/ODR decision prefixes | Official decision-record prefixes | **GDR-001**; applied by OLY-GOV-003 |
| Valid Decision Record statuses | Draft, Proposed, Approved, Superseded, Retired only | OLY-GOV-003 — Approved / Governing |
| Research as a Muse | **No. Research is a cross-cutting activity, not a tenth Muse.** | OLY-GOV-002; Muse Catalog; OPM-001 |
| Promotion approval authority | Only Founder approves Approved / Canonical / Governing; agents may recommend only | OLY-GOV-002; OLY-GOV-003 |
| Minimum metadata bar for Proposed | Defined in Knowledge Asset Standard | OLY-GOV-002 |
| Product / architecture directories | Create when formal product or architecture definition begins | OLY-GOV-002 |
| Research-note Muse metadata | Include relevant Muse lenses when applicable | OLY-GOV-002; `docs/research/README.md` |
| Daily log AI Consumption | Latest handoff Required when resuming; logs Recommended, Required if no handoff | OLY-GOV-004 |
| Evidence packet | Section within handoff; no standalone template required yet | OLY-GOV-004 |
| Filled handoff location | Olympus handoffs in `logs/daily/`; project handoffs in project repositories | OLY-GOV-001; OLY-GOV-004 |
| Named active agent roles | John, Hermes, Hephaestus | OPM-001 — Approved / Advisory |
| Olympus Agent Operating Model | Current operating guidance | OPM-001 — Approved / Advisory |
| Knowledge Capture Workflow | Current capture and routing guidance | OPM-002 — Approved / Advisory |
| Decision Promotion / Approval Workflow | Current promotion and approval workflow | OPM-003 — Approved / Advisory |
| Product-to-Architecture sequencing | Foundation closure precedes product definition; application governance precedes Architect agent construction; alternatives and validation precede technical-stack selection | **OPM-004 — Approved / Advisory** |
| Current roadmap position | Olympus is in **Phase 1: Foundation Closure**. Later phases require explicit Founder gate approval. | **OPM-004** |
| RNO-001 Olympus Babble Fish | Approved / Advisory terminology reference | RNO-001 |
| Agent discovery of authoritative knowledge | Current discovery and safe-consumption guidance; practical validation continues | OLY-GOV-005 — Approved / Advisory |

---

## Open Decisions

| ID | Question | Layer | Status | Notes |
|---|---|---|---|---|
| OLY-DB-010 | How should institutional knowledge be audited? | Governance | Open | Evaluate during OPM-004 Phase 1 Foundation Closure. The answer may become part of the Foundation Closure Assessment or a separate governance decision. |

---

## Partially Addressed

| ID | Question | Layer | Status | Notes |
|---|---|---|---|---|
| OLY-DB-003 | What constitutes a Knowledge Asset? | Governance | Working answer captured | See Approved / Advisory OLY-GOV-002 and Knowledge Asset Model. Formal stronger-authority promotion remains optional. Assess sufficiency during OPM-004 Phase 1. |
| OLY-DB-004 | What statuses and Authority Levels should Knowledge Assets use? | Governance | Working answer captured | See Approved / Advisory OLY-GOV-002. Assess whether stronger authority is required during OPM-004 Phase 1. |
| OLY-DB-008 | What must every participating repository expose? | Governance | Open | Candidate: governance, decisions, architecture, handoff, source map. Handoff rules are partially covered by OLY-GOV-004. Must be resolved no later than OPM-004 Phase 3 if participating-project onboarding is in MVP scope. |
| OLY-DB-009 | How should agents discover authoritative knowledge? | Operating Model | Partially Addressed | OLY-GOV-005 is Approved / Advisory and accepted for current use. Practical validation is deferred to OPM-004 Phases 5 and 6, when architecture and discovery behavior can be tested. |

---

## Resolved / Promoted

| ID | Question | Resolution | Source |
|---|---|---|---|
| OLY-DB-001 | Is Mt. Olympus the official ecosystem name? | Resolved on 2026-07-25. The official ecosystem name is **Olympus**. | **GDR-002 — Approved / Canonical** |
| OLY-DB-002 | What is the official relationship between Olympus, Mnemosyne, Metis, and the Muses? | Resolved on 2026-07-25. Olympus is the ecosystem; Mnemosyne and Metis are cross-cutting memory and judgment capabilities; Muses are durable domain lenses and stewards; human owners retain accountability and approval remains governed. | **GDR-003 — Approved / Canonical** |
| OLY-DB-005 | What is Curator? | Resolved on 2026-07-25. The Curator working concept is renamed **Eunomia** and defined as the Olympus ecosystem librarian and collection-stewardship role. Eunomia is not yet an active agent or application component. | **GDR-004 — Approved / Canonical** |
| OLY-DB-007 | Which project participates first? | Resolved on 2026-07-25. The premise is retired: Olympus and Hobby Brain are separate projects. Hobby Brain is not an Olympus subproject, and Olympus is not a Hobby Brain subproject. Any future participation or adoption relationship requires a separate explicit decision. | **GDR-002 — Approved / Canonical** |
| OLY-DB-017 | Formal promotion of ID convention | Resolved on 2026-07-25. Prefix-based, three-digit stable IDs are official Olympus practice. | **GDR-001 — Approved / Canonical** |

---

## Deferred and Roadmap-Routed

Questions below remain undecided. OPM-004 identifies the earliest phase in which each may be considered. Placement here does not authorize resolution.

| ID | Question | Layer | Earliest Roadmap Phase | Notes |
|---|---|---|---|---|
| OLY-DB-006 | Should knowledge relationships become graph-based? | Architecture | Phase 5 | Compare relational, graph-augmented, and other viable relationship models before selection. |
| OLY-DB-011 | Should formal Knowledge Assets remain GitHub-first or app-first later? | Product / Architecture | Phase 2 for product need; Phase 5 for architecture | Product requirements must precede storage and synchronization decisions. |
| OLY-DB-012 | Should decisions be a separate database table or specialized Knowledge Asset type? | Architecture | Phase 5 | Requires approved product and application-governance inputs. |
| OLY-DB-013 | How much of Metis is deterministic policy versus LLM reasoning? | Product / Architecture | Phase 3 for governance boundary; Phase 5 for architecture | Runtime authority and human-control rules must be defined before technical allocation. |
| OLY-DB-014 | Portfolio-wide versus project-specific asset scope rules | Governance | Phase 3 | Required when application governance defines participating-project boundaries. |
| OLY-DB-015 | Experience Note interim artifact type | Operations | After Phase 1 unless evidence demands earlier action | Continue using handoffs, logs, lessons, and candidate assets. |
| OLY-DB-016 | Standalone evidence packet template | Operations | After repeated gate reviews demonstrate need | Handoff and gate-review sections remain sufficient for now. |

---

## Decision Discipline

- Do not answer open or roadmap-routed items prematurely.
- Use OPM-004 to determine sequencing, prerequisites, and gate ownership.
- Promote a decision only when it will unblock meaningful work and consequences are understood.
- Approved / Advisory guidance is active but does not become Canonical or Governing by implication.
- Backlog status must reflect formal decisions when promotion occurs.
- Completion of a phase artifact does not authorize progression without explicit Founder gate approval.
