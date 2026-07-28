# Knowledge Asset Standard

> **Status:** Approved / Advisory. Accepted for current Olympus use; not Canonical or Governing unless explicitly stated.

## Metadata

| Field | Value |
|---|---|
| Standard ID | OLY-GOV-002 |
| Title | Knowledge Asset Standard |
| Status | Approved |
| Authority Level | Advisory |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-27 |
| Review Cadence | As Needed |
| Related Assets | [[GDR-001_OLYMPUS_ID_CONVENTION|GDR-001]]; [[GDR-004_EUNOMIA_ECOSYSTEM_STEWARDSHIP_ROLE|GDR-004]]; [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]]; [[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]]; [[OLY-GOV-001_REPOSITORY_STANDARD|OLY-GOV-001]]; [[OLY-GOV-003_DECISION_RECORD_STANDARD|OLY-GOV-003]]; [[OLY-GOV-005_AGENT_KNOWLEDGE_DISCOVERY_STANDARD|OLY-GOV-005]]; [[OPM-003_DECISION_PROMOTION_APPROVAL_WORKFLOW|OPM-003]] |
| AI Consumption | Required |
| Change Impact | High |

---

## Purpose

Make Knowledge Assets trustworthy, discoverable, maintainable, and safe for humans and AI agents to consume.

A Knowledge Asset is not merely a file. It is a governed container for meaning: what is known, why it matters, who owns it, whether it is authoritative, and how future work should use it.

## Scope

Applies to formal Knowledge Assets stored in Olympus.

**In scope:** metadata, categories, placement, creation, promotion, maintenance, supersession, retirement, relationships, citation, and experience capture.

**Out of scope:** application UI, database schema, automation pipelines, unapproved external-project standards, and automatic promotion.

## Definition

A **Knowledge Asset** is a durable unit of preserved knowledge useful for future reasoning, decision-making, continuity, or execution.

Formal assets should preserve purpose, context, ownership, authority, related decisions, future use, and enough provenance for safe consumption.

## What Qualifies

Typical asset classes include Concept Records, Decision Records, Governance Standards, Product Definitions, Architecture Definitions, Lessons Learned, Research Notes, Operating Models, and promoted Handoff/Continuity Artifacts.

An asset qualifies when it has future value, accountable ownership, honest metadata, and a clear expected consumer.

## What Does Not Qualify

- Scratch notes with no future value
- Raw transcripts unless curated
- Duplicate copies without an authoritative-source reference
- Temporary logs unless promoted
- Application source code and build artifacts
- Secrets or credentials
- Vague ideas without context, owner, or future use
- Templates and directory indexes

## Categories and Placement

| Category | Typical Location |
|---|---|
| Concept Record | `docs/concepts/` |
| Decision Record | `docs/decisions/` |
| Governance Standard | `docs/governance/` |
| Product Definition | `docs/foundation/` or `docs/projects/` until formal product structure is approved |
| Architecture Definition | `docs/concepts/` until formal architecture structure is approved |
| Lesson Learned | `docs/lessons/` |
| Research Note | `docs/research/` |
| Operating Model | `docs/operations/` |
| Handoff / Continuity Artifact | `logs/` unless promoted |

Research remains cross-cutting and is not a tenth Muse.

## Identifier Convention

**[[GDR-001_OLYMPUS_ID_CONVENTION|GDR-001]]** is the Canonical source for identifiers, prefixes, numbering, stability, and non-reuse. This standard applies those rules without reproducing the catalog.

## Required Metadata

Every formal Knowledge Asset should include:

| Field | Meaning |
|---|---|
| Knowledge Asset ID | Stable identifier under [[GDR-001_OLYMPUS_ID_CONVENTION|GDR-001]] |
| Title | Human-readable name |
| Classification | Asset type |
| Category | Knowledge domain |
| Status | Lifecycle maturity under [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]] |
| Authority Level | Binding weight under [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]] |
| Canonical Source | Source-of-truth designation under [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]] |
| Owner | Accountable human owner |
| Primary AI Owner | Active stewardship role, if any; GDR-004 does not instantiate Eunomia |
| Created On | Creation date |
| Last Updated | Latest material update |
| Review Cadence | Expected review rhythm |
| Related Assets | Dependencies, lineage, and related records; for known Olympus assets prefer Obsidian links shaped like `` [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]] `` |
| AI Consumption | Required, Recommended, Optional, or Restricted |
| Change Impact | Low, Medium, or High |

Seed assets may be completed on their next substantive edit. Do not backfill unknown values speculatively.

## Status, Authority, and Canonical Source

