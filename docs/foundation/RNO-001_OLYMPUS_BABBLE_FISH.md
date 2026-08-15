# Olympus Babble Fish

> **Status:** Approved / Advisory living reference. This document is approved as the Olympus abbreviation and terminology decoder, but it is not Canonical or Governing. It should be updated as new terms are discovered.

## Metadata

| Field | Value |
|---|---|
| Knowledge Asset ID | RNO-001 |
| Title | Olympus Babble Fish |
| Classification | Reference Note |
| Category | Foundation / Knowledge Stewardship |
| Status | Approved |
| Authority Level | Advisory |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Primary AI Owner | Hermes |
| Created On | 2026-07-05 |
| Last Updated | 2026-08-15 |
| Review Cadence | As Needed |
| Related Assets | [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]]; [[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]]; [[GDR-009_CANONICAL_REPOSITORY_LOCATION|GDR-009]]; [[OLY-GOV-002_KNOWLEDGE_ASSET_STANDARD|OLY-GOV-002]]; [[OLY-GOV-003_DECISION_RECORD_STANDARD|OLY-GOV-003]]; [[OPM-001_OLYMPUS_AGENT_OPERATING_MODEL|OPM-001]]; [[OPM-002_KNOWLEDGE_CAPTURE_WORKFLOW|OPM-002]]; [[OPM-003_DECISION_PROMOTION_APPROVAL_WORKFLOW|OPM-003]]; [[GDR-003_OLYMPUS_CONCEPTUAL_CAPABILITY_MODEL|GDR-003]]; [[GDR-004_EUNOMIA_ECOSYSTEM_STEWARDSHIP_ROLE|GDR-004]]; [[MUSE_CATALOG_STARTER|Muse Catalog]]; [[MT_OLYMPUS_DECISION_BACKLOG|Decision Backlog]]; [[ACR-003_OLYMPUS_AS_PROJECT_INTELLIGENCE|ACR-003]]; [[RNO-003_PROJECT_INTELLIGENCE_PRODUCT_HYPOTHESES|RNO-003]] |
| Muse Lenses | Knowledge Stewardship; Governance; Operations |
| AI Consumption | Recommended |
| Change Impact | Low |

---

## Purpose

This document translates Olympus abbreviations, prefixes, role names, workflow shorthand, and recurring terms so future humans and AI agents can decode repository language quickly without rediscovery.

It is a reference glossary, not a decision record or governing standard.

## How to Use This Document

- Use it as the approved quick decoder for Olympus abbreviations, prefixes, role names, and shorthand.
- Update it when new prefixes, roles, workflows, or shorthand are introduced.
- Do not treat it as authority over governance standards or decision records.
- If it conflicts with an OLY-GOV artifact or promoted decision, defer to the higher-authority source.
- Terms explicitly marked **Exploratory** describe current working language, not approved product positioning or architecture.

## Asset Prefixes

| Term | Meaning | Notes |
|---|---|---|
| ACR | Architectural Concept Record | Exploratory concept records, usually in `docs/concepts/` |
| OLY-GOV | Olympus Governance Standard | Governance standards in `docs/governance/` |
| ADR | Architecture Decision Record | Formal architecture decisions |
| PDR | Product Decision Record | Formal product decisions |
| GDR | Governance Decision Record | Formal governance decisions |
| ODR | Operating Decision Record | Formal operating/process decisions |
| LLR | Lesson Learned Record | Lessons from failure, surprise, experience, or retrospective |
| RNO | Research Note | Research, evidence, analysis, and currently this glossary/reference note |
| OPM | Operating Model | Operating workflows, role models, and stewardship models |
| HND | Handoff / Continuity Artifact | Durable handoff or continuity artifacts if promoted |
| OLY-DB | Olympus Decision Backlog item | Tracks open, deferred, partially addressed, and resolved questions; not a decision record |

## Governance and Status Terms

Use **[[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]]** for authoritative Status, Authority Level, and Canonical Source semantics. This glossary decodes common wording; it does not redefine those dimensions.

