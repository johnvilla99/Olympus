# Canonical Repository Location

> **Status:** Superseded / Canonical historical decision. GDR-009 is the current Canonical source for the active Olympus repository.

## Metadata

| Field | Value |
|---|---|
| Decision ID | GDR-007 |
| Title | Canonical Repository Location |
| Classification | Decision Record |
| Decision Category | Governance |
| Status | Superseded |
| Authority Level | Canonical |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Decider / Approver | John S. Villasenor |
| Created On | 2026-07-27 |
| Decided On | 2026-07-27 |
| Last Updated | 2026-08-15 |
| Review Cadence | Historical; review only if migration history requires clarification |
| Related Assets | [[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]]; [[GDR-009_CANONICAL_REPOSITORY_LOCATION|GDR-009]]; [[OLY-GOV-001_REPOSITORY_STANDARD|OLY-GOV-001]]; [[OLY-GOV-004_SESSION_CONTINUITY_STANDARD|OLY-GOV-004]]; [[OPM-004_OLYMPUS_PRODUCT_TO_ARCHITECTURE_ROADMAP|OPM-004]] |
| Supersedes | N/A |
| Superseded By | GDR-009 |
| AI Consumption | Recommended for historical context |
| Change Impact | High |

---

## Historical Decision

At the time of this decision, the active durable repository for Olympus was designated as:

```text
e7-jvillasenor/Olympus
```

The default active branch was `main`.

`johnvilla99/Olympus` was treated as the historical source repository used for migration.

This decision is no longer current. [[GDR-009_CANONICAL_REPOSITORY_LOCATION|GDR-009]] supersedes it and designates `johnvilla99/Olympus` as the active durable repository.

## Context

Olympus was cloned from John’s prior GitHub account into the E7CORE-aligned account so connected agents and future work could use the intended organizational context at that time.

## Options Considered

| Option | Outcome at the time |
|---|---|
| Designate `e7-jvillasenor/Olympus` | **Selected** — aligned active stewardship with the E7CORE environment at that time |
| Continue dual-active repositories | Rejected — created split-brain source-of-truth risk |
| Keep `johnvilla99/Olympus` active | Rejected at the time — conflicted with the migration objective then in force |

## Historical Consequences

- New changes were directed to `e7-jvillasenor/Olympus` while this decision remained current.
- Search and connector configurations were expected to prefer that repository.
- Commit history recorded migration provenance but did not determine governance approval.

Those consequences are superseded by GDR-009 for current work.

## Approval Context

Approved through explicit Founder direction in the E7CORE Hermes session on 2026-07-27.

## Supersession

GDR-009 superseded this decision on 2026-08-15 after explicit Founder direction re-established `johnvilla99/Olympus` as the active durable repository. This record remains preserved to retain migration rationale and prevent historical ambiguity.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-27 | John S. Villasenor | Designated `e7-jvillasenor/Olympus` as the active durable repository. |
| 2026-08-15 | Hermes under explicit Founder direction | Marked GDR-007 Superseded by GDR-009 and preserved the prior repository decision as historical context. |
