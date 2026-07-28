# Session Handoff Prompt

> **Status:** Draft / Advisory operating prompt — not a governed Knowledge Asset.

## Purpose

Reusable prompt for ending an Olympus repository session with honest evidence, governed capture routing, phase awareness, and clear next steps.

## Prompt

Prepare an **Olympus session handoff** as **Hephaestus / Coder**.

Apply OPM-001, OPM-002, OPM-003, OPM-004, and OLY-GOV-004. Use [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]] for metadata semantics, GDR-006 for authority resolution, and GDR-007 for repository identity.

A handoff is a continuity artifact, not a formal decision record. Commit or push is not approval.

Required checks:

1. Verify active repository and branch.
2. Report `git status --short` or the available equivalent.
3. Report current commit or PR state when relevant.
4. State the active OPM-004 phase and gate.
5. Reconcile handoff claims with observable repository state.

The handoff must include:

1. Session date and agent role.
2. Repository, branch, uncommitted-work, commit, push, and PR state.
3. Active phase, gate, and workstream.
4. Work completed.
5. Files created, modified, or deleted.
6. Approved decisions applied, candidate decisions, and observations — separated clearly.
7. Candidate Knowledge Assets, lessons, research, operating changes, or conflicts.
8. Actions or commands performed.
9. Validation and evidence actually obtained.
10. Limitations, failed attempts, open questions, and risks.
11. Recommended next steps and required human approval points.
12. Capture Review under [[OPM-002_KNOWLEDGE_CAPTURE_WORKFLOW|OPM-002]] and OPM-003; explicitly state when no durable candidate knowledge was produced.

Do not resolve roadmap-routed product, application-governance, architecture, or implementation questions before their OPM-004 phase and gate.

Save filled Olympus handoffs under `logs/daily/` unless formally promoted. Project-local handoffs belong in the relevant project repository.

## Suggested Output

```markdown
## Session Handoff — YYYY-MM-DD

### Repository State

### Active Phase and Gate

### Work Completed

### Files Changed

### Approved Decisions Applied

### Candidate Decisions / Backlog Items

### Candidate Knowledge Assets / Lessons / Research

### Actions Performed

### Validation / Evidence

### Limitations / Failed Attempts

### Open Questions and Risks

### Recommended Next Steps

### Commit / Push / PR Status

### Capture Review
```

## Evidence Rules

- State only validation actually performed.
- Distinguish document review, repository inspection, automated checks, and human QA.
- Do not claim tests, screenshots, browser QA, commit, push, or merge unless verified.
- When validation is unavailable, explain why and give clear human steps.
- Preserve evidence proportionally; do not create ceremonial detail.

## Do Not Do

- Treat a handoff as an Approved decision.
- Change Status or Authority without authorized approval.
- Close backlog items without authority.
- Hide failed attempts, limitations, or uncommitted work.
- Rewrite historical continuity merely to modernize terminology.
- Infer approval from conversation, silence, commit, or push.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-27 | Hermes under explicit Founder direction | Aligned handoff evidence, authority, repository, and phase rules to the Foundation Closure decisions. |
