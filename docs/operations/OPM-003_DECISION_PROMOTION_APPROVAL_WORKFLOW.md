# Decision Promotion and Approval Workflow

> **Status:** Draft / Advisory operating workflow. Not Approved, Canonical, or Governing.

## Metadata

| Field | Value |
|---|---|
| Knowledge Asset ID | OPM-003 |
| Title | Decision Promotion and Approval Workflow |
| Classification | Operating Model |
| Category | Operations / Governance |
| Status | Draft |
| Authority Level | Advisory |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Primary AI Owner | Hermes |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-05 |
| Review Cadence | As Needed |
| Related Assets | OPM-001; OPM-002; OLY-GOV-002; OLY-GOV-003; OLY-GOV-004; Decision Backlog; Decision Record Template |
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

**In scope:**

- Decision backlog items
- Working answers
- Candidate decisions from handoffs
- Founder direction with durable impact
- Draft / Proposed / Approved decision workflow
- Decision category routing: ADR / PDR / GDR / ODR
- Evidence and rationale expectations
- Supersession and retirement
- Related asset updates after decisions

**Out of scope:**

- App implementation
- Database workflow
- Voting systems
- Automated approval pipelines
- Product or architecture Tier 3 decisions
- Approving any current decision record in this pass
- Closing backlog items unless explicitly scoped

## Core Principle

> **A decision is not approved because it was discussed; it is approved only when John explicitly approves it and the record captures enough context for future work.**

Backlog items are **questions**. Working answers are **guidance**. Decision records preserve **approved or proposed choices with rationale**.

## Decision Inputs

| Input | Examples |
|---|---|
| Backlog question | OLY-DB-* item needing resolution |
| Working answer | Draft / Advisory guidance captured in OLY-GOV or OPM docs |
| Founder direction | John explicitly chooses a path |
| Handoff candidate | Session identifies decision-worthy issue |
| Asset conflict | Two assets disagree |
| Promotion need | Draft guidance needs stronger authority |
| Supersession need | Prior decision no longer fits |
| Retirement need | Decision no longer active |

## Decision Outcomes

| Outcome | Use When | Location |
|---|---|---|
| No Decision | Tactical or ephemeral choice with no future consequence | None |
| Backlog Item | Question is unresolved but may matter later | `docs/decisions/MT_OLYMPUS_DECISION_BACKLOG.md` |
| Working Answer | Direction useful now but not ready or needed for approval | Relevant OLY-GOV / OPM / asset, plus backlog note |
| Draft Decision Record | Decision record is being shaped | `docs/decisions/` with ADR / PDR / GDR / ODR |
| Proposed Decision Record | Ready for John review | `docs/decisions/` with ADR / PDR / GDR / ODR |
| Approved Decision Record | Explicit John approval captured | `docs/decisions/` with ADR / PDR / GDR / ODR |
| Superseded Decision | Replaced by newer decision | Original and replacement decision records |
| Retired Decision | No longer active, not directly replaced | Original decision record |

## Promotion Decision Tree

Use in order — stop at the first fit unless multiple routes apply:

1. **Is the issue ephemeral or purely tactical?** → No Decision.
2. **Is the question unresolved but may affect future work?** → Backlog Item.
3. **Is there useful working guidance but no need for formal approval yet?** → Working Answer.
4. **Has John selected a durable direction that affects future work?** → Draft or Proposed Decision Record.
5. **Are options, rationale, consequences, risks, and related assets clear enough for review?** → Proposed Decision Record.
6. **Has John explicitly approved the decision?** → Approved Decision Record.
7. **Does the decision replace an older decision?** → Supersede the old decision and link both records.
8. **Is the decision no longer active without direct replacement?** → Retire with rationale.
9. **If uncertain:** → Keep in backlog or Draft. Do not over-promote.

## Decision Readiness Criteria

A candidate decision is **ready for Proposed** when:

- Question or problem is clear
- Decision statement is clear
- Owner is known
- Category and prefix are selected
- Status is Draft or Proposed
- Authority level is honest
- Options considered are captured
- Rationale is captured
- Consequences are captured
- Risks and watch items are captured
- Related assets are listed
- Affected assets, templates, and READMEs are identified
- Open questions are listed
- AI Consumption and Change Impact are set
- Approval status is explicit

A decision is **ready for Approved** only when:

- **John explicitly approves it**
- Approval date and context are captured
- Approver is listed as **John S. Villasenor**
- Status and authority level are set honestly
- Follow-up updates are identified
- Supersession or retirement links are added if relevant

## Backlog Item Rules

- Backlog items use **OLY-DB-*** identifiers.
- Backlog items are **questions**, not decisions.
- Do **not** delete backlog items casually.
- A backlog item may have status: **Open**, **Working answer captured**, **Partially addressed**, **Deferred**, or **Promoted to Decision Record**.
- If promoted, link the decision record ID and keep historical context.
- If partially addressed, state what remains unresolved.
- Working answers remain **Draft / Advisory** unless promoted.

## Draft Decision Record Rules

