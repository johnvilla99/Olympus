# Decision Record Standard

> **Status:** Approved / Governing. This standard controls Olympus decision-record lifecycle and procedure while deferring authority resolution to GDR-006.

## Metadata

| Field | Value |
|---|---|
| Standard ID | OLY-GOV-003 |
| Title | Decision Record Standard |
| Status | Approved |
| Authority Level | Governing |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-27 |
| Review Cadence | As Needed |
| Related Assets | GDR-001; GDR-004; GDR-005; GDR-006; OLY-GOV-002; OPM-003; Decision Backlog |
| AI Consumption | Required |
| Change Impact | High |

---

## Purpose

Make decisions **trustworthy, traceable, reviewable, and safe** for future humans and AI agents to consume.

Decision records preserve what was decided, why it mattered, what options were considered, who approved it, what consequences remain, and what future work is affected.

## Scope

Applies to formal decision records and the Decision Backlog in the Olympus repository.

**In scope:** decision identification, categories, metadata, lifecycle, approval capture, backlog promotion, supersession, retirement, and AI consumption.

**Out of scope:** application implementation, database schema, UI design, automated approval pipelines, and automatic promotion of an existing asset.

## Definition of a Decision Record

A **Decision Record** is a formal Knowledge Asset that captures a proposed, approved, superseded, or retired decision and the rationale required for future reasoning.

Decision records belong in `docs/decisions/` and align with OLY-GOV-002.

## What Qualifies

Create a decision record when a durable choice affects future work, multiple options existed, and preserving rationale prevents rediscovery or re-litigation.

Examples include governance standards, official identifier conventions, product scope, architecture direction, operating processes, and project participation decisions.

## What Does Not Qualify

- Exploratory discussion or brainstorming
- Assistant recommendations not explicitly accepted
- Temporary working assumptions
- Open Decision Backlog questions
- Unresolved conflicts
- Notes captured for later consideration
- Architectural Concept Records unless promoted through the decision process

## Decision Record Categories

| Prefix | Category | Purpose | Typical Location |
|---|---|---|---|
| ADR | Architecture Decision Record | Technical architecture and system structure | `docs/decisions/` |
| PDR | Product Decision Record | Product scope, UX, MVP, roadmap, or user value | `docs/decisions/` |
| GDR | Governance Decision Record | Governance, standards, authority, policy, or stewardship | `docs/decisions/` |
| ODR | Operating Decision Record | Operating process, roles, workflow, or participation | `docs/decisions/` |

ACR means Architectural Concept Record and is not a decision record. **GDR-001** is the Canonical source for ADR/PDR/GDR/ODR identifiers.

## Decision ID Rules

Use **GDR-001** for stable identifiers, numbering, non-reuse, and filename alignment. This standard does not reproduce those rules.

Decision records retain their ID through supersession or retirement.

## Required Decision Metadata

| Field | Meaning |
|---|---|
| Decision ID | Stable identifier governed by GDR-001 |
| Title | Human-readable decision title |
| Classification | Decision Record |
| Decision Category | Architecture, Product, Governance, or Operating |
| Status | Lifecycle value governed by GDR-005 |
| Authority Level | Binding weight governed by GDR-005 |
| Canonical Source | Source-of-truth designation governed by GDR-005 |
| Owner | Accountable human owner |
| Decider / Approver | Person or authority who approved the decision |
| Created On | Creation date |
| Decided On | Approval date, when approved |
| Last Updated | Latest material update |
| Review Cadence | Expected review rhythm |
| Related Assets | Source concepts, standards, projects, or decisions |
| Supersedes | Prior decision IDs replaced by this record |
| Superseded By | Later decision ID replacing this record |
| AI Consumption | Required, Recommended, Optional, or Restricted |
| Change Impact | Low, Medium, or High |

Required content normally includes Decision, Context, Options Considered, Rationale, Consequences, Risks, Follow-up Actions, supersession information, and Change History.

## Decision Status Model

