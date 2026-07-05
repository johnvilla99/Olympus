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
| The Muses | Durable domains of expertise such as Architecture, Product, Governance, Research, UX, Engineering, Operations, Marketing, and Knowledge Stewardship |
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

In scope for the initial foundation:

- terminology
- governance model
- knowledge asset definitions
- authority model
- maturity lifecycle
- project/source-library guidance
- agent instruction patterns
- documentation standards
- decision backlog

Out of scope for the initial foundation:

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

- Founder direction has highest authority.
- Canonical and governing assets outrank exploratory records.
- Exploratory ideas must remain clearly labeled until approved.
- AI agents must check asset status before relying on content.
- AI agents should distinguish approved decisions from inferred guidance.
- Conflicts between assets should be flagged, not silently resolved.

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

## Recommended Starting Structure

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
│   └── operations/
└── templates/
```

## Initial Seed Assets

The first foundation documents should include:

- ACR-001: Mnemosyne, Metis, and The Muses
- Foundation Brief
- Knowledge Asset Model
- Governance Starter
- Muse Catalog Starter
- Decision Backlog

## Product Guardrail

Do not let Mt. Olympus become a cathedral of paperwork.

The system wins only if it reduces confusion, preserves useful judgment, and helps future work move faster with greater confidence.

## Repository Status

This repository is in foundation setup.

Initial priority: establish the GitHub repository, preserve the seed knowledge assets, and create enough governance structure for future agents to consume the project safely.