**Banner shorthand note:** Human-readable banners such as `Approved / Canonical` or `Approved / Governing` combine a lifecycle Status with an Authority Level for scannability. The metadata table remains authoritative. Do not treat the banner as a single combined Status value. Canonical is not a lifecycle Status.

### Lifecycle Status (GDR-005)

| Term | Meaning |
|---|---|
| Exploratory | Emerging idea; not binding; not valid for Decision Records |
| Draft | Being shaped; not approved |
| Proposed | Ready for review; not approved |
| Approved | Accepted as current guidance; requires explicit John approval |
| Superseded | Replaced but preserved |
| Retired | No longer active but preserved |

### Authority Level (GDR-005)

| Term | Meaning |
|---|---|
| Informational | Context only |
| Advisory | Recommended guidance, not binding |
| Canonical | Binding source of truth for a defined subject; requires explicit John approval |
| Governing | Controls process or authority resolution; requires explicit John approval |

### Canonical Source (GDR-005)

| Term | Meaning |
|---|---|
| Canonical Source | Separate `Yes` / `No` designation identifying whether the asset is the source of truth for its defined subject — independent of Status and Authority Level |

### Other governance terms

| Term | Meaning |
|---|---|
| AI Consumption | How agents should use an asset: Required, Recommended, Optional, Restricted |
| Change Impact | Expected scrutiny or risk of changing an asset: Low, Medium, High |
| Superseded decision | Preserved historical decision that has been replaced and is no longer the current source for its subject |

## Operating Model Terms

| Term | Meaning |
|---|---|
| John | Founder and final approval authority |
| Hermes | Director agent role: coordination, continuity, prompts, review, and routing |
| Hephaestus | Coder agent role: Cursor implementation assistant |
| Eunomia | Olympus ecosystem librarian and collection-stewardship role defined by [[GDR-004_EUNOMIA_ECOSYSTEM_STEWARDSHIP_ROLE|GDR-004]]; not yet instantiated as an active agent or application component |
| Curator | Retired working name for the role now defined as Eunomia; preserve only in historical context |
| Founder approval | Explicit John approval, not inferred from silence, commit, or push |
| Commit / push | Repository action; not approval unless John explicitly says so |

## Ecosystem Concept Terms

| Term | Meaning |
|---|---|
| Olympus | The governed knowledge ecosystem; not synonymous with a future Olympus application |
| Mnemosyne | Cross-cutting ecosystem memory capability |
| Metis | Cross-cutting ecosystem judgment capability |
| Eunomia | Cross-collection librarian and knowledge-health stewardship role |
| Muse | Durable domain lens and domain-stewardship capability; not an agent |

GDR-003 is Canonical for Olympus, Mnemosyne, Metis, and the Muses. GDR-004 is Canonical for Eunomia.

## Phase 2 Product Terms

These terms are useful working language from ACR-003 and RNO-003. Unless separately promoted, they remain **Exploratory**.

| Term | Working meaning | Authority posture |
|---|---|---|
| Project Intelligence | Governed ability to understand a project's evolving state, knowledge, decisions, relationships, risks, and history across tools | Exploratory working market/product term; not approved category positioning |
| Governed memory | Preserved knowledge whose status, authority, provenance, scope, relationships, and history remain inspectable | Conceptual shorthand consistent with existing Olympus governance; not a new Authority Level |
| Authority-aware judgment | Applying governed sources with explicit attention to authority, conflicts, provenance, uncertainty, experience, and required human decisions | Current Phase 2 differentiation hypothesis; not an approved product claim |
| Continuous Knowledge Integrity | Working concept in which project changes trigger evaluation of whether governed knowledge, decisions, relationships, and guidance remain accurate and consistent | Exploratory; not an approved workflow or automation requirement |
| Olympus Core | Working term for reusable Olympus governance, memory, judgment, relationship, continuity, and agent-boundary capabilities that may be shared across instances | Exploratory; exact boundary is OLY-DB-020 |
| Project Instance | Working term for project-specific Olympus context, assets, repositories, decisions, integrations, ownership, constraints, and lessons | Exploratory; exact boundary is OLY-DB-020 |
| Documentation / Knowledge Integrity Steward | Narrow possible wedge in which changes are evaluated for impact on governed knowledge and proposed updates | Exploratory product wedge, not the long-term product definition |
| Project Intelligence positioning | Possible external framing for Olympus | Open under OLY-DB-018; not approved |

