# Olympus ID Convention

> **Status:** Proposed Decision Record. This document is ready for John review but does not approve the ID convention. Approval requires explicit John approval per OPM-003.

## Metadata

| Field | Value |
|---|---|
| Decision ID | GDR-001 |
| Title | Olympus ID Convention |
| Classification | Decision Record |
| Decision Category | Governance |
| Status | Proposed |
| Authority Level | Advisory |
| Owner | John S. Villasenor |
| Decider / Approver | TBD — requires explicit John approval |
| Created On | 2026-07-05 |
| Decided On | TBD |
| Last Updated | 2026-07-05 |
| Review Cadence | As Needed |
| Related Assets | OLY-GOV-001; OLY-GOV-002; OLY-GOV-003; OPM-003; OLY-DB-017; Decision Backlog; RNO-001 Olympus Babble Fish |
| Supersedes | N/A |
| Superseded By | N/A |
| AI Consumption | Recommended |
| Change Impact | Medium |

---

## Decision

**Proposed decision statement:** Olympus should use stable, prefix-based, three-digit identifiers for formal Knowledge Assets and decision records.

### Proposed prefix convention

| Prefix | Asset Type |
|---|---|
| ACR | Architectural Concept Record |
| OLY-GOV | Olympus Governance Standard |
| ADR | Architecture Decision Record |
| PDR | Product Decision Record |
| GDR | Governance Decision Record |
| ODR | Operating Decision Record |
| LLR | Lesson Learned Record |
| RNO | Research Note |
| OPM | Operating Model |
| HND | Handoff / Continuity Artifact |

### Proposed rules

- Sequential **three-digit** numbering within each prefix (e.g. `GDR-001`, `OPM-003`).
- IDs are **stable once assigned**.
- **Retired** or **superseded** IDs are **not reused**.
- **Existing IDs** remain valid.
- **New prefixes** require future governance review or decision.

## Context

The ID convention was previously captured as **Draft / Advisory working guidance** in OLY-GOV-002 and related standards.

**OLY-DB-017** (`docs/decisions/MT_OLYMPUS_DECISION_BACKLOG.md`) tracks formal promotion of the ID convention to Canonical or Governing authority. **GDR-001** responds to OLY-DB-017 but does not close it until explicit approval is captured.

A formal **GDR** is needed because IDs affect all future Knowledge Assets, decisions, handoffs, and agent workflows — citation, supersession, discovery, and AI consumption all depend on stable identifiers.

This record is the **first formal decision record candidate** in Olympus. It is now **Proposed** for John review — not Approved.

## Options Considered

| Option | Summary | Pros | Cons |
|---|---|---|---|
| Option A | Prefix-based IDs by asset type | Clear, scalable, human-readable, aligns with existing docs | Requires maintaining prefix discipline |
| Option B | Single global OLY-* sequence | Simple global numbering | Harder to identify asset type quickly |
| Option C | Directory-based filenames without stable IDs | Easy at first | Weak for citations, supersession, and AI consumption |
| Option D | Defer formal ID convention | Avoids premature governance | Increases drift as assets grow |

## Rationale

**Option A** is currently preferred because:

- Already used throughout the repository
- Supports AI consumption and safe source evaluation
- Supports citation and handoff continuity
- Helps distinguish decisions from concepts, standards, operations, lessons, and research
- Aligns with OLY-GOV-001, OLY-GOV-002, and OLY-GOV-003
- Reduces accidental authority confusion when status is checked alongside ID type

## Consequences

If this decision is eventually approved:

- Future formal assets should use the prefix convention.
- Templates and Cursor rules should align with the approved convention.
- Existing Draft / Advisory documents and IDs remain valid.
- The convention creates some governance overhead for ID assignment and maintenance.
- New prefixes should be rare and reviewed before adoption.

## Risks

- Too many prefixes could create confusion.
- **RNO** may not perfectly fit Babble Fish and other reference documents (see RNO-001).
- **HND** may need future clarification for promoted vs operational handoffs.
- Prefixes could imply authority if **status** and **authority level** are ignored.
- Agents may over-focus on IDs instead of content value and rationale.

## Approval Requirements

- Moving this GDR to **Approved** requires **explicit John approval**.
- **Commit/push does not equal approval.**
- **Proposed** means ready for John review; it is **not** approved guidance.
- If approved, update: status, Decider / Approver, Decided On, authority level if needed, backlog **OLY-DB-017**, and related standards if needed.
- **Approved** does not automatically mean **Canonical** or **Governing** unless John explicitly assigns that authority.

## Follow-up Actions

| Action | Owner | Target |
|---|---|---|
| Review Proposed GDR-001 with John | Hermes / John | Current decision review |
| Decide whether to approve, revise, or return to Draft | John | TBD |
| If approved, update OLY-DB-017 | Hephaestus | After approval |
| Consider whether Babble Fish needs a better prefix than RNO | Hermes / John | Later |
| Keep templates and Cursor rules aligned | Hephaestus | Ongoing |

## Supersedes / Superseded By

| Relationship | Asset ID | Notes |
|---|---|---|
| Supersedes | N/A | First formal ID convention decision candidate |
| Superseded By | N/A | N/A |

## Open Questions

- Should this GDR be **approved** after John review?
- Should the ID convention become **Canonical** or remain **Advisory**?
- Should Olympus create a **`REF-*`** prefix for reference notes?
- Should **`HND-*`** be used for every handoff or only promoted continuity artifacts?
- Should participating project repositories adopt the same prefix convention?

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial Draft GDR for Olympus ID convention |
| 2026-07-05 | John S. Villasenor | Promoted GDR-001 from Draft to Proposed for John review; not Approved |
