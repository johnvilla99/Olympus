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
| Last Updated | 2026-07-25 |
| Review Cadence | As Needed |
| Related Assets | OPM-001; OPM-002; OLY-GOV-002; OLY-GOV-003; OLY-GOV-004; OLY-GOV-005; GDR-001; Decision Backlog; Decision Record Template |
| AI Consumption | Recommended |
| Change Impact | Medium |

---

## Purpose

OPM-003 defines how Olympus promotes **questions, working answers, and captured direction** into formal decision records.

This workflow prevents:

- Backlog questions becoming accidental decisions
- Working answers being mistaken for Approved decisions
- Founder approval being inferred
- Decision records being created without rationale
- Decisions lacking consequences, risks, or related asset updates
- Superseded decisions being erased
- AI agents approving decisions

## Scope

**In scope:** backlog questions, working answers, candidate decisions, Founder direction with durable impact, Draft / Proposed / Approved workflow, decision-category routing, rationale and evidence expectations, supersession, retirement, and related-asset updates.

**Out of scope:** application implementation, databases, voting systems, automated approvals, and product or architecture Tier 3 decisions.

## Governing References

- **OLY-GOV-003** owns decision authority, status, approval, hierarchy, and conflict rules.
- **GDR-001** owns the Olympus ID convention.
- **OLY-GOV-002** owns Knowledge Asset metadata and lifecycle guidance.
- **OPM-003 does not restate or override those rules.** It defines the operating workflow used to apply them.

## Core Principle

> **A decision is not approved because it was discussed; it is approved only when John explicitly approves it and the record captures enough context for future work.**

Backlog items are questions. Working answers are guidance. Decision records preserve proposed or approved choices with rationale.

## Decision Inputs

| Input | Examples |
|---|---|
| Backlog question | OLY-DB item needing resolution |
| Working answer | Guidance captured in an OLY-GOV, OPM, or other asset |
| Founder direction | John explicitly chooses a durable path |
| Handoff candidate | Session identifies a decision-worthy issue |
| Asset conflict | Two assets disagree |
| Promotion need | Guidance needs stronger authority |
| Supersession need | Prior decision no longer fits |
| Retirement need | Decision is no longer active |

## Decision Outcomes

| Outcome | Use When | Location |
|---|---|---|
| No Decision | Tactical or ephemeral choice with no future consequence | None |
| Backlog Item | Question is unresolved but may matter later | Decision Backlog |
| Working Answer | Direction is useful but does not require formal approval yet | Relevant asset plus backlog note |
| Draft Decision Record | Record is being shaped | `docs/decisions/` |
| Proposed Decision Record | Ready for John review | `docs/decisions/` |
| Approved Decision Record | Explicit John approval captured | `docs/decisions/` |
| Superseded Decision | Replaced by a newer decision | Original and replacement records |
| Retired Decision | No longer active, not directly replaced | Original record |

## Promotion Decision Tree

1. Is the issue ephemeral or purely tactical? → No Decision.
2. Is it unresolved but potentially consequential? → Backlog Item.
3. Is there useful current guidance without a need for formal approval? → Working Answer.
4. Has John selected a durable direction? → Draft or Proposed Decision Record.
5. Are options, rationale, consequences, risks, and related assets clear enough? → Proposed.
6. Has John explicitly approved it? → Approved.
7. Does it replace an older decision? → Supersede and link both records.
8. Is it inactive without a direct replacement? → Retire with rationale.
9. If uncertain, keep it in the backlog or Draft. Do not over-promote.

## Decision Readiness Criteria

A candidate is ready for Proposed when the problem, decision statement, owner, category, options, rationale, consequences, risks, related assets, follow-up actions, AI Consumption, Change Impact, and approval status are clear.

A decision is ready for Approved only when:

- John explicitly approves it
- Approval date and context are captured
- John is identified as Approver
- Status and Authority Level are set honestly
- Follow-up updates are identified
- Supersession or retirement links are included when relevant

## Backlog Rules

- Backlog items use `OLY-DB-*` identifiers.
- They are questions, not decisions.
- Preserve backlog history.
- If promoted, link the Decision Record and update status.
- If partially addressed, state what remains open.

## Draft, Proposed, and Approved Rules

**Draft:** being shaped; not ready for review and not authority.

**Proposed:** ready for John review; not approved.

**Approved:** requires explicit John approval and captured approval evidence. Approved status does not automatically confer Canonical or Governing authority.

## Founder Approval Capture

Capture:

- Approver
- Approval date
- Approval source or context
- Decision ID
- Decision statement
- Approved Authority Level
- Follow-up actions

Silence, repeated discussion, assistant inference, commit, or push are not approval.

## Decision Category Routing

Use the prefixes defined by GDR-001:

| Prefix | Use For |
|---|---|
| ADR | Architecture structure, technical design, system constraints |
| PDR | Product scope, UX, MVP, roadmap, value decisions |
| GDR | Governance, standards, authority, policy, lifecycle |
| ODR | Operating process, roles, session workflow, stewardship |

Choose the category by dominant consequence. Do not invent new prefixes without governance review and Founder approval.

## Evidence and Rationale

Decision records should include options considered, rationale, rejected alternatives, consequences, risks, related assets, evidence, uncertainty, and future review triggers. Do not invent evidence.

## Related Asset Updates

After approval or supersession, update as needed:

- Decision backlog
- Related standards and operating models
- Templates and READMEs
- Session prompts and Cursor rules
- Affected project references
- Superseded or retired records

Make targeted alignment edits rather than broad rewrites.

## AI Agent Responsibilities

**Hermes:** identify decision candidates, separate working guidance from approval, prepare promotion work, check authority boundaries, review outputs, and advise John.

**Hephaestus:** create or update Draft or Proposed records when scoped, update related assets when instructed, report evidence, and never approve or infer approval.

All agents must distinguish backlog, working answer, proposed decision, approved decision, and superseded guidance.

## Founder Review Points

Ask John before moving Proposed to Approved, assigning Canonical or Governing authority, closing or promoting a backlog item, superseding or retiring a decision, resolving Tier 3 items, changing ID conventions, or creating new asset categories.

## Prohibited Practices

- Treating backlog items as decisions
- Treating working answers as approved
- Treating commit or push as approval
- Creating decisions without rationale
- AI agents approving decisions
- Assigning Canonical or Governing authority without John approval
- Deleting superseded records
- Closing backlog items silently
- Using Exploratory status on Decision Records
- Creating decisions for trivial tactical choices
- Resolving Tier 3 questions accidentally
- Duplicating authority rules already owned by OLY-GOV-003

## Open Questions

- Should OPM-003 later become Canonical?
- Should Olympus create a dedicated decision-promotion checklist?
- Should every Proposed decision include a formal Founder review section?
- Should approval context cite session logs, commits, or both?

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial Draft / Advisory workflow |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory workflow; aligned authority to OLY-GOV-003 and identifiers to GDR-001 |