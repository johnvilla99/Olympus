# docs/decisions/

Decision records and the decision backlog for Mt. Olympus.

## Purpose

Preserve what was decided, why, by whom, and with what consequences — not merely outcomes.

## What belongs here

- Formal decision records (ADR, PDR, GDR, ODR) — statuses: Draft, Proposed, Approved, Superseded, Retired only
- Decision backlog (`MT_OLYMPUS_DECISION_BACKLOG.md`) — open questions, not decisions
- Rationale, options considered, and follow-up actions

## What does not belong here

- Exploratory ideas without a decision frame (use `docs/concepts/`)
- General governance standards (use `docs/governance/`)
- Session handoffs or daily work logs (use `logs/daily/` for filled handoffs; templates in `templates/sessions/`)
- Decisions recorded only in chat without a durable asset

## Status

Starter directory — proposed organization.

## Current assets

| Asset | File |
|---|---|
| Decision Backlog | `MT_OLYMPUS_DECISION_BACKLOG.md` |

## Decision promotion workflow

Use **`docs/operations/OPM-003_DECISION_PROMOTION_APPROVAL_WORKFLOW.md`** (Draft / Advisory) for promoting backlog questions, working answers, and candidate decisions into formal decision records.

- **Proposed is not Approved.**
- **Approved** requires explicit John approval.
- Commit or push does not equal decision approval unless John explicitly says so.

See also: OLY-GOV-003, OPM-002, `templates/decisions/DECISION_RECORD_TEMPLATE.md`.
