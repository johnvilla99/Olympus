# Decision Record Standard

> **Status:** Approved / Governing. This standard controls Olympus decision authority, hierarchy, lifecycle, approval, and backlog discipline.

## Metadata

| Field | Value |
|---|---|
| Standard ID | OLY-GOV-003 |
| Title | Decision Record Standard |
| Status | Approved |
| Authority Level | Governing |
| Owner | John S. Villasenor |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-25 |
| Review Cadence | As Needed |
| Related Assets | Foundation Brief; Knowledge Asset Model; Governance Starter; Repository Standard; Knowledge Asset Standard; Decision Backlog; GDR-001; ACR-001; ACR-002 |

---

## Purpose

Make decisions **trustworthy, traceable, reviewable, and safe** for future humans and AI agents to consume.

Decision records preserve not only **what** was decided, but also:

- **Why** it mattered
- **What options** were considered
- **What was rejected**
- **Who** owned and approved the decision
- **What consequences and risks** remain
- **What future work** is affected

This standard prevents exploratory ideas, assistant suggestions, conversation fragments, or temporary working assumptions from being treated as approved decisions.

## Scope

Applies to **formal decision records** and the **decision backlog** in the Olympus repository during the governed knowledge foundation phase.

**In scope:**

- Decision identification and categories
- Decision metadata and statuses
- Approval and review rules
- Backlog promotion rules
- Supersession and retirement
- AI consumption of decisions
- Decision authority and hierarchy

**Out of scope:**

- Application implementation, database schema, or UI design
- Voting workflows or automated approval pipelines
- External project repository decision standards unless explicitly adopted
- Automatic promotion of any backlog item or concept to **Approved** status

## Definition of a Decision Record

A **Decision Record** is a formal Knowledge Asset that captures an approved, proposed, superseded, or retired decision and the rationale necessary for future reasoning.

A decision record should answer:

- **What** decision was made?
- **Why** was it made?
- **Who** made or approved it?
- **What alternatives** were considered?
- **What consequences** followed?
- **What risks** remain?
- **What assets or projects** are affected?
- **What would cause** this decision to be revisited?

Decision records belong in `docs/decisions/` and should align with OLY-GOV-002.

## What Qualifies as a Decision

Examples of matters that may qualify for a formal decision record when ready:

- Approving a governance standard for repository use
- Choosing the official Knowledge Asset or decision ID convention
- Defining Mnemosyne as the memory layer when promoted from exploration
- Defining Metis as the judgment layer when promoted from exploration
- Selecting which projects participate first
- Approving required repository exposure for participating projects
- Adopting a product MVP scope or roadmap direction

A matter qualifies when the decision will affect future work, multiple options existed, and preserving rationale prevents rediscovery or re-litigation.

## What Does Not Qualify as a Decision

Examples of content that is **not** a decision record:

- Exploratory discussion or brainstorming
- Brainstormed options not yet chosen
- Assistant recommendations not accepted by the Founder
- Temporary working assumptions for a single session
- Open questions in the decision backlog
- Implementation details not yet reviewed or approved
- Unresolved conflicts between assets
- Notes captured for future consideration
- Architectural Concept Records, which are exploratory by default

## Decision Record Categories

The official identifier convention is defined by **GDR-001**, the Approved / Canonical Olympus ID Convention.

| Prefix | Category | Purpose | Typical Location |
|---|---|---|---|
| **ADR** | Architecture Decision Record | Technical architecture and system structure decisions | `docs/decisions/` |
| **PDR** | Product Decision Record | Product scope, UX, MVP, roadmap, or user value decisions | `docs/decisions/` |
| **GDR** | Governance Decision Record | Governance, standards, process, authority, or stewardship decisions | `docs/decisions/` |
| **ODR** | Operating Decision Record | Session workflow, agent operating model, project participation, or operational process decisions | `docs/decisions/` |

**Important distinctions:**

- **ACR** means Architectural Concept Record. It is exploratory by default and is not a decision record.
- ACRs may inform decisions but do not become decisions unless promoted through the decision process.
- Decision prefixes and numbering are governed by GDR-001.

## Decision ID Rules

Decision identifiers must conform to **GDR-001**.

- IDs are stable once assigned.
- Use sequential numbering within each approved prefix.
- Do not reuse retired or superseded IDs.
- Do not rename decision files casually; record supersession instead.
- If a decision is superseded, create a new record and link both records.
- Filename should match the Decision ID where practical.

## Decision Record Status Values

```text
Draft
Proposed
Approved
Superseded
Retired
```

Decision Records do **not** use `Exploratory`.

## Required Decision Metadata

| Field | Meaning |
|---|---|
| **Decision ID** | Stable identifier governed by GDR-001 |
| **Title** | Human-readable decision title |
| **Classification** | Decision Record |
| **Decision Category** | Architecture, Product, Governance, or Operating |
| **Status** | Draft, Proposed, Approved, Superseded, or Retired |
| **Authority Level** | Advisory, Canonical, or Governing as applicable |
| **Owner** | Human accountable for maintaining the record |
| **Decider / Approver** | Person or authority who approved the decision |
| **Created On** | Date the record was created |
| **Decided On** | Date the decision was approved, if approved |
| **Last Updated** | Latest material update |
| **Review Cadence** | Expected review rhythm |
| **Related Assets** | Source concepts, standards, project docs, or prior decisions |
| **Supersedes** | Prior decision IDs replaced by this record |
| **Superseded By** | Later decision ID that replaced this record, if applicable |
| **AI Consumption** | Required, Recommended, Optional, or Restricted |
| **Change Impact** | Low, Medium, or High |

Required content sections: Decision, Context, Options Considered, Rationale, Consequences, Risks, Follow-up Actions, Supersedes / Superseded By, and Change History.

