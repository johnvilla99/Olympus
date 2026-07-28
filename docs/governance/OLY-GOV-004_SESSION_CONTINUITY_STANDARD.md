# Session Continuity Standard

> **Status:** Approved / Advisory. Accepted for current Olympus use; not Canonical or Governing.

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
| Last Updated | 2026-07-27 |
| Review Cadence | As Needed |
| Related Assets | GDR-005; GDR-006; GDR-007; OLY-GOV-001; OLY-GOV-002; OLY-GOV-003; OLY-GOV-005; OPM-004 |
| AI Consumption | Required |
| Change Impact | Medium |

---

## Purpose

Session continuity preserves enough context, evidence, decisions, open questions, limitations, and next steps for a future human or AI agent to resume work safely without rediscovering prior reasoning.

Continuity is a governed practice, not a transcript dump and not a substitute for formal Knowledge Assets or decisions.

## Artifact Types

| Artifact | Purpose | Typical Location |
|---|---|---|
| Session Start | Orient an agent before work | Template plus filled copies in `logs/daily/` |
| Session Handoff | Preserve end-of-session state | `logs/daily/` unless promoted |
| Daily Log | Chronological continuity | `logs/daily/YYYY-MM-DD.md` |
| Evidence Packet | Record changes and validation | Section within a handoff or gate packet |
| Candidate Knowledge | Identify possible promotion | Handoff or log first |
| Candidate Decision | Track unresolved or proposed choice | Decision Backlog or formal decision record |

## Session Start Rules

A session start identifies date, agent role, workstream, required reading, repository state, active objective, constraints, open questions, first actions, and explicit do-not-do boundaries.

Agents must:

- Verify the active repository under GDR-007 and current branch state.
- Read required sources before editing.
- Evaluate metadata under GDR-005 and authority under GDR-006.
- Respect the current OPM-004 phase and Founder gate.
- State uncertainty and conflicts.

## Session Handoff Rules

A handoff records repository state, work completed, decisions versus observations, files changed, commands or actions performed, validation, limitations, open questions, risks, next steps, and commit/PR status.

Handoffs must not claim validation that was not performed, hide failed attempts, or treat uncommitted work as published.

## Daily Logs

Daily logs are concise chronological aids. They are not automatically formal Knowledge Assets. Durable decisions, lessons, or operating guidance should be promoted through the appropriate workflow.

## Evidence Packets

Evidence should be proportional and may include repository state, files changed, commands/actions, test or validation results, limitations, produced artifacts, QA notes, and commit/PR references.

Do not invent evidence. When a capability is unavailable, state the limitation and provide clear human validation steps.

## Decision Capture

- Session observations are not automatically decisions.
- Unresolved consequential questions belong in the Decision Backlog.
- Durable decisions belong in formal records under OLY-GOV-003.
- Approval and authority changes follow GDR-005, GDR-006, and OPM-003.
- Eunomia and agents may recommend but may not approve.

## Experience Capture

Handoffs should flag meaningful surprises, failures, tradeoffs, warnings, and patterns. Capture what happened, why it mattered, what was learned, future guidance, related assets, and confidence where useful.

Not every experience becomes a formal asset.

## Source Reading and Resume Rules

Resume from:

1. Applicable Governing, Canonical, and Approved sources under GDR-006.
2. Latest handoff for the workstream.
3. Relevant daily logs.
4. Observable repository and operational state.

Continuity artifacts explain recent work but do not override formal authority. Verify old handoff claims against current repository state.

## Promotion Rules

Promote only when future decision, reasoning, continuity, or execution value justifies maintenance. Preserve links to the source session when useful and update indexes, backlog items, and Related Assets.

## Placement

- Session templates → `templates/sessions/`
- Olympus handoffs and daily logs → `logs/daily/`
- Project-specific handoffs → relevant project repository
- Durable operating models → `docs/operations/`
- Decisions → `docs/decisions/`
- Lessons → `docs/lessons/`
- Governance → `docs/governance/`

## Prohibited Practices

- Raw transcript dumps
- Treating handoffs as approved decisions
- Hiding failed attempts or limitations
- Omitting uncommitted-work state
- Claiming tests or validation not performed
- Bloated continuity artifacts with no resume value
- Silently resolving conflicts
- Rewriting historical handoffs solely to modernize terminology
- Promoting session ideas without approval

## Exceptions

Exception authority and approval follow GDR-006 and OPM-003. Record approved exceptions in the affected continuity artifact or governance source.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial continuity standard. |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory guidance. |
| 2026-07-27 | Hermes under explicit Founder direction | Aligned continuity authority and repository references to GDR-005 through GDR-007 while preserving historical artifacts. |
