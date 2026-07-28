# Olympus — Knowledge Asset Model

## Definition

A **Knowledge Asset** is a durable unit of preserved knowledge useful for future reasoning, decision-making, continuity, or execution.

A Knowledge Asset is not merely a file. It is a governed container for meaning.

## Why Knowledge Assets Exist

Knowledge Assets should preserve:

- why the knowledge matters
- who owns it
- whether it is authoritative
- what decisions it informs
- what context would otherwise be lost
- how future agents should use it

## Asset Categories

| Category | Purpose |
|---|---|
| Concept Record | Preserve an emerging idea before it becomes a decision |
| Decision Record | Capture a durable decision and rationale |
| Governance Standard | Define rules for how work is done |
| Product Definition | Define user value, scope, principles, and outcomes |
| Architecture Definition | Define technical structure after product and governance clarity |
| Lesson Learned | Preserve experience from success, failure, or surprise |
| Research Note | Capture evidence and analysis |
| Operating Model | Define roles, responsibilities, and workflows |
| Handoff / Continuity Artifact | Preserve project or session state for continuity |

## Minimum Metadata

Formal assets should include ID, Title, Classification, Category, Status, Authority Level, Canonical Source, Owner, Primary AI Owner when active, Created On, Last Updated, Review Cadence, Related Assets, AI Consumption, and Change Impact.

Identifiers are governed by **GDR-001**. Metadata semantics are governed by **GDR-005**. Authority resolution is governed by **GDR-006**. Operational procedure remains in OLY-GOV-002.

## Status Model

The authoritative lifecycle model is **GDR-005**. This foundation model does not duplicate the status definitions.

## Authority Levels

The authoritative metadata semantics are **GDR-005** and the authority-resolution order is **GDR-006**. This foundation model does not duplicate those definitions.

## Promotion Path

```text
Exploratory idea → Concept Record → Proposed Decision or Standard → Approved Artifact → authority and source designation under GDR-005, where appropriate
```

Not every concept should be promoted. Many should remain preserved but non-binding.

## AI Usage Rules

Agents should:

- evaluate asset metadata before relying on content
- use GDR-006 for authority resolution
- cite material sources
- distinguish approved direction from inference
- never treat a concept record as implementation authority
- flag conflicts rather than silently resolving them
- preserve project-local versus portfolio-wide boundaries

## Open Questions

- The ID convention is governed by GDR-001.
- Asset relationship implementation remains deferred under OLY-DB-006.
- Promotion and authority changes follow GDR-005, GDR-006, OLY-GOV-002, and OPM-003.
- Portfolio-wide versus project-specific scope remains open under OLY-DB-014.
- Archival-integrity requirements remain open.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-27 | Hermes under explicit Founder direction | Aligned the model to GDR-001, GDR-005, and GDR-006 without repeating their definitions. |
