# Knowledge Asset Authority Semantics

> **Status:** Approved / Governing. This decision is the source of truth for the separation of lifecycle Status, Authority Level, and Canonical Source.

## Metadata

| Field | Value |
|---|---|
| Decision ID | GDR-005 |
| Title | Knowledge Asset Authority Semantics |
| Classification | Decision Record |
| Decision Category | Governance |
| Status | Approved |
| Authority Level | Governing |
| Canonical Source | Yes |
| Owner | John S. Villasenor |
| Decider / Approver | John S. Villasenor |
| Created On | 2026-07-27 |
| Decided On | 2026-07-27 |
| Last Updated | 2026-07-27 |
| Review Cadence | As Needed |
| Related Assets | GDR-001; GDR-006; OLY-GOV-002; OLY-GOV-003; OLY-GOV-005; OLY-DB-004 |
| Supersedes | N/A |
| Superseded By | N/A |
| AI Consumption | Required |
| Change Impact | High |

---

## Decision

Olympus uses three independent metadata dimensions:

1. **Status** records lifecycle maturity: `Exploratory`, `Draft`, `Proposed`, `Approved`, `Superseded`, or `Retired`.
2. **Authority Level** records binding weight: `Informational`, `Advisory`, `Canonical`, or `Governing`.
3. **Canonical Source** is `Yes` or `No` and identifies whether the asset is the source of truth for its defined subject.

**Canonical is not a lifecycle Status.** An active source-of-truth asset normally uses `Status: Approved`, `Authority Level: Canonical` or `Governing`, and `Canonical Source: Yes`.

Operational metadata requirements remain in **OLY-GOV-002**. Decision-record metadata remains in **OLY-GOV-003**. Those standards must reference this decision rather than redefine these semantics.

## Context

The foundation used “Canonical” both as a status and as an authority concept. The overlap made it difficult for humans and agents to distinguish maturity, binding weight, and source-of-truth designation.

## Options Considered

| Option | Outcome |
|---|---|
| Three independent dimensions | **Selected** — preserves lifecycle, authority, and source designation without semantic overlap |
| Keep Canonical as both Status and Authority Level | Rejected — perpetuates ambiguity |
| Merge Status and Authority into one field | Rejected — loses important governance distinctions |

## Consequences

- Active standards, templates, glossaries, and examples must align to this decision.
- Historical records remain unchanged when they accurately preserve prior usage.
- Assignment of `Approved`, `Canonical`, `Governing`, or `Canonical Source: Yes` continues to require explicit Founder approval under GDR-006 and the applicable workflow.

## Approval Context

Approved through explicit Founder direction in the E7CORE Hermes session on 2026-07-27. Commit or push is not the source of approval; this record captures the approval.

## Follow-up Actions

- Align OLY-GOV-002, OLY-GOV-003, OLY-GOV-005, templates, and RNO-001 by reference.
- Mark OLY-DB-004 resolved by GDR-005.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-27 | John S. Villasenor | Approved the three-axis metadata semantics and removed Canonical from lifecycle Status. |