- Use when a decision record is being shaped.
- Use `templates/decisions/DECISION_RECORD_TEMPLATE.md`.
- **Draft** does not require John approval.
- Draft may contain incomplete options or rationale.
- Draft must **not** be treated as guidance or approval.
- Draft should identify what is missing before Proposed.

## Proposed Decision Record Rules

- Use when ready for **John review**.
- **Proposed is not Approved.**
- Proposed should meet readiness criteria.
- Proposed may recommend a decision — John still decides.
- AI agents may draft Proposed records but **cannot approve** them.
- Proposed records may include explicit review questions for John.

## Approved Decision Record Rules

- Requires **explicit John approval**.
- Must capture approval date and context.
- Must identify approver.
- Must set status to **Approved**.
- Must set authority honestly: Advisory, Canonical, or Governing.
- **Approved** does not automatically mean Canonical or Governing.
- Related assets, backlog, and READMEs should be updated after approval.
- Handoffs may mention approval but are **not** the formal source of truth.

## Superseded and Retired Decision Rules

- **Superseded** decisions remain in the repository.
- Superseded decision links to its replacement.
- Replacement links to the superseded decision.
- **Retired** decisions explain why they are inactive.
- Do **not** delete decision history.
- Supersession or retirement may require README and backlog updates.

## Founder Approval Capture

Required approval capture fields:

- **Approver:** John S. Villasenor
- **Approval date**
- **Source / context of approval**
- **Decision ID**
- **Decision statement**
- **Authority level approved**
- **Follow-up actions**

**Acceptable approval sources:**

- Direct written instruction in session
- Explicit approval in repository review
- Explicit approval in handoff review
- Other clear written direction from John

**Not acceptable:**

- Silence
- Repeated discussion
- Assistant inference
- Hephaestus saying "ready"
- Hermes recommendation alone
- Implied approval from commit or push unless John explicitly says it approves the decision

## Decision Category Routing

| Prefix | Use For |
|---|---|
| ADR | Architecture structure, technical design, system constraints |
| PDR | Product scope, UX, MVP, roadmap, value decisions |
| GDR | Governance, standards, authority, policy, lifecycle |
| ODR | Operating process, roles, session workflow, stewardship |

**Rules:**

- If ambiguous, choose the **dominant consequence**.
- Governance of technical work may be **GDR**, not ADR.
- Product implications do not automatically make it PDR.
- Operating models usually route to **ODR** if a formal decision is needed.
- Do **not** create new prefixes in this workflow.

## Evidence and Rationale Requirements

Decision records should include:

- Options considered
- Rationale for chosen option
- Rejected alternatives
- Consequences
- Risks
- Related assets
- Evidence or source documents
- Known uncertainty
- Future review triggers

Evidence may include:

- Source asset references
- Handoff notes
- Research notes
- Founder direction
- Validation results
- Project outcomes

Do **not** invent evidence.

## Related Asset Update Rules

After a decision is **approved** or **superseded**, update as needed:

- Decision backlog
- Related standards
- Related operating models
- Related templates
- Directory READMEs
- Session prompts
- Cursor rules
- Affected project references
- Superseded or retired records

Make **targeted** alignment edits — do not perform broad rewrites.

## AI Agent Responsibilities

**Hermes** should:

- Identify decision candidates
- Separate working guidance from approval
- Prepare decision-promotion prompts
- Check authority boundaries
- Review Hephaestus output
- Advise John

**Hephaestus** should:

- Create or update Draft or Proposed decision records when scoped
- Update backlog and related assets when instructed
- Report changed files and evidence
- **Not** approve decisions
- **Not** infer approval

**All agents** must:

- Flag candidate decisions
- Avoid over-promotion
- Distinguish backlog, workaround, working answer, and decision
- Preserve history
- Cite source assets
- Escalate to John when authority changes

See **OPM-001** and **OPM-002** for role and capture boundaries.

## Founder Review Points

Ask **John** before:

- Moving Proposed to Approved
- Assigning Canonical or Governing authority
- Closing or promoting a backlog item
- Superseding or retiring a decision
- Resolving Tier 3 items
- Changing ID conventions
- Approving new asset categories
- Converting working guidance into binding policy

## Prohibited Practices

- Treating backlog items as decisions
- Treating working answers as approved
- Treating commit or push as approval without explicit instruction
- Creating decision records without rationale
- Approving decisions as AI agents
- Assigning Canonical or Governing authority without John approval
- Deleting superseded decision records
- Closing backlog items silently
- Using **Exploratory** status on Decision Records
- Creating decisions for trivial tactical choices
- Resolving Tier 3 questions by accident
- Rewriting unrelated assets during decision promotion

## Open Questions

- Should OPM-003 later become Canonical?
- Should Olympus create a dedicated decision-promotion checklist template?
- Should every Proposed decision require a formal review section for John?
- Should backlog statuses be standardized further?
- Should approval context cite session logs, commits, or both?
- Should **OLY-DB-009** be partially resolved by OPM-003, or remain open until agent discovery is stronger?
- Should formal **GDR** promotion of ID convention be the first real decision record?

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial Draft / Advisory Decision Promotion and Approval Workflow |
