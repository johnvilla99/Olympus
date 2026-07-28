# Knowledge Capture Workflow

> **Status:** Approved / Advisory operating workflow. Accepted for current Olympus use; not Canonical or Governing.

## Metadata

| Field | Value |
|---|---|
| Knowledge Asset ID | OPM-002 |
| Title | Knowledge Capture Workflow |
| Classification | Operating Model |
| Category | Operations / Knowledge Stewardship |
| Status | Approved |
| Authority Level | Advisory |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Primary AI Owner | Hermes |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-27 |
| Review Cadence | As Needed |
| Related Assets | GDR-004; GDR-005; GDR-006; OLY-GOV-001 through OLY-GOV-005; OPM-001; OPM-003; OPM-004; Decision Backlog |
| AI Consumption | Recommended |
| Change Impact | Medium |

---

## Purpose

Define how Olympus captures, triages, preserves, promotes, or discards knowledge from sessions, decisions, failures, surprises, research, and project events.

The default outcome for most raw observations is not a formal Knowledge Asset. Capture only what improves future reasoning, decision-making, continuity, or execution.

## Capture Outcomes

| Outcome | Use When |
|---|---|
| No Capture | Ephemeral detail with no future value |
| Daily Log | Chronological continuity only |
| Handoff Item | Needed to resume the next session |
| Backlog Question | Unresolved issue may require a future decision |
| Knowledge Asset Candidate | Durable knowledge may have future value |
| Lesson Learned | Failure, surprise, warning, or hard-won experience |
| Research Note | Evidence or analysis should be preserved |
| Decision Record | Durable decision is Proposed or Approved |
| Operating Model Update | Repeatable role or workflow changes |

## Triage

1. Ephemeral? Do not capture.
2. Chronological only? Daily log.
3. Needed to resume? Handoff.
4. Unresolved and consequential? Decision Backlog.
5. Durable Founder direction? Candidate decision or operating update.
6. Evidence or analysis? Research Note.
7. Failure, surprise, or repeated friction? Lesson candidate.
8. Repeatable workflow or role pattern? Operating-model update.
9. Otherwise preserve lightly until future value is clear.

## Routing Rules

- Concepts → `docs/concepts/`
- Decisions and backlog → `docs/decisions/`
- Governance → `docs/governance/`
- Operating models → `docs/operations/`
- Research → `docs/research/`
- Lessons → `docs/lessons/`
- Olympus continuity → `logs/daily/`
- Project-local continuity → the relevant project repository

## Authority and Metadata

- Use GDR-005 for Status, Authority Level, and Canonical Source semantics.
- Use GDR-006 for authority resolution.
- Use OLY-GOV-002 for Knowledge Asset metadata and maintenance procedure.
- Use OLY-GOV-003 and OPM-003 for decision creation, promotion, and approval.
- Use GDR-004 for Eunomia’s defined stewardship role; Eunomia is not yet instantiated and cannot approve.

## Decision Capture

Backlog items are questions, not decisions. Proposed is not Approved. AI recommendations are not decisions. Durable decisions require a formal record and explicit approval capture. Do not create decision bureaucracy for trivial tactical choices.

## Lessons and Research

Create lesson candidates when future agents might repeat a meaningful mistake or benefit from a surprising success. Research is evidence, not authority or decision. Research remains cross-cutting and may identify relevant Muse lenses.

## Experience Capture

Experience may begin as an observation, scar, intuition, surprise, tradeoff, or pattern. Capture lightly first. A formal Experience Note type remains deferred under OLY-DB-015.

## Handoff Capture Review

When durable knowledge may have been produced, handoffs should identify candidate decisions, backlog questions, lessons, research, operating changes, asset conflicts, and what should be promoted now versus deferred.

## Promotion Rules

- Start light.
- Do not promote raw transcripts or logs wholesale.
- Apply GDR-005, GDR-006, OLY-GOV-002, OLY-GOV-003, and OPM-003.
- Update indexes, Related Assets, backlog entries, and history when promotion occurs.
- Remain inside the current OPM-004 phase and Founder gate.

## Agent Responsibilities

Hermes identifies and routes candidate knowledge. Hephaestus implements scoped edits and reports evidence. Agents distinguish observation from decision, evidence from recommendation, and unresolved questions from approved direction.

## Prohibited Practices

- Capturing every comment as an asset
- Treating chat history as governed knowledge
- Treating backlog, research, or handoffs as decisions
- Creating lessons without context
- Promoting assets without metadata and approval
- Closing questions silently
- Creating later-phase application, schema, or architecture design in this workflow
- Generalizing project-local knowledge without promotion
- Reproducing metadata or authority definitions owned by GDR-005 and GDR-006

## Open Questions

- Should Olympus later define an Experience Note type?
- What threshold separates a handoff lesson from an LLR?
- Should participating projects adopt this workflow?
- What future product should implement capture and review queues?

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial workflow. |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory operating guidance. |
| 2026-07-27 | Hermes under explicit Founder direction | Aligned capture, promotion, authority, Eunomia, and roadmap references to approved foundation decisions. |
