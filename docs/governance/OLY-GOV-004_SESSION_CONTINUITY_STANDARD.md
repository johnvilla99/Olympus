# Session Continuity Standard

> **Status:** Approved / Advisory. Accepted for current Olympus use; not Canonical or Governing unless explicitly stated.

## Metadata

| Field | Value |
|---|---|
| Standard ID | OLY-GOV-004 |
| Title | Session Continuity Standard |
| Status | Approved |
| Authority Level | Advisory |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-25 |
| Review Cadence | As Needed |
| Related Assets | Foundation Brief; Knowledge Asset Model; OLY-GOV-001; OLY-GOV-002; OLY-GOV-003; OLY-GOV-005; GDR-001; ACR-001; ACR-002; Session Start Template; Session Handoff Template |
| AI Consumption | Required |
| Change Impact | Medium |

---

## Purpose

Session continuity preserves working context across AI-assisted sessions so future humans and agents can resume work safely and quickly.

Continuity should explain:

- What happened
- What changed
- What was decided versus merely discussed
- What remains open
- What evidence exists
- What risks or limitations matter
- What should happen next

Continuity is a governed practice, not a transcript dump.

## Scope

Applies to session artifacts in the Olympus repository and to any future participating project that explicitly adopts this standard.

**In scope:** session starts, session handoffs, daily logs, evidence packets, continuity artifacts, candidate knowledge, and candidate decisions.

**Out of scope:** application implementation, database schemas, automation pipelines, mandatory external-project adoption, and replacement of project-local governance.

## Definition

**Session continuity** is the governed practice of preserving enough context, evidence, decisions, open questions, and next steps for a future human or AI agent to resume work without rediscovering or reinventing prior reasoning.

Continuity is not a raw transcript and is not a substitute for formal Knowledge Assets or Decision Records.

## Session Artifact Types

| Artifact Type | Purpose | Typical Location |
|---|---|---|
| Session Start | Orient an agent at the beginning of work | Template plus filled copy in `logs/daily/` when preserved |
| Session Handoff | Preserve end-of-session state and next actions | `logs/daily/` |
| Daily Log | Chronological operational record | `logs/daily/` |
| Evidence Packet | Structured proof of changes and validation | Section within a handoff unless a future standard changes this |
| Candidate Knowledge Asset | Session-generated knowledge that may deserve promotion | Handoff or log first, then appropriate `docs/` folder |
| Candidate Decision | Open or proposed decision discovered during work | Decision Backlog or formal Decision Record |

Templates are starters, not governed artifacts.

## Session Start Rules

A session start should include:

- Date
- Agent name and role
- Project or workstream
- Required reading
- Repository state
- Active objective
- Constraints
- Open questions
- First actions
- Explicit Do Not Do items

Agents must read required sources before editing, identify the maturity and authority of relevant work, respect Founder direction and approved governance, and state uncertainty when authority is unclear.

## Session Handoff Rules

A handoff should include:

- Session date
- Agent and role
- Repository state
- Work completed
- Decisions made with honest status
- Files changed
- Commands run
- Validation and evidence
- Open questions
- Risks and watch items
- Recommended next steps
- Commit and PR status when applicable

Handoffs must distinguish decisions from observations, identify uncommitted work, avoid invented evidence, preserve failed attempts and limitations, and flag candidate Knowledge Assets and decisions.

## Daily Log Rules

- Daily logs belong under `logs/daily/`.
- Use date-oriented names when practical.
- Logs are chronological continuity aids, not automatically formal Knowledge Assets.
- Promote durable lessons, decisions, or standards to the appropriate `docs/` area.
- Keep logs concise enough to remain useful.

### AI Consumption for Resume

| Artifact | Consumption Guidance |
|---|---|
| Latest handoff for the workstream | Required |
| Relevant daily logs when a handoff exists | Recommended |
| Relevant daily logs when no handoff exists | Required |
| Formal governance and decisions | Outrank logs and handoffs for authority |

## Evidence Packet Rules

