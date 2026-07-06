# Decision Record Standard

> **Status:** Draft — advisory guidance, not approved or governing policy.

## Metadata

| Field | Value |
|---|---|
| Standard ID | OLY-GOV-003 |
| Title | Decision Record Standard |
| Status | Draft |
| Authority Level | Advisory |
| Owner | John S. Villasenor |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-05 |
| Review Cadence | As Needed |
| Related Assets | Foundation Brief; Knowledge Asset Model; Governance Starter; Repository Standard; Knowledge Asset Standard; Decision Backlog; ACR-001; ACR-002 |

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

**Out of scope:**

- Application implementation, database schema, or UI design
- Voting workflows or automated approval pipelines
- External project repository decision standards (unless explicitly adopted)
- Automatic promotion of any existing backlog item or concept to **Approved** status

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

Decision records belong in `docs/decisions/` and should align with `docs/governance/OLY-GOV-002_KNOWLEDGE_ASSET_STANDARD.md` (OLY-GOV-002).

## What Qualifies as a Decision

Examples of matters that may qualify for a formal decision record when ready:

- Approving a governance standard for repository use
- Choosing the official Knowledge Asset or decision ID convention
- Defining Mnemosyne as the memory layer (when promoted from exploration)
- Defining Metis as the judgment layer (when promoted from exploration)
- Selecting which projects participate first
- Choosing whether Research remains cross-cutting or becomes a formal Muse
- Approving required repository exposure for participating projects
- Adopting a product MVP scope or roadmap direction

A matter qualifies when the decision will affect future work, multiple options existed, and preserving rationale prevents rediscovery or re-litigation.

## What Does Not Qualify as a Decision

Examples of content that is **not** a decision record:

- Exploratory discussion or brainstorming
- Brainstormed options not yet chosen
- Assistant recommendations not accepted by the Founder
- Temporary working assumptions for a single session
- **Open questions** in the decision backlog (`MT_OLYMPUS_DECISION_BACKLOG.md`)
- Implementation details not yet reviewed or approved
- Unresolved conflicts between assets
- Notes captured for future consideration
- **Architectural Concept Records (ACRs)** — exploratory by default unless promoted through the decision process

## Decision Record Categories

| Prefix | Category | Purpose | Typical Location |
|---|---|---|---|
| **ADR** | Architecture Decision Record | Technical architecture and system structure decisions | `docs/decisions/` |
| **PDR** | Product Decision Record | Product scope, UX, MVP, roadmap, or user value decisions | `docs/decisions/` |
| **GDR** | Governance Decision Record | Governance, standards, process, authority, or stewardship decisions | `docs/decisions/` |
| **ODR** | Operating Decision Record | Session workflow, agent operating model, project participation, or operational process decisions | `docs/decisions/` |

**Important distinctions:**

- **ACR** means **Architectural Concept Record** — lives in `docs/concepts/`, exploratory by default, **not** a decision record.
- ACRs may inform decisions but do not become decisions unless promoted through Draft → Proposed → Approved.
- ADR/PDR/GDR/ODR prefix convention is **Draft / Advisory working guidance** (Founder-aligned, 2026-07-05) — not Canonical or Governing until formally promoted.

## Decision ID Rules

**Draft / Advisory decision prefix convention** (Founder-aligned, 2026-07-05):

```text
ADR-001
PDR-001
GDR-001
ODR-001
```

**Rules:**

- IDs must be **stable** once assigned.
- Use **sequential numbering** within each prefix.
- Do **not reuse** retired or superseded IDs.
- Do **not rename** decision files casually — record supersession instead.
- If a decision is superseded, **create a new record** and link both records.
- Filename should match Decision ID where practical (e.g. `GDR-001_OFFICIAL_ID_CONVENTION.md`).
- This convention aligns with the Knowledge Asset ID Convention in OLY-GOV-002. Remains **Draft / Advisory** until formally promoted via decision record.

**Decision Record status values (only these):**

```text
Draft
Proposed
Approved
Superseded
Retired
```

Decision Records do **not** use `Exploratory`. Exploratory belongs to concept records, research notes, early knowledge assets, or backlog items — not decision records.

## Required Decision Metadata

