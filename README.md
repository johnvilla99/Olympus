# Mt. Olympus

Mt. Olympus is a portfolio-wide knowledge ecosystem for preserving memory, context, decisions, lessons learned, authority, and judgment across projects.

It is not intended to become another document dump. Its purpose is to help future humans and AI agents understand what was decided, why it mattered, who owns it, whether it is authoritative, and how prior experience should guide future work.

## Purpose

Modern AI-assisted work often suffers from continuity loss:

- new sessions lack prior reasoning
- agents rediscover old decisions
- implementation work reopens strategy
- lessons learned disappear into chat history
- documentation explains outcomes but not rationale
- knowledge is scattered across projects and tools

Mt. Olympus exists to reduce that loss by turning important knowledge into governed, durable assets.

## Core Concepts

| Concept | Role |
|---|---|
| Mt. Olympus | The overall knowledge ecosystem |
| Mnemosyne | The memory layer: accumulated knowledge, experience, and historical context |
| Metis | The judgment layer: reasoning over memory to support decisions and recommendations |
| The Muses | Durable domains of expertise: Architecture, Product, Governance, Knowledge Stewardship, Lessons Learned / Risk, User Experience, Engineering, Operations, and Marketing |
| Research | A cross-cutting activity that may support any Muse domain; not a tenth Muse |
| Agents | Temporary assistants that serve one or more Muses in specific sessions |
| Projects | Consumers and contributors of Knowledge Assets |

## Knowledge Assets

A Knowledge Asset is a durable unit of preserved knowledge that is useful for future reasoning, decision-making, continuity, or execution.

A Knowledge Asset is not merely a file. It is a governed container for meaning.

Knowledge Assets should explain:

- why the knowledge matters
- who owns it
- whether it is authoritative
- what decisions it informs
- what context would otherwise be lost
- how future agents should use it

## Initial Repository Scope

This repository begins as a governed knowledge foundation, not a production software platform.

In scope for the foundation:

- terminology
- governance model
- knowledge asset definitions
- authority model
- maturity lifecycle
- project/source-library guidance
- agent instruction patterns
- documentation standards
- decision backlog

Out of scope unless explicitly authorized:

- application UI
- database design
- graph implementation
- automation pipelines
- API contracts
- vector storage decisions
- vendor/tool selection

## Governance Principles

Mt. Olympus should make knowledge trustworthy, discoverable, and usable without becoming ceremonial paperwork.

Key rules:

- Founder direction has highest authority within the Founder’s authority.
- OLY-GOV-003 owns the decision authority hierarchy.
- Canonical and Governing assets outrank lower-authority records.
- Status and Authority Level are distinct and must be evaluated together.
- Exploratory ideas must remain clearly labeled until promoted.
- AI agents must check asset status and authority before relying on content.
- AI agents must distinguish approved decisions from inferred guidance.
- Conflicts between assets must be flagged, not silently resolved.
- Supporting documents should reference authoritative sources rather than duplicate rules.

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

| Authority Level | Meaning |
|---|---|
| Informational | Provides context only |
| Advisory | Recommended guidance, not binding |
| Canonical | Source of truth for a defined topic |
| Governing | Controls process, standards, or authority |

## Repository Structure

```text
Olympus/
├── README.md
├── LICENSE
├── docs/
│   ├── foundation/
│   ├── governance/
│   ├── concepts/
│   ├── decisions/
│   ├── muses/
│   ├── operations/
│   ├── research/
│   ├── lessons/
│   └── projects/
├── templates/
├── logs/
│   └── daily/
└── .cursor/
    └── rules/
```

## Current Governance Baseline

| Asset | Status / Authority | Purpose |
|---|---|---|
| OLY-GOV-001 | Approved / Advisory | Repository organization and placement |
| OLY-GOV-002 | Approved / Advisory | Knowledge Asset lifecycle and metadata |
| OLY-GOV-003 | Approved / Advisory | Decision authority, hierarchy, approval, and decision records |
| OLY-GOV-004 | Approved / Advisory | Session continuity |
| OLY-GOV-005 | Approved / Advisory | Authority-aware discovery and safe knowledge consumption |
| GDR-001 | Approved / Canonical | Olympus ID convention |
| OPM-001 | Approved / Advisory | Agent operating model |
| OPM-002 | Approved / Advisory | Knowledge capture workflow |
| OPM-003 | Approved / Advisory | Decision promotion and approval workflow |

## Initial Seed Assets

| Asset | Path |
|---|---|
| ACR-001: Mnemosyne, Metis, and The Muses | `docs/concepts/ACR-001_MNEMOSYNE_METIS_AND_THE_MUSES.md` |
| Foundation Brief | `docs/foundation/MT_OLYMPUS_FOUNDATION_BRIEF.md` |
| Knowledge Asset Model | `docs/foundation/KNOWLEDGE_ASSET_MODEL.md` |
| Project Instructions | `docs/foundation/MT_OLYMPUS_PROJECT_INSTRUCTIONS.md` |
| Muse Catalog | `docs/muses/MUSE_CATALOG_STARTER.md` |
| Decision Backlog | `docs/decisions/MT_OLYMPUS_DECISION_BACKLOG.md` |

## Product Guardrail

Do not let Mt. Olympus become a cathedral of paperwork.

The system wins only if it reduces confusion, preserves useful judgment, and helps future work move faster with greater confidence.

## Repository Status

The governed foundation is active. Exploratory concept work and future product / architecture decisions remain clearly separated from approved operating guidance.