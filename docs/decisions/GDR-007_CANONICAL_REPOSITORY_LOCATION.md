# Canonical Repository Location

> **Status:** Approved / Canonical. This decision identifies the active durable repository for Olympus.

## Metadata

| Field | Value |
|---|---|
| Decision ID | GDR-007 |
| Title | Canonical Repository Location |
| Classification | Decision Record |
| Decision Category | Governance |
| Status | Approved |
| Authority Level | Canonical |
| Canonical Source | Yes |
| Owner | John S. Villasenor |
| Decider / Approver | John S. Villasenor |
| Created On | 2026-07-27 |
| Decided On | 2026-07-27 |
| Last Updated | 2026-07-27 |
| Review Cadence | When repository ownership or hosting changes |
| Related Assets | GDR-006; OLY-GOV-001; OLY-GOV-004; OPM-004 |
| Supersedes | N/A |
| Superseded By | N/A |
| AI Consumption | Required |
| Change Impact | High |

---

## Decision

The active durable repository for Olympus is:

```text
e7-jvillasenor/Olympus
```

The default active branch is `main`.

`johnvilla99/Olympus` is the historical source repository used for migration. It is not the location for new Olympus work after this decision. Historical handoffs and records must not be rewritten solely to change the repository name; active instructions, indexes, prompts, and rules must reference GDR-007 or the active repository.

## Context

Olympus was cloned from John’s prior GitHub account into the E7CORE-aligned account so connected agents and future work use the correct organizational context.

## Options Considered

| Option | Outcome |
|---|---|
| Designate `e7-jvillasenor/Olympus` | **Selected** — aligns active stewardship with the E7CORE environment |
| Continue dual-active repositories | Rejected — creates split-brain source-of-truth risk |
| Keep `johnvilla99/Olympus` active | Rejected — conflicts with the approved transition objective |

## Consequences

- New changes must target `e7-jvillasenor/Olympus`.
- The historical repository should be frozen or archived after branch, tag, and commit parity are verified.
- Search and connector configurations must prefer the active repository and avoid mixing results from both repositories.
- Commit history records migration provenance but does not determine governance approval.

## Approval Context

Approved through explicit Founder direction in the E7CORE Hermes session on 2026-07-27.

## Follow-up Actions

- Verify `main`, required branches, tags, and the expected migration commit history.
- Update active repository locators without rewriting historical handoffs.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-27 | John S. Villasenor | Designated `e7-jvillasenor/Olympus` as the active durable repository. |
