# Decision Promotion and Approval Workflow

> **Status:** Approved / Advisory operating workflow. Accepted for current Olympus use; not Canonical or Governing.

## Metadata

| Field | Value |
|---|---|
| Knowledge Asset ID | OPM-003 |
| Title | Decision Promotion and Approval Workflow |
| Classification | Operating Model |
| Category | Operations / Governance |
| Status | Approved |
| Authority Level | Advisory |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Primary AI Owner | Hermes |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-27 |
| Review Cadence | As Needed |
| Related Assets | GDR-001; GDR-004; GDR-005; GDR-006; OLY-GOV-002; OLY-GOV-003; OPM-001; OPM-002; OPM-004; Decision Backlog |
| AI Consumption | Recommended |
| Change Impact | Medium |

---

## Purpose

Define how Olympus promotes questions, working answers, and durable direction into formal decision records without confusing discussion, persistence, or agent recommendation with approval.

## Core Principle

A decision is approved only when the authorized human authority explicitly approves it and the record preserves enough context for future work.

Backlog items are questions. Working answers are guidance. Decision records preserve Proposed, Approved, Superseded, or Retired choices with rationale.

## Decision Outcomes

| Outcome | Use When |
|---|---|
| No Decision | Tactical choice with no durable consequence |
| Backlog Item | Question remains unresolved |
| Working Answer | Useful guidance does not yet require formal approval |
| Draft Decision Record | Record is being shaped |
| Proposed Decision Record | Ready for review |
| Approved Decision Record | Explicit approval is captured |
| Superseded Decision | Replaced by a newer record |
| Retired Decision | No longer active without direct replacement |

## Promotion Decision Tree

1. Ephemeral or tactical? No decision.
2. Unresolved but consequential? Backlog.
3. Useful guidance without formal approval need? Working answer.
4. Durable direction selected? Draft or Proposed decision record.
5. Options, rationale, consequences, risks, and related assets complete? Proposed.
6. Explicit authorized approval captured? Approved.
7. Replaces an older decision? Supersede and link both.
8. No longer active without replacement? Retire with rationale.
9. Uncertain? Keep in backlog or Draft.

## Governing References

- **GDR-001** controls identifiers.
- **GDR-005** controls Status, Authority Level, and Canonical Source semantics.
- **GDR-006** controls authority resolution.
- **OLY-GOV-003** controls decision-record procedure.
- **GDR-004** defines Eunomia but does not instantiate it or grant approval authority.
- **OPM-004** controls phase and gate sequencing.

This workflow does not reproduce those definitions.

## Readiness for Proposed

A decision candidate is ready for Proposed when the problem, decision statement, owner, category, options, rationale, consequences, risks, related assets, affected artifacts, open questions, AI Consumption, Change Impact, and approval status are clear enough for review.

## Readiness for Approved

A decision is ready for Approved only when:

- The authorized human approver explicitly approves it.
- Approval date and context are captured.
- Status and authority metadata follow GDR-005.
- Follow-up updates are identified.
- Supersession or retirement links are added when relevant.

## Backlog Rules

- OLY-DB items are questions, not decisions.
- Preserve backlog history.
- Link promoted items to their decision record.
- State what remains unresolved for partially addressed items.
- Working answers remain at their stated authority until promoted.

## Draft and Proposed Rules

Draft records are incomplete and not implementation authority. Proposed records are ready for review but are not Approved. Agents may draft or recommend Proposed records; they cannot approve them.

## Approval Capture

Capture:

- Approver
- Approval date
- Source or context
- Decision ID and statement
- Authority metadata approved
- Follow-up actions

Acceptable approval requires clear written direction from the authorized human authority. Silence, repetition, assistant inference, agent readiness, commit, and push are not approval.

## Category Routing

| Prefix | Use For |
|---|---|
| ADR | Architecture structure and technical constraints |
| PDR | Product value, scope, UX, MVP, or roadmap |
| GDR | Governance, standards, authority, or policy |
| ODR | Operating processes, roles, and workflows |

Use the dominant consequence when categories overlap.

## Evidence and Rationale

Decision records should preserve options, rationale, rejected alternatives, consequences, risks, related assets, evidence, uncertainty, and review triggers. Do not invent evidence.

## Related Asset Updates

After approval, supersession, or retirement, update as needed:

- Decision Backlog
- Related standards and operating models
- Templates and indexes
- Session prompts and Cursor rules
- Affected project references
- Prior and successor records

Use targeted alignment, not broad unrelated rewrites.

## Agent Responsibilities

Hermes identifies candidates, separates guidance from approval, checks authority boundaries, and reviews implementation. Hephaestus implements scoped changes and reports evidence. Eunomia may later support stewardship under GDR-004 but cannot approve and is not yet instantiated.

## Prohibited Practices

- Treating backlog or working answers as decisions
- Inferring approval from silence, repetition, commit, or push
- Creating decisions without rationale
- Allowing an AI agent or Eunomia to approve
- Assigning authority without authorized approval
- Deleting superseded records
- Closing backlog items silently
- Using Exploratory Status on a Decision Record
- Resolving later-phase questions prematurely
- Reproducing the authority hierarchy owned by GDR-006

## Open Questions

- Should Olympus create a dedicated decision-promotion checklist?
- Should every Proposed decision include a formal review section?
- Should backlog statuses be standardized further?
- What additional promotion, if any, should follow RNO-002 validation of OLY-GOV-005?

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial workflow. |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory operating guidance. |
| 2026-07-27 | Hermes under explicit Founder direction | Aligned identifiers, metadata, authority, Eunomia, and phase sequencing to approved foundation sources. |
