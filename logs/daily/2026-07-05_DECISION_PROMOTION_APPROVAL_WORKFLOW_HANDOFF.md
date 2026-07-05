# Mt. Olympus Decision Promotion / Approval Workflow Handoff — 2026-07-05

> **Continuity artifact — not an approved decision record.** All work described here remains **Draft / Advisory**, not Approved, Canonical, or Governing.

## Session / Workstream

This handoff covers the **Decision Promotion / Approval Workflow** workstream completed 2026-07-05.

Scope: define a practical Draft / Advisory workflow for how backlog questions, working answers, candidate decisions, and Founder direction become formal Decision Records — without mistaking discussion for approval.

Nothing in this workstream was promoted to Approved, Canonical, or Governing status.

## Repository State

**Branch:** `main`

**`git status --short`:**

```text
(clean — no uncommitted changes at handoff creation time, before this file is written)
```

**`git branch --show-current`:**

```text
main
```

**`git log --oneline -5`:**

```text
f6e7843 Add decision promotion approval workflow
0235ee1 Add knowledge capture workflow handoff
e78784b Add knowledge capture workflow
8582d2d Add operating model handoff
1e5bce7 Add Olympus agent operating model
```

Decision promotion workflow changes are committed in `f6e7843`. This handoff file is new and uncommitted.

## Work Completed

- **`OPM-003_DECISION_PROMOTION_APPROVAL_WORKFLOW.md`** created — Draft / Advisory promotion and approval workflow
- **Operations README** updated to list OPM-003
- **Decision README** updated with decision promotion workflow section
- **Session start and handoff prompts** updated to reference OPM-003
- **Decision Record template** updated with Proposed ≠ Approved and John approval note
- **Session handoff template** updated — Capture Review routes include Draft/Proposed Decision Record paths
- **Cursor rules** updated to reference OPM-003 (`asset-authority`, `knowledge-assets`, `session-continuity`, rules README)
- **Decision backlog** updated with OPM-003 working answer — **OLY-DB-009** and **OLY-DB-017** remain open or deferred

## Assets Created or Updated

```text
docs/operations/OPM-003_DECISION_PROMOTION_APPROVAL_WORKFLOW.md
docs/operations/README.md
docs/operations/session_start_prompt.md
docs/operations/session_handoff_prompt.md
docs/decisions/README.md
docs/decisions/MT_OLYMPUS_DECISION_BACKLOG.md
templates/decisions/DECISION_RECORD_TEMPLATE.md
templates/sessions/SESSION_HANDOFF_TEMPLATE.md
.cursor/rules/asset-authority.mdc
.cursor/rules/knowledge-assets.mdc
.cursor/rules/session-continuity.mdc
.cursor/rules/README.md
```

## Decision Workflow Summary

Core principle:

```text
A decision is not approved because it was discussed; it is approved only when John explicitly approves it and the record captures enough context for future work.
```

Key routing model:

```text
Ephemeral/tactical choice → no decision
Unresolved future-impact question → decision backlog
Useful but unapproved guidance → working answer
Decision being shaped → Draft Decision Record
Ready for John review → Proposed Decision Record
Explicit John approval captured → Approved Decision Record
Replaced decision → Superseded Decision
Inactive without replacement → Retired Decision
```

## Decisions vs Observations

- **No asset** was promoted to Approved, Canonical, or Governing.
- **OPM-003** is Draft / Advisory — not an approved or canonical workflow.
- **Backlog updates** are working guidance, not formal decisions.
- **Commit/push does not equal decision approval** unless John explicitly says so.
- Formal decision promotion still requires explicit **John approval** through `docs/decisions/`.

## Open Questions Preserved

- OLY-DB-009: How should agents discover authoritative knowledge?
- OLY-DB-017: Formal GDR promotion of ID convention
- Should OPM-003 later become Canonical?
- Should Olympus create a dedicated decision-promotion checklist template?
- Should every Proposed decision require a formal John review section?
- Should backlog statuses be standardized further?
- Should approval context cite session logs, commits, or both?
- Should the formal GDR promotion of ID convention become the first real Decision Record?

Also captured in OPM-003 Open Questions section.

## Evidence / Validation

Validation performed: **document review and alignment** against:

```text
OLY-GOV-002
OLY-GOV-003
OLY-GOV-004
OPM-001
OPM-002
OPM-003
Decision backlog
Decision Record Template
Session Handoff Template
Cursor rules
```

Git command output reviewed (`git status --short`, `git branch --show-current`, `git log --oneline -5`).

**No app tests** were run — no application code exists or was changed in this workstream.

## Known Limitations

- Product and architecture Tier 3 questions remain deferred.
- OLY-DB-009 remains open.
- OLY-DB-017 remains deferred.
- No formal decision records were created in this pass.
- OPM-003 is not Approved, Canonical, or Governing.
- Commit/push alone is not approval.

## Recommended Next Steps

1. Commit and push this handoff if not already committed.
2. Start the next Olympus session using `docs/operations/session_start_prompt.md`.
3. Consider creating the first formal Draft or Proposed GDR for the Olympus ID convention.
4. Keep OLY-DB-009 open until agent discovery behavior is stronger.
5. Keep product/architecture Tier 3 questions deferred unless explicitly scoped.

## Resume Instructions for Next Session

- Read this handoff first.
- Read OPM-003.
- Read OPM-002.
- Read OLY-GOV-003.
- Read the decision backlog.
- Check git status before editing.
- Confirm the active workstream with John before making changes.

## Capture Review

| Capture Candidate | Route | Notes |
|---|---|---|
| Decision Promotion / Approval Workflow | `docs/operations/OPM-003_DECISION_PROMOTION_APPROVAL_WORKFLOW.md` | Created as Draft / Advisory operating workflow |
| First formal GDR for ID convention | Decision backlog / future Draft GDR | Candidate next step; not created in this pass |
| OLY-DB-009 | Decision backlog | Still open; partially addressed by OPM-003 |
| OLY-DB-017 | Decision backlog | Formal ID convention promotion still deferred |

## Change / Commit Status

- Decision promotion workflow work **committed** on `main` as `f6e7843 Add decision promotion approval workflow`.
- **This handoff file is uncommitted** at creation time.
- **Do not commit** unless John explicitly requests it.
