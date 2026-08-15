# Canonical Repository Location

> **Status:** Approved / Canonical. This decision identifies the active durable repository for Olympus and supersedes GDR-007.

## Metadata

| Field | Value |
|---|---|
| Decision ID | GDR-009 |
| Title | Canonical Repository Location |
| Classification | Decision Record |
| Decision Category | Governance |
| Status | Approved |
| Authority Level | Canonical |
| Canonical Source | Yes |
| Owner | John S. Villasenor |
| Decider / Approver | John S. Villasenor |
| Created On | 2026-08-15 |
| Decided On | 2026-08-15 |
| Last Updated | 2026-08-15 |
| Review Cadence | When repository ownership or hosting changes |
| Related Assets | [[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]]; [[GDR-007_CANONICAL_REPOSITORY_LOCATION|GDR-007]]; [[OLY-GOV-001_REPOSITORY_STANDARD|OLY-GOV-001]]; [[OLY-GOV-004_SESSION_CONTINUITY_STANDARD|OLY-GOV-004]]; [[OPM-004_OLYMPUS_PRODUCT_TO_ARCHITECTURE_ROADMAP|OPM-004]] |
| Supersedes | GDR-007 |
| Superseded By | N/A |
| AI Consumption | Required |
| Change Impact | High |

---

## Decision

The active durable repository for Olympus is:

```text
johnvilla99/Olympus
```

Repository branch selection and default-branch configuration are operational state and do not alter this Canonical repository-location decision.

The `e7-jvillasenor/Olympus` repository may remain available as migration or historical context, but it is not the active durable repository for new Olympus work unless a future approved decision changes this designation.

## Context

GDR-007 designated `e7-jvillasenor/Olympus` as the active repository during an earlier migration effort. Subsequent working practice and explicit Founder direction established that active Olympus development and product-definition work should remain in `johnvilla99/Olympus`, with Cursor's `origin` remote tracking that repository.

Continuing to treat the E7 repository as authoritative created split-brain behavior across agents and tooling. This decision removes that ambiguity.

## Options Considered

| Option | Outcome |
|---|---|
| Return active stewardship to `johnvilla99/Olympus` | **Selected** — matches current Founder direction, Cursor `origin`, and active Phase 2 work |
| Continue dual-active repositories | Rejected — preserves source-of-truth ambiguity |
| Keep `e7-jvillasenor/Olympus` active | Rejected — conflicts with current Founder direction and active working practice |

## Rationale

Olympus requires one unambiguous durable repository. The active repository must match the repository used by the Founder, implementation tools, and authorized agents. Keeping governance aligned with actual operating practice prevents future agents from following a stale migration decision into the wrong repository.

## Consequences

- New Olympus work must target `johnvilla99/Olympus` unless explicitly directed otherwise.
- Active prompts, indexes, rules, standards, and working artifacts should reference GDR-009 rather than GDR-007 for repository location.
- `e7-jvillasenor/Olympus` must not be treated as an active peer source of truth.
- Historical records may retain references to GDR-007 where preserving history is appropriate.
- GDR-007 is superseded and remains preserved for rationale and migration history.

## Risks

- Existing agents or local clones may still have an `e7` remote or stale instructions.
- The GitHub repository default branch may not yet reflect the desired long-term branch strategy.
- Historical copies may continue to appear in search results and should not be mistaken for current authority.

## Follow-up Actions

- Update active repository locators to GDR-009.
- Keep Cursor `origin` pointed at `johnvilla99/Olympus`.
- Treat alternate remotes as explicitly named historical or migration remotes rather than active defaults.
- Review repository default-branch configuration separately if needed.

## Approval Record

- **Approver:** John S. Villasenor
- **Approval date:** 2026-08-15
- **Approved authority:** Canonical
- **Approval context:** Explicit Founder direction in the active Olympus Phase 2 session to use `johnvilla99/Olympus` as the active repository and proceed with the repository-governance correction.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-08-15 | John S. Villasenor / Hermes | Superseded GDR-007 and designated `johnvilla99/Olympus` as the active durable repository. |
| 2026-08-15 | Hermes under explicit Founder direction | Removed transient branch state from the Canonical decision and clarified that branch selection is operational state. |