## Decision Status Model

| Status | Meaning |
|---|---|
| **Draft** | Decision record is being shaped; not ready for review |
| **Proposed** | Decision is ready for review but not yet approved |
| **Approved** | Decision is accepted as current guidance and requires explicit Founder approval during the foundation phase |
| **Superseded** | Decision has been replaced by a later decision and is preserved with a link to its replacement |
| **Retired** | Decision is no longer active and is preserved for historical context with rationale |

**Clarifications:**

- A decision backlog item is a question, not a decision.
- Exploratory concept records are not decisions.
- Assistant suggestions are not decisions unless accepted by the Founder and recorded.
- Approved status and Authority Level are distinct.
- Canonical or Governing authority requires explicit Founder approval.

## Decision Authority Rules

This section is the authoritative Olympus source for decision authority and hierarchy. Operating models and supporting documents must reference this section rather than restating it.

Decision hierarchy for Olympus, highest first:

1. **Explicit current Founder direction** within the Founder’s authority
2. **Governing assets**
3. **Canonical assets**
4. **Approved decision records and Approved / Advisory governance standards**
5. **Approved product, architecture, and operating definitions**
6. **Proposed assets and decisions**, for review guidance only
7. **Exploratory and Informational assets**
8. **Continuity artifacts and conversation context**
9. **Assistant inference or general knowledge**

**Application rules:**

- Status and Authority Level must be evaluated together.
- A more specific applicable asset normally controls over a general asset at the same authority level.
- A newer asset controls only when it explicitly supersedes or replaces older guidance.
- Approved decisions outrank exploratory ACRs and backlog items.
- Continuity artifacts provide context but do not override formal assets.
- Assistant recommendations have no decision authority unless accepted by the Founder and recorded.
- Conflicts must be surfaced rather than silently resolved.
- Durable Founder direction should be captured in the appropriate formal asset.

This standard is Approved / Governing. It defines the controlling Olympus rules for decision authority, hierarchy, approval, and lifecycle; it does not itself approve individual decisions.

## Decision Creation Rules

Create a decision record when:

- The decision will affect future work
- Future agents may need to know what was decided
- Multiple options existed
- The decision affects standards, architecture, product scope, or operations
- Failing to preserve rationale could cause rediscovery or re-litigation

**Process:**

- Use the Decision Record template when possible.
- Copy into `docs/decisions/` with a stable Decision ID.
- Set honest initial status, normally Draft or Proposed.
- Include the decision, context, options, rationale, consequences, risks, affected assets, follow-up actions, supersession information, and change history.
- Do not create decision bureaucracy for trivial matters.

## Decision Review and Approval

Preferred path:

```text
Draft → Proposed → Approved
```

**Approval rules:**

- Only John S. Villasenor / Founder may approve Approved status and Canonical or Governing authority during the foundation phase.
- AI agents may recommend or draft but cannot approve.
- Approval must be explicit and cannot be inferred from silence, repeated discussion, commit, or push.
- Capture approval date, context, and Decider / Approver in the record.
- Approved does not automatically mean Canonical or Governing.

## Decision Backlog Rules

The decision backlog lives at `docs/decisions/MT_OLYMPUS_DECISION_BACKLOG.md`.

- Open questions belong in the backlog before they become decisions.
- Backlog items prevent exploratory questions from becoming accidental architecture.
- Promote a backlog item only when the decision will unblock meaningful work and consequences are understood.
- When promoted, update the backlog with the Decision ID and status.
- Preserve backlog history.
- OLY-DB identifiers are not decision IDs.

## Decision Supersession and Retirement

- Superseded decisions remain in the repository for historical continuity.
- New decisions must link to decisions they supersede.
- Superseded decisions must link to their replacement.
- Retired decisions must explain why they are inactive.
- Historical rationale must not be erased.

## Relationship and Citation Rules

Decision records should cite or link source assets and related decisions. If a decision resolves an open backlog question, link both the backlog item and the decision record.

Recognized relationship types include `informs`, `supersedes`, `contradicts`, `depends_on`, `implements`, `references`, `replaces`, and `related_to`.

## AI Consumption Rules

AI agents must:

- Treat backlog items as questions, not decisions
- Distinguish Proposed from Approved decisions
- Prefer Approved decisions over exploratory concept records
- Respect Authority Level
- Cite decision records when recommending action based on a decision
- Flag conflicts
- Never infer approval

## Founder Direction Rules

- Founder direction has highest authority within the Founder’s authority.
- Durable Founder direction should be captured when it will affect future work beyond the current session.
- Not every Founder comment requires a decision record; proportionality matters.
- If Founder direction conflicts with existing records, flag the conflict and update, supersede, or revise the appropriate asset.

## Prohibited Practices

- Treating ACRs as approved decisions
- Treating backlog items as decisions
- Treating assistant suggestions as decisions
- Inferring approval from silence, conversation, commit, or push
- Creating decision records without rationale
- Reusing decision IDs
- Deleting superseded decisions
- Promoting decisions without Founder approval
- Creating decision bureaucracy for trivial tactical choices
- Assigning Exploratory status to a Decision Record
- Restating this authority hierarchy in operating documents when a reference is sufficient

## Exceptions

Exceptions require Founder approval and should be documented in the affected decision record, backlog entry, or governance standard Change History.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial draft |
| 2026-07-05 | John S. Villasenor | Added decision prefixes, decision-only status model, and Founder-only approval guidance |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory guidance; established OLY-GOV-003 as the authoritative source for decision authority and hierarchy; aligned identifiers to GDR-001 |
| 2026-07-25 | John S. Villasenor | Promoted to Governing authority as the controlling decision authority, hierarchy, lifecycle, approval, and backlog standard |