Use **[[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]]** for lifecycle Status, Authority Level, and Canonical Source semantics. Canonical is an Authority Level, not a lifecycle Status.

Use **[[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]]** for authority resolution and conflicts. This standard does not duplicate either decision.

## Discoverability Links (Obsidian)

Formal references to known Olympus assets should use Obsidian internal links shaped like `` [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]] ``. Stable IDs remain the visible labels.

Obsidian links are a discoverability and navigation mechanism. They do not determine authority, lifecycle, canonical status, or formal relationship semantics. A graph edge does not by itself define relationship type or approval. Relationship meaning remains in metadata, prose, and terms such as informs, references, depends_on, supersedes, replaces, contradicts, implements, and related_to.

Do not treat Graph View, Dataview, or plugin behavior as Olympus architecture. Historical records need not be rewritten solely to add links.

New assets normally begin at `Exploratory` or `Draft` unless a higher status is explicitly approved.

## Canonical Source Rules

- Prefer one Canonical source per defined subject.
- Duplicate content must identify and defer to its authoritative source.
- Canonical or Governing authority and `Canonical Source: Yes` require explicit approval under [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]], GDR-006, and OPM-003.
- Exploratory ACRs are not Canonical.
- Root README is a front door, not the source of truth for every topic.
- `LICENSE` controls repository usage rights.

## AI Consumption Rules

Agents must:

1. Evaluate Status, Authority Level, and Canonical Source together.
2. Apply GDR-006 and OLY-GOV-005.
3. Cite material sources.
4. Distinguish approved direction from inference or conversation.
5. Flag conflicts.
6. Respect Restricted assets.

## Asset Creation Rules

- Start from the appropriate template when useful.
- Assign an ID under [[GDR-001_OLYMPUS_ID_CONVENTION|GDR-001]].
- Complete required metadata.
- Set honest initial lifecycle and authority values.
- Include purpose, context, authority notes, AI guidance, related assets, open questions, and history as appropriate.
- Create an asset only when it improves future reasoning, decisions, continuity, or execution.
- Keep one primary concern per asset and link related content.

## Minimum Bar for Proposed

An asset may move to Proposed when required metadata is complete or explicitly marked TBD with reason; purpose, context, owner, related assets, AI Consumption, open questions, and history are clear; and the asset has future value.

Proposed means ready for review, not Approved.

## Promotion Rules

Typical path:

```text
Exploratory idea → Concept Record → Proposed Decision or Standard → Approved Artifact → authority and source designation under GDR-005, where appropriate
```

Promotion requires a clear problem, known owner, future value, and maintenance responsibility. Status and authority changes follow GDR-005 and GDR-006; approval workflow and agent boundaries follow OPM-003 and GDR-004.

Promotion should update Related Assets, indexes, the Decision Backlog when applicable, and Change History.

## Review and Maintenance

- Set a review cadence.
- Update Last Updated for material changes.
- Record meaningful changes in Change History.
- Review stale and High-impact assets before relying on them.
- Owners remain accountable for accurate metadata.

## Supersession and Retirement

Preserve superseded and retired assets with rationale and links. Do not delete historical assets casually. Update Related Assets on predecessor and successor.

## Relationships and Citation

Recognized relationship terms include `informs`, `supersedes`, `contradicts`, `depends_on`, `references`, `replaces`, and `related_to`. Relationships remain expressed through metadata and links; graph implementation is deferred.

## Experience Capture

Experience often begins as an observation, lesson, failure, surprise, tradeoff, or pattern. Capture lightly in handoffs or logs when appropriate. Promote durable experience when it has future decision value, preserving what happened, why it mattered, the lesson, future use, related assets, and confidence.

A formal Experience Note type remains deferred.

## Prohibited Practices

- Treating every note as authoritative
- Creating formal assets with missing required metadata
- Duplicating authoritative content without a source reference
- Treating exploratory ACRs as implementation authority
- Bypassing GDR-005, GDR-006, or OPM-003 when changing lifecycle or authority
- Deleting superseded assets without preservation rationale
- Storing secrets
- Creating paperwork without future value
- Assigning conflicting Canonical sources
- Repeating a rule owned by another authoritative artifact when a reference is sufficient

## Exceptions

Exception authority and approval follow GDR-006 and OPM-003. Record approved exceptions in the affected asset or a decision record.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial draft and foundation working guidance. |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory guidance and aligned identifiers to GDR-001. |
| 2026-07-27 | Hermes under explicit Founder direction | Aligned metadata, identifiers, stewardship, and authority references to GDR-001 and GDR-004 through [[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]]; removed duplicated semantics. |
