# Mt. Olympus — Knowledge Asset Model

## Definition

A **Knowledge Asset** is a durable unit of preserved knowledge that is useful for future reasoning, decision-making, continuity, or execution.

A Knowledge Asset is not merely a file. It is a governed container for meaning.

## Why Knowledge Assets Exist

Traditional documents often answer "what changed?"

Knowledge Assets should also answer:

- why it mattered
- who owns it
- whether it is authoritative
- what decisions it informs
- what context would otherwise be lost
- how future agents should use it

## Asset Categories

| Category | Purpose | Example |
|---|---|---|
| Concept Record | Preserve an emerging idea before it becomes a decision | ACR-001 |
| Decision Record | Capture an approved decision and rationale | ADR, PDR, GDR |
| Governance Standard | Define rules for how work is done | Documentation governance |
| Product Definition | Define user value, scope, principles, and outcomes | Product brief, MVP definition |
| Architecture Definition | Define technical structure after product/governance clarity | Architecture overview |
| Lesson Learned | Preserve experience from success, failure, or surprise | Postmortem, retrospective |
| Research Note | Capture evidence and analysis | Competitive research |
| Operating Model | Define roles, responsibilities, and workflows | AI agent operating model |
| Handoff / Continuity Artifact | Preserve current project state for session continuity | Session handoff |

## Minimum Metadata

Every formal Knowledge Asset should include:

| Field | Meaning |
|---|---|
| Knowledge Asset ID | Stable identifier |
| Title | Human-readable name |
| Classification | Type of asset |
| Category | Knowledge domain |
| Status | Draft, exploratory, proposed, approved, superseded, retired |
| Authority Level | Informational, advisory, canonical, governing |
| Canonical Source | Yes or no |
| Owner | Human accountable owner |
| Primary AI Owner | AI role or agent responsible for stewardship, if any |
| Created On | Creation date |
| Last Updated | Latest material update |
| Review Cadence | Expected review rhythm |
| Related Assets | Linked records or dependencies |
| AI Consumption | Required, recommended, optional, restricted |
| Change Impact | Low, medium, high |

## Status Model

| Status | Meaning |
|---|---|
| Exploratory | Captures an emerging idea; not a decision |
| Draft | Being shaped into a usable artifact |
| Proposed | Ready for review or approval |
| Approved | Accepted as current guidance |
| Canonical | Source of truth for a domain or decision |
| Superseded | Replaced by a newer asset |
| Retired | No longer active, preserved for history |

## Authority Levels

| Level | Meaning |
|---|---|
| Informational | Provides context only |
| Advisory | Recommended guidance, not binding |
| Canonical | Source of truth for a defined topic |
| Governing | Controls process, standards, or authority |

## Promotion Path

Exploratory idea → Concept Record → Proposed Decision or Standard → Approved Artifact → Canonical Source, where appropriate.

Not every concept should be promoted. Many should remain preserved but non-binding.

## AI Usage Rules

AI agents should:

- check asset status before relying on content
- prefer canonical and governing assets over exploratory assets
- cite or reference source documents when making recommendations
- distinguish approved decisions from inferred guidance
- never treat a concept record as implementation authority
- flag conflicts between assets rather than silently resolving them

## Open Questions

- ~~What ID convention should Mt. Olympus use?~~ **Working answer captured** — see OLY-GOV-002 (Draft / Advisory).
- Should asset relationships eventually become graph-based? **Deferred** — see Decision Backlog OLY-DB-006.
- ~~Who approves promotion from exploratory to approved?~~ **Working answer captured** — Founder only during foundation phase; see OLY-GOV-002 and Governance Starter.
- Which assets are portfolio-wide versus project-specific? **Open / deferred** — see Decision Backlog OLY-DB-014.
- What does archival integrity require? **Open** — future concern.