RNO-003 currently concludes that generic cross-tool intelligence, knowledge graphs, engineering intelligence, and documentation automation already have substantial market overlap. The strongest surviving Olympus differentiation hypothesis is governed memory plus authority-aware judgment, but that remains subject to validation and Product Gate approval.

## Muse Terms

| Muse | Domain |
|---|---|
| Urania | Architecture |
| Calliope | Product |
| Polyhymnia | Governance |
| Clio | Knowledge Stewardship |
| Melpomene | Lessons Learned / Risk |
| Erato | User Experience |
| Euterpe | Engineering |
| Terpsichore | Operations |
| Thalia | Marketing |

Additional notes:

- Muses are durable domain lenses, not agents.
- Agents may serve one or more Muses.
- Research is cross-cutting, not a tenth Muse.
- Eunomia does not replace Clio or any other Muse; Eunomia stewards collection health across domains, while Muses steward domain meaning and quality.

## Session / Workflow Terms

| Term | Meaning |
|---|---|
| Handoff | Continuity artifact for future session resume |
| Daily Log | Chronological operational note in `logs/daily/` |
| Evidence Packet | Section within a handoff documenting what changed and how it was validated |
| Capture Review | Handoff section for routing candidate knowledge |
| Backlog Item | Open or tracked question; not a decision |
| Working Answer | Non-canonical guidance useful for current work |
| Candidate Knowledge Asset | Captured knowledge that may deserve promotion |
| Decision Candidate | Possible future decision not yet formalized |
| Tier 3 | Deferred product or architecture question |
| Stewardship Health | Advisory Eunomia assessment such as Healthy, At Risk, Unhealthy, Not Decision-Ready, or Review Required |
| Product Gate | OPM-004 Founder gate that approves Product Vision, MVP boundary, non-goals, prioritized capabilities, outcomes, and sufficient product requirements before Application Governance begins |

## Common Repository Terms

| Term | Meaning |
|---|---|
| `docs/` | Governed Knowledge Asset area |
| `templates/` | Starter templates, not completed assets |
| `logs/daily/` | Daily logs and completed Olympus handoffs |
| `.cursor/rules/` | Hephaestus operating rules |
| `README.md` | Directory index or front door, not necessarily Canonical authority |
| Active repository | `johnvilla99/Olympus` under GDR-009 |
| SSOT | Single Source of Truth, if used |
| RAG | Retrieval-Augmented Generation, not the same as Mnemosyne |

## Open Questions

- Should Olympus create a dedicated `REF-*` prefix for reference notes and glossaries?
- Should Babble Fish later become Canonical?
- Should project-specific Babble Fish documents exist for participating repositories?
- Should Babble Fish be required reading for new agents?
- Is `RNO-*` the right prefix for glossary and reference notes?
- Which Phase 2 product terms, if any, should eventually be promoted into approved product language?

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial Draft / Advisory abbreviation and terminology reference |
| 2026-07-05 | John S. Villasenor | Approved Babble Fish as the living Olympus abbreviation and terminology reference; renamed file with `RNO-001` prefix |
| 2026-07-25 | John S. Villasenor | Replaced the retired Curator terminology with Eunomia and added GDR-003/GDR-004 concept boundaries |
| 2026-07-27 | Hermes under explicit Founder direction | Separated Status, Authority Level, and Canonical Source per [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]]; clarified banner shorthand; retained Curator as retired term only |
| 2026-08-15 | Hermes under explicit Founder direction | Added GDR-009 repository terminology and Phase 2 exploratory terms from ACR-003/RNO-003 while preserving their non-binding status. |