Evidence packets should include, when applicable:

- Branch and repository state
- Files changed
- Commands run
- Test or validation results
- Known limitations
- Produced artifacts
- Human QA instructions when direct validation is unavailable
- Commit or PR references

Do not invent evidence or claim validation not performed. Evidence should be proportional to the work.

## Decision Capture Rules

Apply **OLY-GOV-003**, the authoritative source for decision authority, status, approval, hierarchy, and conflict treatment.

- Not every observation is a decision.
- Unresolved decision candidates belong in the backlog unless formally promoted.
- Durable approved decisions belong in Decision Records.
- Founder approval must be explicit.
- Handoffs may mention decisions but are not the formal source of decision authority.

## Experience Capture Rules

Handoffs should flag experience worth preserving, especially surprises, failures, tradeoffs, warnings, and repeated patterns.

Capture:

- What happened
- Why it mattered
- What was learned
- How future agents should use it
- Related assets or projects
- Confidence where useful

Not every experience note becomes a formal asset. Promote durable experience under OLY-GOV-002 and OPM-002.

## Agent Capability and Limitation Rules

Agents must not claim capabilities they do not have. They must distinguish inspection, recommendation, implementation, validation, and human QA.

When validation is unavailable, state why and provide clear human-validation steps.

## Source Reading Rules

- Required reading must be explicit.
- Prefer Governing, Canonical, and Approved assets over lower-authority context.
- Check Status and Authority Level before relying on a source.
- Apply OLY-GOV-005 for authority-aware discovery.
- Cite or reference material sources.
- Flag conflicts rather than silently resolving them.

## Resume Rules

Resume from:

- Relevant governance and Approved decisions
- Latest handoff for the workstream
- Relevant daily logs
- Current git state
- Decision backlog
- Active objective and constraints

Verify repository state before acting. Treat handoff claims as continuity guidance and verify them against observable state and formal assets.

## Promotion Rules

Continuity artifacts may produce Knowledge Assets, Decision Records, Lessons Learned, governance updates, or operating-model changes.

- Promote only when future value justifies maintenance cost.
- Do not promote raw logs wholesale.
- Preserve links to the session source when useful.
- Update related indexes and backlog entries.
- Apply OLY-GOV-002 and OLY-GOV-003.

## Placement and Naming Rules

| Content | Location |
|---|---|
| Session templates | `templates/sessions/` |
| Filled Olympus handoffs | `logs/daily/` unless promoted |
| Project-specific handoffs | Relevant project repository by default |
| Daily logs | `logs/daily/` |
| Durable operating models | `docs/operations/` |
| Decision records | `docs/decisions/` |
| Lessons learned | `docs/lessons/` |
| Governance standards | `docs/governance/` |

Formal asset identifiers follow GDR-001.

## AI Consumption Rules

Agents must:

- Read continuity artifacts when resuming related work
- Distinguish handoff claims from formal decisions
- Verify current repository state
- Cite formal sources when recommendations depend on them
- Identify candidate knowledge worth promotion review
- Respect Status and Authority Level
- Avoid re-litigating settled decisions without new evidence or Founder direction

## Prohibited Practices

- Dumping raw transcripts as continuity
- Treating handoffs as approved decisions
- Hiding failed attempts or limitations
- Omitting uncommitted-work state
- Claiming tests or validation not performed
- Creating bloated logs nobody will use
- Requiring evidence an agent cannot produce
- Silently resolving conflicts
- Replacing formal decisions with chat or handoff summaries
- Turning every note into a formal Knowledge Asset
- Promoting exploratory ideas without Founder approval
- Duplicating decision-authority rules already owned by OLY-GOV-003

## Exceptions

Exceptions require Founder approval and must be documented in the affected handoff, log, decision, or governance asset.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial draft |
| 2026-07-05 | John S. Villasenor | Added handoff placement, daily-log consumption, and evidence-packet guidance |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory guidance; aligned decision authority to OLY-GOV-003 and identifiers to GDR-001 |