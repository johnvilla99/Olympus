# Olympus Babble Fish

> **Status:** Draft / Advisory reference note. Not Approved, Canonical, or Governing.

## Metadata

| Field | Value |
|---|---|
| Knowledge Asset ID | RNO-001 |
| Title | Olympus Babble Fish |
| Classification | Reference Note |
| Category | Foundation / Knowledge Stewardship |
| Status | Draft |
| Authority Level | Advisory |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Primary AI Owner | Hermes |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-05 |
| Review Cadence | As Needed |
| Related Assets | OLY-GOV-002; OLY-GOV-003; OPM-001; OPM-002; OPM-003; Muse Catalog; Decision Backlog |
| Muse Lenses | Knowledge Stewardship; Governance; Operations |
| AI Consumption | Recommended |
| Change Impact | Low |

---

## Purpose

This document translates Olympus **abbreviations, prefixes, role names, workflow shorthand, and recurring terms** so future humans and AI agents can decode repository language quickly without rediscovery.

It is a **reference glossary**, not a decision record or governing standard.

## How to Use This Document

- Use as a **quick decoder** when encountering unfamiliar Olympus shorthand.
- Do **not** treat this document as authority over standards or decision records.
- If this document conflicts with **OLY-GOV**, **OPM**, or **decision records**, defer to the higher-authority source.
- Update when new prefixes, roles, workflows, or shorthand are introduced.

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
| RNO | Research Note | Research, evidence, analysis — and currently this glossary/reference note |
| OPM | Operating Model | Operating workflows, role models, and stewardship models |
| HND | Handoff / Continuity Artifact | Durable handoff or continuity artifacts if promoted |
| OLY-DB | Olympus Decision Backlog item | Backlog IDs track open, deferred, or partially addressed questions. They are not decision records and do not indicate approval |

## Governance and Status Terms

| Term | Meaning |
|---|---|
| Draft | Being shaped; not approved |
| Proposed | Ready for review; not approved |
| Approved | Accepted as current guidance; requires explicit John approval |
| Canonical | Source of truth for a defined subject; requires explicit John approval |
| Governing | Controls process/authority; requires explicit John approval |
| Exploratory | Emerging idea; not binding; not valid for Decision Records |
| Superseded | Replaced but preserved |
| Retired | No longer active but preserved |
| Advisory | Recommended guidance, not binding |
| Informational | Context only |
| AI Consumption | How agents should use an asset: Required, Recommended, Optional, Restricted |
| Change Impact | Expected scrutiny/risk of changing an asset: Low, Medium, High |

## Operating Model Terms

| Term | Meaning |
|---|---|
| John | Founder and final approval authority |
| Hermes | Director role: coordination, continuity, prompts, review, routing |
| Hephaestus | Coder role: Cursor implementation assistant |
| Curator | Proposed stewardship concept; not active/approved yet |
| Founder approval | Explicit John approval — not inferred from silence, commit, or push |
| Commit/push | Repository action; not approval unless John explicitly says so |

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

- **Muses** are durable domain lenses, not agents.
- **Agents** may serve one or more Muses.
- **Research** is cross-cutting — not currently a tenth Muse.

## Session / Workflow Terms

| Term | Meaning |
|---|---|
| Handoff | Continuity artifact for future session resume |
| Daily Log | Chronological operational note in `logs/daily/` |
| Evidence Packet | Section within handoff documenting what changed and how it was validated |
| Capture Review | Handoff section for routing candidate knowledge |
| Backlog Item | Open question — not a decision |
| Working Answer | Draft / Advisory guidance useful now, not Approved |
| Candidate Knowledge Asset | Captured knowledge that may deserve promotion |
| Decision Candidate | Possible future decision not yet formalized |
| Tier 3 | Deferred product / architecture questions |

## Common Repository Terms

| Term | Meaning |
|---|---|
| `docs/` | Governed knowledge asset area |
| `templates/` | Starter templates — not completed assets |
| `logs/daily/` | Daily logs and filled Olympus handoffs |
| `.cursor/rules/` | Hephaestus operating rules |
| `README.md` | Directory index or front door — not necessarily canonical authority |
| SSOT | Single Source of Truth, if used |
| RAG | Retrieval-Augmented Generation — not the same as Mnemosyne |
| Mnemosyne | Memory layer concept |
| Metis | Judgment layer concept |

## Open Questions

- Should Olympus create a dedicated **`REF-*`** prefix for reference notes and glossaries?
- Should Babble Fish later become **Canonical**?
- Should project-specific Babble Fish documents exist for participating repos?
- Should the Babble Fish document be **required reading** for new agents?
- Is **`RNO-*`** the right prefix fit for glossary/reference notes?

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial Draft / Advisory abbreviation and terminology reference |