| Field | Meaning |
|---|---|
| **Decision ID** | Stable identifier (e.g. GDR-001). |
| **Title** | Human-readable decision title. |
| **Classification** | Decision Record (always). |
| **Decision Category** | Architecture, Product, Governance, or Operating — maps to ADR/PDR/GDR/ODR prefix. |
| **Status** | Draft, Proposed, Approved, Superseded, or Retired — see Decision Status Model. |
| **Authority Level** | Advisory, Canonical, or Governing as applicable (not all decisions are Governing). |
| **Owner** | Human accountable for maintaining the record. |
| **Decider / Approver** | Person or authority who approved the decision (typically Founder during foundation phase). |
| **Created On** | Date the record was created. |
| **Decided On** | Date the decision was approved, if approved. |
| **Last Updated** | Latest material update. |
| **Review Cadence** | Expected review rhythm. |
| **Related Assets** | Source concepts, standards, project docs, or prior decisions. |
| **Supersedes** | Prior decision IDs replaced by this record. |
| **Superseded By** | Later decision ID that replaced this record, if applicable. |
| **AI Consumption** | Required, Recommended, Optional, or Restricted. |
| **Change Impact** | Low, Medium, or High. |

**Required content sections** (from `templates/decisions/DECISION_RECORD_TEMPLATE.md`): Decision, Context, Options Considered, Rationale, Consequences, Risks, Follow-up Actions, Supersedes / Superseded By, Change History.

## Decision Status Model

| Status | Meaning |
|---|---|
| **Draft** | Decision record is being shaped; not ready for review. |
| **Proposed** | Decision is ready for review but **not yet approved**. |
| **Approved** | Decision is accepted as current guidance. Requires Founder approval during foundation phase. |
| **Superseded** | Decision has been replaced by a later decision. Preserved with link to replacement. |
| **Retired** | Decision is no longer active. Preserved for historical context with rationale. |

**Clarifications:**

- A **decision backlog item** is a **question**, not a decision.
- **Exploratory concept records (ACRs)** are **not** decisions.
- **Assistant suggestions** are **not** decisions unless accepted by Founder and recorded.
- Decision Records use **Draft, Proposed, Approved, Superseded, Retired only** — never Exploratory.
- **Approved** decisions may carry **Advisory**, **Canonical**, or **Governing** authority depending on subject — Approved status and authority level are related but distinct.
- **Canonical** or **Governing** authority level requires explicit **Founder approval**, even when status is Approved.

## Decision Authority Rules

Decision hierarchy for Olympus (aligned with Governance Starter):

1. **Founder direction**
2. Governance charter and standards
3. Canonical knowledge assets
4. **Approved decision records**
5. Product or architecture definitions
6. Exploratory concept records
7. Conversation context
8. Assistant inference

**Rules:**

- **Founder direction** can create or override decisions; durable Founder direction should be captured in a decision record when it will affect future work.
- **Approved decision records** outrank exploratory ACRs and backlog items.
- **Assistant recommendations** have **no decision authority** unless accepted by the Founder and recorded.
- **Conflicts** between decisions, standards, or concepts should be **flagged**, not silently resolved.
- This standard is **Draft / Advisory** — it does not itself approve any decision.

## Decision Creation Rules

Create a decision record when:

- The decision will **affect future work**
- Future agents may need to know **what was decided**
- **Multiple options** existed
- The decision affects **standards, architecture, product scope, or operations**
- Failing to preserve rationale could cause **rediscovery or re-litigation**

**Process:**

- Use `templates/decisions/DECISION_RECORD_TEMPLATE.md` when possible.
- Copy into `docs/decisions/` with a stable Decision ID.
- Set honest initial status (**Draft** or **Proposed**).
- Include: decision statement, context, options considered, rationale, consequences, risks, affected assets/projects, follow-up actions, supersession information, and change history.
- Do **not** create decision bureaucracy for trivial matters that do not affect future work.

## Decision Review and Approval

**Preferred path:**

```text
Draft → Proposed → Approved
```

**Approval rules (foundation phase):**

- **Only John S. Villasenor / Founder** may approve **Approved** status (and **Canonical** or **Governing** authority levels).
- **Curator** remains proposed — may recommend promotion but **cannot approve** during foundation phase.
- **AI agents** may recommend or draft but **cannot approve**.
- Approval must be **explicit** — not inferred from silence, repeated discussion, or assistant assertion.
- If approval is given in conversation, capture **date**, **source/context**, and **Decider / Approver** in the decision record.
- **Governance decisions** may require updating related standards or README files as follow-up actions.
- **Approved** does not automatically mean **Canonical** or **Governing** — set authority level explicitly and honestly.

