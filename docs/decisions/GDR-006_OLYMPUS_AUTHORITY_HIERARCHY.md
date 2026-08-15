# Olympus Authority Hierarchy

> **Status:** Approved / Governing. This decision governs authority resolution for Olympus-owned knowledge and replaces duplicated hierarchy language in lower-authority assets.

## Metadata

| Field | Value |
|---|---|
| Decision ID | GDR-006 |
| Title | Olympus Authority Hierarchy |
| Classification | Decision Record |
| Decision Category | Governance |
| Status | Approved |
| Authority Level | Governing |
| Canonical Source | Yes |
| Owner | John S. Villasenor |
| Decider / Approver | John S. Villasenor |
| Created On | 2026-07-27 |
| Decided On | 2026-07-27 |
| Last Updated | 2026-08-15 |
| Review Cadence | As Needed |
| Related Assets | [[GDR-003_OLYMPUS_CONCEPTUAL_CAPABILITY_MODEL|GDR-003]]; [[GDR-004_EUNOMIA_ECOSYSTEM_STEWARDSHIP_ROLE|GDR-004]]; [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]]; [[GDR-009_CANONICAL_REPOSITORY_LOCATION|GDR-009]]; [[OLY-GOV-003_DECISION_RECORD_STANDARD|OLY-GOV-003]]; [[OLY-GOV-005_AGENT_KNOWLEDGE_DISCOVERY_STANDARD|OLY-GOV-005]]; [[OPM-001_OLYMPUS_AGENT_OPERATING_MODEL|OPM-001]] |
| Supersedes | N/A |
| Superseded By | N/A |
| AI Consumption | Required |
| Change Impact | High |

---

## Decision

For Olympus governance and Olympus-owned knowledge, authority resolves in this order, subject to scope and applicability:

1. **Explicit current Founder direction** from John within his authority.
2. **Governing assets** whose Status permits reliance.
3. **Canonical sources** whose Status permits reliance.
4. **Approved Advisory guidance and Approved decision records** not already covered above.
5. **Proposed** assets and decisions.
6. **Draft / Advisory** standards and operating models.
7. **Exploratory / Informational** concepts and other non-binding context.
8. **Continuity artifacts** such as handoffs and daily logs.
9. **Conversation context**.
10. **Assistant inference or general knowledge**.

Apply the metadata semantics in **[[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]]**. Apply safe discovery and conflict handling through **[[OLY-GOV-005_AGENT_KNOWLEDGE_DISCOVERY_STANDARD|OLY-GOV-005]]**.

## Governing Rules

- Establish the applicable scope before comparing authority. Project- or client-local authority remains local unless explicitly promoted.
- More specific applicable authority controls when sources have the same authority and compatible status.
- Observable repository or operational evidence establishes current facts; it is not an Authority Level and does not create or override a decision.
- Multiple competing Governing or Canonical sources for the same subject are a conflict requiring explicit resolution.
- Lower-authority assets must **reference this decision** rather than restate the hierarchy. They may define domain-specific procedures without reproducing this list.
- Agents may identify and recommend resolution; only the authorized human authority may approve a change in authority.

## Context

OLY-GOV-003, OPM-001, OLY-GOV-005, Governance Starter, and Cursor rules expressed similar but non-identical hierarchies. The duplication created ambiguity about precedence.

## Options Considered

| Option | Outcome |
|---|---|
| One Governing decision referenced by derivative assets | **Selected** — reduces drift and preserves one authority source |
| Keep hierarchy in [[OLY-GOV-003_DECISION_RECORD_STANDARD|OLY-GOV-003]] only | Rejected — OLY-GOV-003 is a Draft standard and decision-record procedure is narrower than ecosystem authority |
| Continue synchronized copies in multiple files | Rejected — duplication already produced drift |

## Consequences

- Active standards, operating models, prompts, indexes, and Cursor rules must remove or subordinate duplicate hierarchy language.
- Historical and exploratory records may retain prior wording when their status and context are clear.
- OLY-GOV-005 remains the operational discovery workflow; GDR-006 supplies its authority basis.

## Approval Context

Approved through explicit Founder direction in the E7CORE Hermes session on 2026-07-27.

## Follow-up Actions

- Replace duplicate active hierarchy sections with references to GDR-006.
- Use [[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]] in Phase 2 product work and later application-governance work.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-27 | John S. Villasenor | Approved one Governing Olympus authority hierarchy and the reference-over-repetition rule. |
| 2026-08-15 | Hermes under explicit Founder direction | Updated the active repository relationship from superseded GDR-007 to GDR-009 without changing the authority hierarchy. |
