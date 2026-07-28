# Olympus ID Convention

> **Status:** Approved / Canonical. This decision is the source of truth for Olympus Knowledge Asset and decision-record identifiers.

## Metadata

| Field | Value |
|---|---|
| Decision ID | GDR-001 |
| Title | Olympus ID Convention |
| Classification | Decision Record |
| Decision Category | Governance |
| Status | Approved |
| Authority Level | Canonical |
| Canonical Source | Yes |
| Owner | John S. Villasenor |
| Decider / Approver | John S. Villasenor |
| Created On | 2026-07-05 |
| Decided On | 2026-07-25 |
| Last Updated | 2026-07-25 |
| Review Cadence | As Needed |
| Related Assets | [[OLY-GOV-001_REPOSITORY_STANDARD|OLY-GOV-001]]; [[OLY-GOV-002_KNOWLEDGE_ASSET_STANDARD|OLY-GOV-002]]; [[OLY-GOV-003_DECISION_RECORD_STANDARD|OLY-GOV-003]]; [[OPM-003_DECISION_PROMOTION_APPROVAL_WORKFLOW|OPM-003]]; OLY-DB-017; [[MT_OLYMPUS_DECISION_BACKLOG|Decision Backlog]]; [[RNO-001_OLYMPUS_BABBLE_FISH|RNO-001]] |
| Supersedes | N/A |
| Superseded By | N/A |
| AI Consumption | Required |
| Change Impact | Medium |

---

## Decision

Olympus uses stable, prefix-based, three-digit identifiers for formal Knowledge Assets and decision records.

### Approved prefix convention

| Prefix | Asset Type |
|---|---|
| ACR | Architectural Concept Record |
| OLY-GOV | Olympus Governance Standard |
| ADR | Architecture Decision Record |
| PDR | Product Decision Record |
| GDR | Governance Decision Record |
| ODR | Operating Decision Record |
| LLR | Lesson Learned Record |
| RNO | Research Note |
| OPM | Operating Model |
| HND | Handoff / Continuity Artifact |

### Approved rules

- Use sequential **three-digit** numbering within each prefix (for example, `GDR-001`, `OPM-003`).
- IDs are **stable once assigned**.
- **Retired** or **superseded** IDs are **not reused**.
- **Existing IDs** remain valid.
- **New prefixes** require governance review and explicit Founder approval.
- Status and Authority Level determine how an asset may be used; an ID prefix does not confer authority by itself.

## Context

The ID convention was initially captured as Draft / Advisory working guidance in [[OLY-GOV-002_KNOWLEDGE_ASSET_STANDARD|OLY-GOV-002]] and related standards. It has since been used consistently across Olympus governance standards, operating models, decisions, concepts, research, continuity practices, templates, and repository navigation.

**OLY-DB-017** tracked formal promotion of the convention. John explicitly approved the convention as official and Canonical on 2026-07-25. This decision resolves OLY-DB-017.

A formal **GDR** is required because identifiers affect citation, supersession, discovery, continuity, and AI consumption across all future Olympus Knowledge Assets and decisions.

## Options Considered

| Option | Summary | Pros | Cons |
|---|---|---|---|
| Option A | Prefix-based IDs by asset type | Clear, scalable, human-readable, aligns with existing assets | Requires maintaining prefix discipline |
| Option B | Single global OLY-* sequence | Simple global numbering | Harder to identify asset type quickly |
| Option C | Directory-based filenames without stable IDs | Easy at first | Weak for citations, supersession, and AI consumption |
| Option D | Defer formal ID convention | Avoids premature governance | Increases drift as assets grow |

## Rationale

**Option A** is approved because it:

- Is already used throughout the repository
- Supports AI consumption and safe source evaluation
- Supports citation and handoff continuity
- Distinguishes decisions from concepts, standards, operations, lessons, and research
- Aligns with OLY-GOV-001, OLY-GOV-002, and OLY-GOV-003
- Reduces accidental authority confusion when status and authority are evaluated alongside asset type

## Consequences

- Future formal assets must use the approved prefix convention.
- Templates, repository indexes, Cursor rules, and related standards must reference GDR-001 as the Canonical source rather than restating the convention as provisional guidance.
- Existing IDs remain valid.
- The convention creates modest governance overhead for ID assignment and maintenance.
- New prefixes should be rare and require explicit review.

## Risks

- Too many prefixes could create confusion.
- **RNO** may not perfectly fit Babble Fish and other reference documents; that question remains open and does not invalidate the convention.
- **HND** may need future clarification for promoted versus operational handoffs.
- Prefixes could imply authority if Status and Authority Level are ignored.
- Agents may over-focus on IDs instead of content value and rationale.

## Approval Record

- **Approver:** John S. Villasenor
- **Approval date:** 2026-07-25
- **Approval context:** Founder review confirmed that the convention is official, reflects established repository practice, and should be promoted.
- **Approved authority:** Canonical
- **Commit/push distinction:** Repository persistence alone does not constitute approval; this record captures explicit Founder approval.

## Follow-up Actions

| Action | Owner | Status |
|---|---|---|
| Update OLY-DB-017 as resolved through [[GDR-001_OLYMPUS_ID_CONVENTION|GDR-001]] | Hermes / repository steward | Required |
| Replace provisional ID-convention language in related standards with references to GDR-001 | Hermes / repository steward | Required |
| Keep templates, indexes, and Cursor rules aligned | Repository steward | Ongoing |
| Consider whether Babble Fish needs a future `REF-*` prefix | Hermes / John | Deferred |

## Supersedes / Superseded By

| Relationship | Asset ID | Notes |
|---|---|---|
| Supersedes | N/A | First formal ID convention decision |
| Superseded By | N/A | N/A |

## Open Questions

- Should Olympus later create a **`REF-*`** prefix for reference notes and glossaries?
- Should **`HND-*`** be used for every handoff or only promoted continuity artifacts?
- Should participating project repositories adopt the same prefix convention?

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial Draft GDR for Olympus ID convention |
| 2026-07-05 | John S. Villasenor | Promoted GDR-001 from Draft to Proposed for John review; not Approved |
| 2026-07-25 | John S. Villasenor | Approved GDR-001 as the Canonical Olympus ID convention; resolved OLY-DB-017 |