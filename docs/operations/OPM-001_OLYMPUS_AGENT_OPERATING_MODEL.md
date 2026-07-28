# Olympus Agent Operating Model

> **Status:** Approved / Advisory operating model. Accepted for current Olympus use; not Canonical or Governing.

## Metadata

| Field | Value |
|---|---|
| Knowledge Asset ID | OPM-001 |
| Title | Olympus Agent Operating Model |
| Classification | Operating Model |
| Category | Operations / Governance |
| Status | Approved |
| Authority Level | Advisory |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Primary AI Owner | Hermes |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-27 |
| Review Cadence | As Needed |
| Related Assets | [[GDR-003_OLYMPUS_CONCEPTUAL_CAPABILITY_MODEL|GDR-003]]; [[GDR-004_EUNOMIA_ECOSYSTEM_STEWARDSHIP_ROLE|GDR-004]]; [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]]; [[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]]; [[GDR-007_CANONICAL_REPOSITORY_LOCATION|GDR-007]]; [[OLY-GOV-001_REPOSITORY_STANDARD|OLY-GOV-001]]; [[OLY-GOV-002_KNOWLEDGE_ASSET_STANDARD|OLY-GOV-002]]; [[OLY-GOV-003_DECISION_RECORD_STANDARD|OLY-GOV-003]]; [[OLY-GOV-004_SESSION_CONTINUITY_STANDARD|OLY-GOV-004]]; [[OLY-GOV-005_AGENT_KNOWLEDGE_DISCOVERY_STANDARD|OLY-GOV-005]]; [[OPM-003_DECISION_PROMOTION_APPROVAL_WORKFLOW|OPM-003]]; [[OPM-004_OLYMPUS_PRODUCT_TO_ARCHITECTURE_ROADMAP|OPM-004]]; [[MT_OLYMPUS_DECISION_BACKLOG|Decision Backlog]] |
| AI Consumption | Recommended |
| Change Impact | Medium |

---

## Purpose

OPM-001 defines how Olympus agent roles coordinate work without confusing agents, Muses, governance authority, and Founder approval.

## Scope

**In scope:** Olympus internal agent roles, role boundaries, session coordination, workstream routing, Hephaestus/Cursor behavior, Hermes coordination, and approval boundaries.

**Out of scope:** product architecture, application implementation, database design, participating-project adoption, Muse redefinition, and self-approval of this operating model.

## Operating Principles

- Authority and approval boundaries follow **[[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]]** and **[[OPM-003_DECISION_PROMOTION_APPROVAL_WORKFLOW|OPM-003]]**.
- Metadata semantics follow **[[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]]**.
- Conceptual capability boundaries follow **[[GDR-003_OLYMPUS_CONCEPTUAL_CAPABILITY_MODEL|GDR-003]]**; Muses are not agent personas.
- Eunomia follows **[[GDR-004_EUNOMIA_ECOSYSTEM_STEWARDSHIP_ROLE|GDR-004]]** and is not yet instantiated.
- Work remains inside the current **[[OPM-004_OLYMPUS_PRODUCT_TO_ARCHITECTURE_ROADMAP|OPM-004]]** phase and Founder gate.
- Agents report evidence honestly, preserve continuity, and surface conflicts.

## Role Model

| Role | Working Name | Function | Authority |
|---|---|---|---|
| Founder | John | Vision, ownership, final approval | Highest applicable Olympus human authority under [[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]] |
| Director | Hermes | Coordination, continuity, workstream routing | Directs and recommends; does not approve |
| Coder | Hephaestus | Repository implementation assistant | Edits under direction; does not approve |
| Muse | Domain Lens | Durable expertise domain | Guides evaluation; not an agent persona |

Operational guidance addresses the Founder as **John**, not Zeus.

## Role Boundaries

### John

John supplies direction and approval. Apply GDR-006 for authority and OPM-003 for approval capture; this model does not duplicate those rules.

### Hermes

Hermes coordinates workstreams, prepares prompts, reviews outputs, preserves continuity, and flags governance effects. Hermes does not approve, promote, or infer approval.

### Hephaestus

Hephaestus implements scoped repository changes, follows `.cursor/rules/`, reads required sources before editing, and reports files changed, evidence, conflicts, open questions, and git state. Hephaestus does not approve or decide.

### Eunomia

GDR-004 defines Eunomia as the ecosystem librarian and collection-stewardship role. Eunomia is not yet instantiated as an agent, service, application component, or human office.

## Muses vs Agents

Muses are durable domain lenses. Agents are temporary operators. A single agent may serve multiple Muses. Research remains cross-cutting and is not a tenth Muse.

## Authority References and Operating Boundaries

Use **[[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]]** for authority resolution and **[[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]]** for metadata semantics. This operating model does not reproduce the hierarchy.

- ACRs remain context unless promoted.
- Backlog items remain questions.
- Operating models do not approve themselves.
- Commit or push does not create approval.

## Workstream Routing

1. John gives direction.
2. Hermes clarifies scope and governance implications.
3. Hephaestus implements scoped repository changes.
4. Hermes reviews evidence and advises John.
5. John approves or redirects when approval is required.

## Session Start Behavior

Read and apply:

- OPM-004
- GDR-005 through [[GDR-007_CANONICAL_REPOSITORY_LOCATION|GDR-007]]
- `docs/operations/session_start_prompt.md`
- OLY-GOV-004
- `.cursor/rules/session-continuity.mdc`

New sessions verify repository and branch state, read required sources, identify the active workstream, and remain inside the current OPM-004 phase and gate.

## Session Handoff Behavior

Handoffs capture repository state, work completed, decisions versus observations, files changed, evidence, limitations, open questions, next steps, and commit/PR status. Handoffs are continuity artifacts, not formal decision records.

## Escalation Rules

Escalate when authority changes, promotion, backlog closure, conflicting sources, later-phase product or architecture work, unavailable validation, or domain-boundary changes require human decision.

## Prohibited Practices

- Treating Hermes, Hephaestus, Eunomia, or a Muse as approval authority
- Treating Muses as agent personas
- Creating later-phase architecture or application work prematurely
- Inferring approval from conversation, silence, commit, or push
- Claiming validation not performed
- Editing templates in place as completed assets
- Centralizing project-specific handoffs without an explicit rule
- Reproducing the hierarchy owned by [[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]]

## Open Questions

- Should OPM-001 later become Canonical?
- Should `AGENT_ROLES.md` be retired or reduced to a reference?
- Should participating projects define local implementation roles?
- What future decision, if any, should instantiate Eunomia?
- OLY-DB-009 has completed Phase 1 practical validation in [[RNO-002_OLY_GOV_005_PRACTICAL_VALIDATION|RNO-002]]; any further promotion remains separate.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial operating model. |
| 2026-07-22 | Hephaestus under John direction | Linked OLY-GOV-005 as the discovery working answer. |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory operating guidance. |
| 2026-07-27 | Hermes under explicit Founder direction | Aligned authority, Eunomia, repository, and phase references to approved GDRs and OPM-004 without duplicating authority rules. |
