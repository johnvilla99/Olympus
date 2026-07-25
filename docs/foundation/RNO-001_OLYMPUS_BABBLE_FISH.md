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
| Last Updated | 2026-07-25 |
| Review Cadence | As Needed |
| Related Assets | OLY-GOV-002; OLY-GOV-003; OPM-001; OPM-002; OPM-003; GDR-003; GDR-004; Muse Catalog; Decision Backlog |
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

| Term | Meaning |
|---|---|
| Draft | Being shaped; not approved |
| Proposed | Ready for review; not approved |
| Approved | Accepted as current guidance; requires explicit John approval |
| Canonical | Source of truth for a defined subject; requires explicit John approval |
| Governing | Controls process or authority; requires explicit John approval |
| Exploratory | Emerging idea; not binding; not valid for Decision Records |
| Superseded | Replaced but preserved |
| Retired | No longer active but preserved |
| Advisory | Recommended guidance, not binding |
| Informational | Context only |
| AI Consumption | How agents should use an asset: Required, Recommended, Optional, Restricted |
| Change Impact | Expected scrutiny or risk of changing an asset: Low, Medium, High |

## Operating Model Terms

| Term | Meaning |
|---|---|
| John | Founder and final approval authority |
| Hermes | Director agent role: coordination, continuity, prompts, review, and routing |
| Hephaestus | Coder agent role: Cursor implementation assistant |
| Eunomia | Olympus ecosystem librarian and collection-stewardship role defined by GDR-004; not yet instantiated as an active agent or application component |
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

## Common Repository Terms

| Term | Meaning |
|---|---|
| `docs/` | Governed Knowledge Asset area |
| `templates/` | Starter templates, not completed assets |
| `logs/daily/` | Daily logs and completed Olympus handoffs |
| `.cursor/rules/` | Hephaestus operating rules |
| `README.md` | Directory index or front door, not necessarily Canonical authority |
| SSOT | Single Source of Truth, if used |
| RAG | Retrieval-Augmented Generation, not the same as Mnemosyne |

## Open Questions

- Should Olympus create a dedicated `REF-*` prefix for reference notes and glossaries?
- Should Babble Fish later become Canonical?
- Should project-specific Babble Fish documents exist for participating repositories?
- Should Babble Fish be required reading for new agents?
- Is `RNO-*` the right prefix for glossary and reference notes?

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial Draft / Advisory abbreviation and terminology reference |
| 2026-07-05 | John S. Villasenor | Approved Babble Fish as the living Olympus abbreviation and terminology reference; renamed file with `RNO-001` prefix |
| 2026-07-25 | John S. Villasenor | Replaced the retired Curator terminology with Eunomia and added GDR-003/GDR-004 concept boundaries |
