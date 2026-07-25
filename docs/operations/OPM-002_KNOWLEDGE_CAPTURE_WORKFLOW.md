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
| Last Updated | 2026-07-25 |
| Review Cadence | As Needed |
| Related Assets | OPM-001; OLY-GOV-001; OLY-GOV-002; OLY-GOV-003; OLY-GOV-004; OLY-GOV-005; ACR-002; Decision Backlog; Session Handoff Template |
| AI Consumption | Recommended |
| Change Impact | Medium |

---

## Purpose

OPM-002 defines how Olympus **captures, triages, preserves, promotes, or discards** knowledge from ongoing work: sessions, conversations, project events, decisions, failures, surprises, and research.

This workflow prevents:

- Valuable experience disappearing into chat history
- Every observation becoming paperwork
- Backlog questions being mistaken for decisions
- Lessons being lost because they were not promoted
- Exploratory ideas being treated as approved guidance
- Agents creating assets without future decision value
- Session handoffs becoming bloated archives

## Scope

**In scope:**

- Session observations
- Handoff notes
- Decision candidates
- Lesson candidates
- Research findings
- Governance and operations improvement candidates
- Agent-discovered conflicts
- Founder direction that may have durable value

**Out of scope:**

- Application capture UI
- Database schema
- Graph or vector storage
- Product MVP design
- Automated pipelines
- Replacing formal decision approval
- Participating project adoption requirements

## Core Principle

> **Capture only what improves future reasoning, decision-making, continuity, or execution.**

The default outcome for most raw observations is **not** a formal Knowledge Asset.

## Capture Inputs

| Input | Examples |
|---|---|
| Founder direction | John clarifies authority, naming, scope, priorities |
| Session work | Edits, reviews, handoffs, implementation attempts |
| Agent observations | Conflicts, missing metadata, unclear ownership |
| Decisions or near-decisions | Selected direction, rejected options, durable tradeoffs |
| Lessons | Failures, surprises, repeated friction, warnings |
| Research | Evidence, tool comparisons, market findings, technical investigation |
| Project events | Releases, incidents, QA findings, retrospectives |
| Experience | Patterns, scars, judgment, intuition worth preserving |

## Capture Outcomes

| Outcome | Use When | Location |
|---|---|---|
| No Capture | Ephemeral detail with no future value | None |
| Daily Log Note | Chronological continuity value only | `logs/daily/` |
| Handoff Item | Needed for next session resume | Session handoff / `logs/daily/` |
| Backlog Question | Open question may require future decision | `docs/decisions/MT_OLYMPUS_DECISION_BACKLOG.md` |
| Knowledge Asset Candidate | Durable knowledge may have future reasoning value | Handoff or log first; promote to `docs/` |
| Lesson Learned | Experience, failure, surprise, or warning has future value | `docs/lessons/` with `LLR-*` |
| Research Note | Evidence or analysis should be preserved | `docs/research/` with `RNO-*` |
| Decision Record | Durable decision is approved or proposed for review | `docs/decisions/` with ADR/PDR/GDR/ODR |
| Operating Model Update | Workflow, role, or stewardship pattern changes | `docs/operations/` with `OPM-*` |

## Triage Decision Tree

Use in order. Stop at the first fit unless multiple routes apply.

1. Is it ephemeral with no future value? → No Capture.
2. Is it only useful for chronological continuity? → Daily Log Note.
3. Is it needed to resume the next session? → Handoff Item.
4. Is it an unresolved question that could affect future work? → Backlog Question.
5. Is it Founder direction with durable impact? → Candidate Decision, Operating Model update, or Knowledge Asset depending on scope.
6. Is it an approved durable choice with rationale? → Decision Record.
7. Is it evidence or analysis? → Research Note.
8. Is it a failure, surprise, repeated friction, warning, or hard-won experience? → Lesson Learned candidate.
9. Is it a repeatable role, workflow, or stewardship pattern? → Operating Model update or OPM candidate.
10. Does it help future reasoning, decision-making, continuity, or execution? → Knowledge Asset candidate.
11. If uncertain, capture lightly in a handoff or backlog. Do not over-promote.

## Capture Criteria

A formal asset candidate should usually have:

- Future value
- Owner or likely owner
- Context
- Status
- Authority Level
- Related assets
- Open questions
- Expected consumer
- Consequence of losing the knowledge

If the consequence of losing it is low, prefer a log, handoff, or no capture. If the consequence of misusing it is high, add explicit authority warnings. If it is unresolved, use the backlog or Open Questions rather than a decision record.

## Artifact Routing Rules

