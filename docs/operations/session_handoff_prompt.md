# Session Handoff Prompt

> **Status:** Draft / Advisory operating prompt — not an approved Knowledge Asset.

## Purpose

Reusable prompt for ending a Cursor session in the Olympus repository. Preserves continuity, honest evidence, and clear next steps.

## Prompt

Copy and paste the block below into Cursor at session end:

---

Prepare an **Olympus session handoff** for this work session.

**Do not treat this handoff as a formal decision record.** Durable decisions belong in `docs/decisions/` with Founder approval.

**Required checks — run or report:**

1. `git status --short`
2. Current branch (`git branch --show-current`)
3. Recent commit info if relevant (`git log -1 --oneline` when commits were made)

**Handoff must include:**

1. **Session date** and agent/role
2. **Repository state** — branch, uncommitted work, commit/push status
3. **Work completed** — concise summary
4. **Files changed** — list with created/modified/deleted
5. **Decisions made** vs **observations** — separate clearly; Decision Records do not use Exploratory status
6. **Candidate decisions** — for decision backlog if not yet formal
7. **Candidate Knowledge Assets** — for promotion review if applicable
8. **Commands run** — relevant shell commands
9. **Validation / evidence** — honest account of what was verified
10. **Open questions** and **risks / watch items**
11. **Recommended next steps**
12. **Commit status** — committed or not; do not commit unless John asked

**Tier 3 items:** List any product/architecture questions encountered but **do not resolve** them — mark as deferred.

**Follow-up needed?** Note if Knowledge Assets, decision records, backlog items, or templates need updates in a future session.

Use structure from `templates/sessions/SESSION_HANDOFF_TEMPLATE.md`. File filled Olympus handoffs in `logs/daily/` when saving to the repo.

---

## Required Checks

- [ ] `git status --short`
- [ ] Branch and uncommitted work reported
- [ ] Files changed listed
- [ ] Decisions vs observations separated
- [ ] Validation reported honestly
- [ ] Commit/push status stated

## Required Output Format

```markdown
## Session Handoff — YYYY-MM-DD

### Repository State
(branch, git status summary, commit/push status)

### Work Completed
-

### Files Changed
|

### Decisions Made (session observations)
|

### Candidate Decisions / Backlog Items
|

### Candidate Knowledge Assets
|

### Commands Run

### Validation / Evidence
(honest — what was actually verified)

### Open Questions
-

### Risks / Watch Items
-

### Recommended Next Steps
1.

### Commit Status
(committed / not committed)
```

## Evidence Rules

- Do **not** claim tests or validation not performed.
- Do **not** claim screenshots or browser QA unless actually performed.
- If no tests applied, say so (e.g. documentation-only session).
- If only document review was performed, state that explicitly.
- If uncommitted work remains, state that clearly.
- Provide human QA steps when Cursor could not validate.

## Do Not Do

- Promote documents to Approved, Canonical, or Governing
- Treat session observations as formal approved decisions
- Close backlog items without explicit Founder direction
- Delete historical context or hide failed attempts
- Resolve Tier 3 product/architecture questions
- Commit unless John explicitly requested it