Use **GDR-005** for lifecycle Status, Authority Level, and Canonical Source semantics.

Decision records may use `Draft`, `Proposed`, `Approved`, `Superseded`, or `Retired`. They do not use `Exploratory`; unresolved exploration belongs in concept records or the Decision Backlog.

## Decision Authority Rules

Use **GDR-006** as the Governing Olympus authority hierarchy. This standard does not reproduce that hierarchy.

Decision-specific rules:

- A backlog item is a question, not a decision.
- `Proposed` is ready for review, not approval.
- An Approved decision may carry Advisory, Canonical, or Governing authority under GDR-005.
- Conflicts must be surfaced and routed through OPM-003.

## Decision Creation Rules

Create a decision record when the decision affects future work, multiple options existed, and rationale has future value.

- Start from the decision template when useful.
- Assign an ID under GDR-001.
- Set an honest initial Status, normally Draft or Proposed.
- Capture the decision, context, options, rationale, consequences, risks, affected assets, follow-up actions, and history.
- Avoid decision bureaucracy for trivial tactical choices.

## Decision Review and Approval

Preferred lifecycle:

```text
Draft → Proposed → Approved
```

- Approval and authority assignment follow GDR-005, GDR-006, and OPM-003.
- **Eunomia** is defined by GDR-004; it may recommend stewardship action but cannot approve and is not yet instantiated.
- AI agents may recommend or draft but cannot approve.
- Approval must be explicit and must capture date, context, and approver.
- Approved does not automatically mean Canonical or Governing.

## Decision Backlog Rules

The backlog lives at `docs/decisions/MT_OLYMPUS_DECISION_BACKLOG.md`.

- Open questions belong in the backlog before they become decisions.
- Promote only when the decision will unblock meaningful work and consequences are understood.
- When promoted, update the backlog with the Decision ID and resolution.
- Preserve backlog history.
- OLY-DB identifiers are backlog-question IDs, not decision IDs.

## Decision Supersession and Retirement

- Preserve superseded decisions and link both predecessor and successor.
- Retired decisions explain why they are inactive.
- Do not erase historical rationale.

## Relationship and Citation Rules

Decision records should cite source assets and identify affected standards, concepts, projects, and related decisions. Recognized relationship terms include `informs`, `supersedes`, `contradicts`, `depends_on`, `implements`, `references`, `replaces`, and `related_to`.

If a decision resolves a backlog question, link both records.

## AI Consumption Rules

Agents must:

- Treat backlog items as questions
- Distinguish Proposed from Approved
- Respect GDR-005 metadata and GDR-006 authority
- Prefer applicable Approved decisions over exploratory concepts
- Cite material decision sources
- Flag conflicts
- Never infer approval from repetition, silence, commit, or push

## Founder Direction Capture

Authority follows **GDR-006**. Durable Founder direction that affects future work should be captured proportionally in a decision record or explicitly related governed asset. Conflicts with existing records must be surfaced and routed through OPM-003.

## Prohibited Practices

- Treating ACRs or backlog items as approved decisions
- Treating assistant suggestions as decisions
- Inferring approval from silence, repetition, commit, or push
- Creating decisions without rationale or options
- Reusing IDs
- Deleting superseded decisions
- Promoting decisions without authorized approval
- Assigning Exploratory Status to a Decision Record
- Reproducing authority hierarchy or identifier definitions owned by GDR-006 or GDR-001

## Exceptions

Exception authority and approval follow GDR-006 and OPM-003. Document an approved exception in the affected decision, backlog item, or governance asset.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial draft |
| 2026-07-05 | John S. Villasenor | Added decision categories, lifecycle, and Founder-only approval working guidance |
| 2026-07-25 | John S. Villasenor | Approved as Governing decision-record procedure |
| 2026-07-27 | Hermes under explicit Founder direction | Referenced GDR-001 and GDR-004 through GDR-006; removed duplicated identifier, metadata, and authority-hierarchy definitions. |