| Content Type | Route |
|---|---|
| Raw session detail | Usually no capture or daily log |
| Session next-step context | Handoff |
| Open governance, product, or architecture question | Decision backlog |
| Approved durable decision | Decision record |
| Emerging concept | `docs/concepts/` as ACR or concept record |
| Operational workflow | `docs/operations/` as OPM or operations note |
| Research evidence | `docs/research/` as RNO |
| Failure, surprise, or lesson | `docs/lessons/` as LLR |
| Repository organization rule | `docs/governance/` as OLY-GOV standard |
| Project-specific handoff | Project repository, not Olympus by default |

## Decision Capture Rules

Apply **OLY-GOV-003**, the authoritative Olympus source for decision authority, status, approval, and hierarchy.

- Backlog items are questions, not decisions.
- Decision Records do not use Exploratory status.
- John approval is required for Approved status.
- Proposed means ready for review, not accepted.
- Assistant recommendations are not decisions.
- Durable Founder direction may become a decision record when it affects future work.
- Do not create decision records for tiny tactical choices with no future consequence.

## Lesson Capture Rules

Create a Lesson Learned candidate when:

- Something failed in a meaningful way
- A repeated friction pattern appears
- An assumption was wrong
- A surprising success reveals a pattern
- Future agents would likely repeat the mistake
- A warning should travel across projects

Include what happened, why it mattered, root cause or contributing factors, the lesson, future guidance, related assets and projects, and confidence where useful.

## Research Capture Rules

- **Research is a cross-cutting activity, not a tenth Muse.**
- Use `RNO-*` for research notes under GDR-001.
- Include source, provenance, and confidence.
- Include relevant Muse lenses when applicable.
- Research findings are evidence, not decisions.
- Tool, vendor, or product choices still require decision records when selected.

## Experience Capture Rules

- Experience may start as an observation, scar, surprise, intuition, or repeated pattern.
- Capture lightly first unless future value is clear.
- Do not implement the conceptual `experience_events` schema in this workflow.
- An Experience Note artifact type remains deferred under OLY-DB-015.
- For now, use handoffs, logs, lessons, operating notes, and candidate Knowledge Assets.

## Session Handoff Capture Rules

Handoffs should include a Capture Review when the session produced candidate knowledge. The review asks whether the session produced candidate decisions, backlog questions, lesson candidates, research findings, operating-model changes, asset conflicts, or material requiring promotion.

If nothing durable was produced, state that explicitly.

## Promotion Rules

- Start light with a handoff, log, or backlog unless the knowledge is clearly durable.
- Promote only when future value justifies maintenance cost.
- Do not promote raw chat transcripts wholesale.
- Formal assets require metadata under OLY-GOV-002.
- Decisions follow OLY-GOV-003.
- Continuity follows OLY-GOV-004.
- Promotion to Approved, Canonical, or Governing requires explicit John approval.
- Update indexes and related assets when promoting.

## AI Agent Responsibilities

**Hermes** should identify capture candidates, route them correctly, flag over-capture and under-capture, and preserve continuity.

**Hephaestus** should implement scoped capture edits, update templates and indexes when asked, report changed files and evidence, and never approve or promote assets.

All agents must distinguish observation from decision, evidence from recommendation, and unresolved questions from approved direction.

## Founder Review Points

Ask John before:

- Promoting to Approved, Canonical, or Governing
- Creating a new formal asset category
- Closing a backlog item
- Creating a decision record for durable direction
- Changing Muse definitions
- Changing ID conventions
- Turning a workflow into a standard
- Resolving Tier 3 product or architecture questions

## Prohibited Practices

- Capturing every comment as a Knowledge Asset
- Treating chat history as governed knowledge
- Treating backlog items or Research Notes as decisions
- Creating lessons without context
- Promoting assets without metadata
- Closing open questions without John approval
- Creating app, storage, or schema designs in this workflow
- Centralizing project-specific handoffs in Olympus by default
- Silently discarding high-value lessons
- Silently promoting exploratory content
- Duplicating governance rules that are already owned by an OLY-GOV artifact

## Open Questions

- Should Olympus later define a formal Experience Note artifact type?
- Should Capture Review become required in every handoff?
- Should OPM-002 later become Canonical?
- Should participating projects adopt the same capture workflow?
- Should a future product implement capture queues or review inboxes?
- What is the threshold for creating `LLR-*` versus keeping a lesson in a handoff?

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial Draft / Advisory Knowledge Capture Workflow |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory operating guidance; aligned decision authority to OLY-GOV-003 and Research to the cross-cutting model |