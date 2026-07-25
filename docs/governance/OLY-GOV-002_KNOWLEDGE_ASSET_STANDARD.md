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
| Last Updated | 2026-07-25 |
| Review Cadence | As Needed |
| Related Assets | Foundation Brief; Knowledge Asset Model; OLY-GOV-001; OLY-GOV-003; OLY-GOV-004; OLY-GOV-005; GDR-001; ACR-001; ACR-002; Muse Catalog; Decision Backlog |
| AI Consumption | Required |
| Change Impact | High |

---

## Purpose

Make Knowledge Assets trustworthy, discoverable, maintainable, and safe for humans and AI agents to consume.

A Knowledge Asset is not merely a file. It is a governed container for meaning that preserves what is known, why it matters, who owns it, whether it is authoritative, and how future work should use it.

This standard prevents:

- Notes being mistaken for authoritative guidance
- Exploratory concepts being treated as implementation authority
- Assets lacking metadata needed for safe evaluation
- Duplicate or conflicting sources of truth
- Experience and lessons being lost when they have future decision value

## Scope

Applies to formal Knowledge Assets stored in the Olympus repository.

**In scope:** metadata, categories, Status, Authority Level, AI Consumption, creation, placement, promotion, maintenance, supersession, retirement, relationships, citation, and experience capture.

**Out of scope:** database schema, application UI, automation pipelines, external project standards unless adopted, and automatic promotion of any existing asset.

## Definition of a Knowledge Asset

A **Knowledge Asset** is a durable unit of preserved knowledge useful for future reasoning, decision-making, continuity, or execution.

A formal asset should help future humans or agents understand:

- Why it matters
- Who owns it
- Whether it is authoritative
- What decisions it informs
- What context would otherwise be lost
- How it should be used

## What Qualifies

Examples include:

| Type | Purpose |
|---|---|
| Concept Record | Preserve an emerging idea before it becomes a decision |
| Decision Record | Capture a proposed, approved, superseded, or retired decision and rationale |
| Governance Standard | Define rules for how work is done |
| Product Definition | Define user value, scope, principles, and outcomes |
| Architecture Definition | Define technical structure after product and governance clarity |
| Lesson Learned | Preserve experience from success, failure, or surprise |
| Research Note | Capture evidence and analysis |
| Operating Model | Define roles, responsibilities, and workflows |
| Handoff / Continuity Artifact | Preserve current state and session continuity |

An asset qualifies when it has future value, accountable ownership, honest Status and Authority Level, and appropriate metadata.

## What Does Not Qualify

- Scratch notes with no future decision value
- Raw chat transcripts unless curated
- Duplicate copies without an authoritative-source reference
- Temporary logs unless promoted
- Application source code and build artifacts
- Secrets, credentials, or environment values
- Vague ideas without context, owner, or future use
- Templates and directory indexes

## Asset Categories and Placement

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

Research is a cross-cutting activity, not a tenth Muse. Research notes may identify one or more relevant Muse lenses.

## Identifier Convention

The official Olympus identifier convention is defined by **GDR-001**, the Approved / Canonical source.

- Use the prefix and three-digit numbering rules defined by GDR-001.
- IDs are stable once assigned.
- Retired or superseded IDs are not reused.
- Existing IDs remain valid.
- New prefixes require governance review and explicit Founder approval.

This standard does not duplicate the full prefix table because GDR-001 owns that rule.

## Required Metadata

Every formal Knowledge Asset should include:

| Field | Meaning |
|---|---|
| Knowledge Asset ID | Stable identifier governed by GDR-001 |
| Title | Human-readable name |
| Classification | Asset type |
| Category | Knowledge domain |
| Status | Maturity state |
| Authority Level | Binding weight |
| Canonical Source | Yes or No |
| Owner | Accountable human owner |
| Primary AI Owner | Stewardship role, if any |
| Created On | Creation date |
| Last Updated | Latest material update |
| Review Cadence | Expected review rhythm |
| Related Assets | Dependencies, lineage, and related records |
| AI Consumption | Required, Recommended, Optional, or Restricted |
| Change Impact | Low, Medium, or High |

Seed assets may be completed on their next substantive edit. Do not backfill unknown metadata speculatively.

## Status Model

| Status | Meaning |
|---|---|
| Exploratory | Emerging idea; not a decision and not binding |
| Draft | Being shaped into a usable artifact |
| Proposed | Ready for review or approval |
| Approved | Accepted as current guidance |
| Canonical | Source of truth for a defined topic |
| Superseded | Replaced by a newer asset and preserved for history |
| Retired | No longer active and preserved with rationale |

Decision Records use only the statuses defined by OLY-GOV-003.

## Authority Levels