## Decision Backlog Rules

The decision backlog lives at `docs/decisions/MT_OLYMPUS_DECISION_BACKLOG.md`.

**Rules:**

- **Open questions** belong in the backlog **before** they become decisions.
- Backlog items prevent exploratory questions from becoming **accidental architecture**.
- Promote a backlog item to a decision record only when the decision will **unblock meaningful work** and **consequences are understood**.
- When promoted, **update the backlog** with the new Decision ID and status (e.g. Promoted → GDR-001).
- Do **not delete** backlog history casually — preserve the question and promotion trail.
- Backlog IDs (OLY-DB-*) are **not** decision IDs — they track open questions only.

## Decision Supersession and Retirement

- **Superseded** decisions remain in the repository for historical continuity.
- New decisions must **link to decisions they supersede** (Supersedes field).
- Superseded decisions must **link to their replacement** (Superseded By field).
- **Retired** decisions must explain **why** they are no longer active.
- **Historical rationale must not be erased** — supersession adds clarity; it does not delete the story of why the earlier decision existed.

## Relationship and Citation Rules

- Decision records should **cite or link** source assets (ACRs, standards, research) and related decisions.
- Identify **affected standards**, concepts, projects, and Muse domains where relevant.
- Exploratory relationship types (no graph implementation in this pass):

| Type | Meaning |
|---|---|
| `informs` | Source provides context for the decision |
| `supersedes` | Decision replaces a prior decision or guidance |
| `contradicts` | Decision conflicts with another record — flag for resolution |
| `depends_on` | Decision requires another asset to be understood |
| `implements` | Decision puts an approved standard or concept into effect |
| `references` | Decision cites another asset |
| `replaces` | Decision is the successor to prior guidance |
| `related_to` | General association |

- If a decision **resolves an open backlog question**, link both the **backlog item (OLY-DB-*)** and the **decision record**.

## AI Consumption Rules

AI agents **must**:

- Treat **backlog items as questions**, not decisions
- **Distinguish Proposed from Approved** decisions
- **Prefer Approved decisions** over exploratory concept records
- **Respect authority level** on each decision record
- **Cite decision records** when recommending action based on a decision
- **Flag conflicts** between decisions or between decisions and standards
- **Never infer approval** from repeated discussion alone

**AI Consumption values:**

| Value | Meaning |
|---|---|
| **Required** | Agents should consult this decision when working in its domain. |
| **Recommended** | Agents should reference when relevant. |
| **Optional** | Agents may consult for additional context. |
| **Restricted** | Agents must not rely on or surface without explicit permission. |

## Founder Direction Rules

- **Founder direction has highest authority** in the Olympus ecosystem.
- **Durable Founder direction** should be captured as a decision record when it will affect future work beyond the current session.
- **Not every Founder comment** requires a decision record — preserve the ability to move quickly without turning every sentence into governance paperwork.
- When Founder direction is given informally but has durable impact, a **lightweight decision record** or explicit note in an existing record is sufficient — proportionality matters.
- If Founder direction **conflicts** with existing records, **flag the conflict** and recommend a decision update, supersession, or standard revision.

## Prohibited Practices

- Treating **ACRs** as approved decisions
- Treating **backlog items** as decisions
- Treating **assistant suggestions** as decisions
- **Inferring approval from silence** or conversational repetition
- Creating decision records **without rationale** or options considered
- **Reusing** decision IDs
- **Deleting** superseded decisions
- **Promoting decisions** to Approved without Founder approval
- Creating **decision bureaucracy** for trivial matters with no future impact
- Assigning **Approved** status to exploratory concept records without the decision process
- Assigning **Exploratory** status to a Decision Record

## Exceptions

- Exceptions require **Founder approval** only.
- Document exceptions in the affected decision record, backlog entry, or governance standard Change History.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial draft (OLY-GOV-003) |
| 2026-07-05 | John S. Villasenor | Tier 1/2 working answers: ADR/PDR/GDR/ODR prefixes, decision-only status model, Founder-only approval |
