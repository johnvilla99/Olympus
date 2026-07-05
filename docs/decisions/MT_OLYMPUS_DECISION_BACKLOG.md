# Mt. Olympus — Decision Backlog

## Purpose

This backlog captures unresolved questions that should become formal decisions only when they are ready.

It prevents exploratory questions from becoming accidental architecture.

---

## Working Answers Captured (Draft / Advisory — not Approved)

Founder-aligned working direction captured in governance standards (2026-07-05). These are **not** Approved or Canonical decisions.

| Topic | Working Answer | Reference |
|---|---|---|
| Formal Knowledge Asset ID convention | Prefixes: ACR, OLY-GOV, ADR, PDR, GDR, ODR, LLR, RNO, OPM, HND; three-digit sequential numbering | OLY-GOV-002 |
| ADR/PDR/GDR/ODR decision prefixes | Approved as draft decision prefix convention | OLY-GOV-003 |
| Valid Decision Record statuses | Draft, Proposed, Approved, Superseded, Retired only — not Exploratory | OLY-GOV-003 |
| Research as tenth Muse | **No** — Research remains cross-cutting; notes in `docs/research/` with Muse lens metadata when applicable | OLY-GOV-002, Muse Catalog |
| Promotion approval authority | Only Founder approves Approved / Canonical / Governing; Curator and agents may recommend only | OLY-GOV-002, OLY-GOV-003, Governance Starter |
| Minimum metadata bar for Proposed | Defined checklist in Knowledge Asset Standard | OLY-GOV-002 |
| When to create `docs/product/` / `docs/architecture/` | Do not create now; future candidates when formal product/architecture work begins | OLY-GOV-002 |
| Research notes Muse lens metadata | Yes when applicable; General Research or TBD if none | OLY-GOV-002, `docs/research/README.md` |
| Daily log AI Consumption | Handoff Required when resuming; logs Recommended (Required if no handoff) | OLY-GOV-004 |
| Evidence packet template | Remains handoff section; no standalone template yet | OLY-GOV-004 |
| Filled handoff location | Olympus handoffs in `logs/daily/`; project handoffs in project repos | OLY-GOV-004, OLY-GOV-001 |
| Named agent roles | **John** (Founder), **Hermes** (Director), **Hephaestus** (Coder / Cursor) — Draft / Advisory | `docs/operations/OPM-001_OLYMPUS_AGENT_OPERATING_MODEL.md`; `AGENT_ROLES.md` (short reference) |
| Olympus Agent Operating Model | Draft / Advisory working answer in OPM-001 — **not** Approved or Canonical | OPM-001 |
| Knowledge Capture Workflow | Draft / Advisory triage and routing workflow in OPM-002 — **not** Approved or Canonical | OPM-002 |
| Decision Promotion / Approval Workflow | Draft / Advisory promotion workflow in OPM-003 — **not** Approved or Canonical | OPM-003 |

---

## Open Decisions

| ID | Question | Layer | Status | Notes |
|---|---|---|---|---|
| OLY-DB-001 | Is Mt. Olympus the official ecosystem name? | Vision | Open | ACR-001 lists Olympus/Mount Olympus as naming possibilities, not final decisions. |
| OLY-DB-002 | What is the official relationship between Olympus, Mnemosyne, Metis, and the Muses? | Conceptual Model | Open | Current model is promising but exploratory. |
| OLY-DB-005 | What is Curator? | Operating Model | Open | Proposed AI owner; may recommend promotion but cannot approve during foundation phase. OPM-001 does not define Curator as an active agent role. |
| OLY-DB-007 | Which project participates first? | Strategy | Open | Hobby Brain is origin, but portfolio-wide intent is explicit. |
| OLY-DB-009 | How should agents discover authoritative knowledge? | Operating Model | Open | Partially addressed by OLY-GOV-002/003/004, OPM-001, OPM-002, OPM-003, and Cursor rules; formal decision still open. |
| OLY-DB-010 | How should institutional knowledge be audited? | Governance | Open | Future concern after initial foundation. |

---

## Partially Addressed (standards exist; formal decision still open)

| ID | Question | Layer | Status | Notes |
|---|---|---|---|---|
| OLY-DB-003 | What constitutes a Knowledge Asset? | Governance | Working answer captured | See OLY-GOV-002 and Knowledge Asset Model. Formal GDR promotion deferred. |
| OLY-DB-004 | What statuses and authority levels should Knowledge Assets use? | Governance | Working answer captured | See OLY-GOV-002. Formal GDR promotion deferred. |
| OLY-DB-008 | What must every participating repository expose? | Governance | Open | Candidate: governance, decisions, architecture, handoff, source map. Handoff rules partially in OLY-GOV-004. |

---

## Deferred (Tier 3 — do not decide now)

Deferred until product / architecture phase unless noted.

| ID | Question | Layer | Notes |
|---|---|---|---|
| OLY-DB-006 | Should knowledge relationships become graph-based? | Architecture | Deferred until product / architecture phase. |
| OLY-DB-011 | Should formal Knowledge Assets remain GitHub-first or app-first later? | Architecture | Deferred until product / architecture phase. |
| OLY-DB-012 | Should decisions be a separate database table or specialized Knowledge Asset type? | Architecture | Deferred until product / architecture phase. |
| OLY-DB-013 | How much of Metis is deterministic policy versus LLM reasoning? | Product / Architecture | Deferred until product / architecture phase. |
| OLY-DB-014 | Portfolio-wide versus project-specific asset scope rules | Governance | Deferred until product / architecture phase. |
| OLY-DB-015 | Experience Note interim artifact type | Operations | Deferred | OPM-002 defers formal Experience Note type; continue using handoffs, logs, lessons, candidate assets. Revisit at product MVP design if needed. |
| OLY-DB-016 | Standalone evidence packet template | Operations | Deferred — revisit if repeated workflows require it. Handoff section sufficient for now. |
| OLY-DB-017 | Formal promotion of ID convention to Canonical/Governing | Governance | Working answer in OLY-GOV-002/003; formal GDR deferred. |

---

## Decision Discipline

Do not answer open or deferred items prematurely.

Promote a decision only when the decision will unblock meaningful work and the consequences are understood.

Working answers in governance standards are **Draft / Advisory** until promoted through the decision process.