| Level | Meaning | Agent Behavior |
|---|---|---|
| Informational | Provides context only | May inform reasoning; not binding |
| Advisory | Recommended guidance, not binding | Should be weighed against higher authority |
| Canonical | Source of truth for a defined topic | Prefer over lower-authority assets on that topic |
| Governing | Controls process, standards, or authority | Highest repository-level guidance after Founder direction |

Status and Authority Level must be evaluated together. Approved does not automatically mean Canonical or Governing.

## Canonical Source Rules

- Prefer one Canonical source per defined subject.
- Duplicate content must identify the authoritative source.
- Canonical authority requires explicit Founder approval.
- Exploratory ACRs are not Canonical.
- Root README is a front door, not the source of truth for all topics.
- GDR-001 is the Canonical source for identifiers.

## AI Consumption Rules

Agents must:

1. Check Status.
2. Check Authority Level.
3. Apply the decision authority hierarchy in OLY-GOV-003.
4. Apply the discovery and safe-consumption rules in OLY-GOV-005.
5. Cite or reference material sources.
6. Distinguish approved decisions from conversational or inferred guidance.
7. Flag conflicts rather than silently resolving them.
8. Respect Restricted assets.

| Value | Meaning |
|---|---|
| Required | Must be read and applied when working in its domain |
| Recommended | Should be consulted when relevant |
| Optional | May be consulted for context |
| Restricted | Must not be used or surfaced without permission |

## Asset Creation Rules

- Start from the appropriate template when useful.
- Assign an ID under GDR-001.
- Complete required metadata.
- Set honest initial Status and Authority Level.
- Include purpose, context, authority notes, AI usage guidance, related assets, open questions, and change history where appropriate.
- Create an asset only when it improves future reasoning, decisions, continuity, or execution.
- Keep one primary concern per asset and link related content.

## Minimum Bar for Proposed

An asset may move to Proposed when:

- Required metadata is complete or explicitly marked TBD with reason
- Purpose and context are clear
- Owner is known
- Status and Authority Level are explicit
- Related assets are listed or marked None/TBD
- AI Consumption is set
- Open questions are captured
- Change History exists
- The asset has future value

Proposed means ready for review, not Approved.

## Promotion Rules

Typical path:

```text
Exploratory idea → Concept Record → Proposed Decision or Standard → Approved Artifact → Canonical Source, where appropriate
```

- Not every concept should be promoted.
- Promotion requires a clear problem, known owner, downstream value, and maintenance responsibility.
- Only John may approve Approved, Canonical, or Governing status during the foundation phase.
- Agents may recommend and draft but cannot approve.
- Approval must be explicit.
- Update related assets, indexes, and backlog entries when promotion occurs.
- Significant promotions should be captured in the appropriate decision record or change history.

## Review and Maintenance

- Set a review cadence.
- Update Last Updated on material change.
- Record meaningful changes in Change History.
- Review stale or high-impact assets before relying on them.
- Owners are accountable for accurate Status and Authority Level.

## Supersession and Retirement

- Preserve superseded assets and link to replacements.
- Retired assets must explain why they are inactive.
- Do not delete historical assets casually.
- Update Related Assets on both predecessor and successor.

## Relationship and Citation Rules

Recognized relationship types include `informs`, `supersedes`, `contradicts`, `depends_on`, `references`, `replaces`, and `related_to`.

Relationships are currently expressed through metadata and links. Graph implementation remains deferred.

## Experience Capture

- Experience often begins as a lesson, observation, failure, surprise, tradeoff, or pattern.
- Not every experience event becomes a formal asset.
- Capture lightly in handoffs and logs first when appropriate.
- Promote durable experience to a Lesson Learned or other asset when it has future decision value.
- Include what happened, why it mattered, the lesson, future use, related assets, and confidence where useful.
- A formal Experience Note type remains deferred.

## Prohibited Practices

- Treating every note as authoritative
- Creating formal assets with missing required metadata
- Duplicating authoritative content without a source reference
- Treating exploratory ACRs as implementation authority
- Promoting assets without Founder approval
- Deleting superseded assets without preservation rationale
- Storing secrets or credentials
- Creating paperwork without future value
- Assigning multiple conflicting Canonical sources to one subject
- Repeating a rule already owned by another authoritative artifact when a reference is sufficient

## Exceptions

Exceptions require explicit Founder approval and must be documented in the affected asset or an appropriate decision record.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial draft |
| 2026-07-05 | John S. Villasenor | Added working guidance for identifiers, Research, promotion, metadata, placement, and experience capture |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory guidance; aligned identifiers to GDR-001, decision authority to OLY-GOV-003, and Research to the cross-cutting model |