# Architectural Concept Record (ACR-003)

# Olympus as Project Intelligence

## A Deployable Intelligence Layer for Governed Project Knowledge

| Metadata | Value |
|---|---|
| **Knowledge Asset ID** | ACR-003 |
| **Title** | Olympus as Project Intelligence |
| **Classification** | Architectural Concept Record |
| **Category** | Product / Knowledge Management / Conceptual Architecture |
| **Status** | Exploratory |
| **Authority Level** | Informational |
| **Canonical Source** | No |
| **Version** | 0.1.0 |
| **Owner** | John S. Villasenor |
| **Primary AI Owner** | Hermes |
| **Created On** | 2026-08-15 |
| **Last Updated** | 2026-08-15 |
| **Review Cadence** | As Needed |
| **AI Consumption** | Recommended |
| **Change Impact** | High |
| **Related Assets** | ACR-001; ACR-002; MT_OLYMPUS_FOUNDATION_BRIEF; OLY-GOV-002; OPM-001; OPM-002; OPM-003; RNO-003 |
| **Tags** | olympus, project-intelligence, institutional-memory, knowledge-continuity, governance, product-thesis, change-impact, agents |

---

# Status

This document captures an emerging product and architecture thesis.

It is **not** a product decision, market commitment, implementation plan, MVP specification, or commercial strategy.

Its purpose is to preserve the conceptual step from Olympus as a portfolio-wide knowledge continuity system to Olympus as a potentially deployable **Project Intelligence** model that can be instantiated across projects and, eventually, organizations.

Nothing in this record should be treated as implementation authority until promoted through the appropriate Olympus governance process.

---

# Origin

ACR-001 established the core Olympus philosophy:

- preserve knowledge rather than documents
- preserve decisions and context
- treat experience as a first-class knowledge asset
- separate memory, judgment, and domain expertise
- enable future humans and AI agents to reason over accumulated knowledge

ACR-002 translated that philosophy into a more tangible system model:

- Mnemosyne as governed memory
- Metis as judgment
- Muses as durable domain lenses
- agents as operators
- projects as contexts and contributors
- governed assets, metadata, relationships, sessions, and experience as possible system primitives

A later Brainstorms session began with a narrower operational problem: development work, especially AI-assisted work, was moving faster than project documentation could be maintained.

The initial idea was to create an agent that observes development activity and updates relevant documentation. The discussion quickly expanded beyond documentation and surfaced a broader product thesis:

> Olympus may be useful not only as John's portfolio-wide knowledge ecosystem, but as a reusable operating model and intelligence layer that can be instantiated into individual projects.

This record preserves that conceptual evolution.

---

# Core Insight

The central insight is:

> **Documentation is not the product. Project understanding is the product.**

Documentation remains important, but it becomes one output of a broader system that understands:

- what changed
- why it changed
- what knowledge is affected
- what decisions govern the change
- which sources are authoritative
- what risks or conflicts are introduced
- what knowledge is stale
- what future work should know

In this framing, Olympus becomes an **intelligence layer above project tools**, not a replacement for them.

GitHub may know code.

Jira may know work items.

Obsidian, Confluence, or Notion may know documents.

Cursor and other coding agents may create implementation output.

Olympus would attempt to understand the **meaning, authority, relationships, history, and consequences across them**.

---

# Project Intelligence

For purposes of this concept record, **Project Intelligence** is a working term for:

```text
The governed ability to understand a project's evolving state, knowledge, decisions,
relationships, risks, and history across the tools in which the work occurs.
```

Project Intelligence is not equivalent to:

- project management
- engineering metrics
- document search
- RAG over project files
- code intelligence
- knowledge management alone
- an AI chatbot

It may draw from all of these, but its distinguishing concern is **coherent project understanding over time**.

A Project Intelligence system should eventually be able to answer questions such as:

```text
What changed?
Why did it change?
Which approved decisions apply?
Which knowledge assets are now stale?
What conflicts with this change?
What downstream projects or artifacts are affected?
What lessons from prior work should inform this?
What should be reviewed next?
How confident are we in this recommendation?
```

---

# Olympus as a Deployable Framework

The Brainstorms discussion introduced a potentially important extension to the Olympus model:

> The Olympus operating model may be reusable across projects rather than being handcrafted independently for each one.

Under this model, there would be a distinction between **Olympus Core** and a **Project Instance**.

## Olympus Core

Potentially reusable elements include:

- Knowledge Asset model
- status and authority model
- provenance rules
- decision records
- lesson capture
- promotion workflows
- agent operating boundaries
- Muse/domain lens model
- Metis judgment principles
- Mnemosyne memory principles
- relationship semantics
- session continuity patterns
- conflict handling
- AI consumption rules

## Project Instance

A participating project may supply:

- project-specific assets
- repositories
- product definitions
- architecture
- local terminology
- project decisions
- project-specific Muse emphasis
- tool integrations
- ownership
- implementation constraints
- local lessons and experience

Conceptually:

```text
                 Olympus Core
        governance + memory + judgment
                      │
       ┌──────────────┼──────────────┐
       ▼              ▼              ▼
   CraftHaus       TripNetX      Hobby Brain
    Instance        Instance       Instance
       │              │              │
 code / docs /     code / docs /   code / docs /
 decisions /       decisions /     decisions /
 history           history         history
```

This raises a new architectural question that ACR-001 and ACR-002 did not fully resolve:

> **What belongs to Olympus itself, and what is configuration or knowledge supplied by an individual project?**

That question should remain open until product and architecture work formally begins.

---

# Documentation Steward as a Product Wedge

The narrow problem that triggered this concept remains valuable.

A possible first Project Intelligence workflow is a **Documentation Steward** or, more broadly, **Knowledge Integrity Steward**.

Conceptual flow:

```text
Pull request / material change
            │
            ▼
Analyze the change
            │
            ▼
Identify affected Knowledge Assets
            │
            ▼
Check status, authority, ownership, and relationships
            │
            ▼
Propose updates, warnings, or review actions
            │
            ▼
Human reviews and approves consequential changes
            │
            ▼
Project knowledge returns to a known state of integrity
```

The key distinction is that the steward should not merely ask:

```text
Which Markdown files mention this code?
```

It should eventually ask:

```text
Which knowledge is affected by this change?
Which source is authoritative?
Is the affected guidance approved, exploratory, or superseded?
Does the change conflict with an existing decision?
Who should review the impact?
What should future agents now know?
```

This makes documentation maintenance a visible wedge into the larger Project Intelligence thesis rather than the final product definition.

---

# Continuous Knowledge Integrity

The Brainstorms discussion described a concept similar to "governance by construction."

This record uses the working term **Continuous Knowledge Integrity** instead.

Continuous Knowledge Integrity means:

```text
Project changes continuously trigger evaluation of whether governed knowledge,
decisions, relationships, and guidance remain accurate and internally consistent.
```

Traditional documentation workflows ask:

```text
Did someone remember to update the docs?
```

Continuous Knowledge Integrity asks:

```text
What knowledge did this change potentially invalidate?
```

Potential outcomes may include:

- no action required
- documentation update proposed
- decision conflict flagged
- stale Knowledge Asset identified
- lesson or experience candidate created
- owner review requested
- relationship updated
- project risk surfaced

This is conceptually aligned with OPM-002's knowledge capture and promotion model, but it extends the model by making **project change itself a trigger for knowledge review**.

---

# Relationship to Mnemosyne and Metis

The Project Intelligence thesis does not replace ACR-001 or ACR-002.

It gives their concepts a possible market-facing expression.

## Mnemosyne

Mnemosyne remains the governed memory layer.

Project Intelligence expands the likely sources of memory to include project activity across repositories, work systems, discussions, documentation, and governed assets.

## Metis

Metis remains the judgment layer.

Project Intelligence gives Metis concrete questions to answer:

- what changed?
- what matters?
- what conflicts?
- what is authoritative?
- what is stale?
- what needs review?
- what should be recommended?

## Muses

Muses remain durable domain lenses.

A project change may have different implications under Architecture, Product, Governance, Operations, Engineering, User Experience, or other lenses.

## Agents

Agents remain operators, not authority.

They may discover, analyze, recommend, draft, and route changes, but consequential promotion or approval remains governed by human authority.

---

# Product Positioning Hypothesis

A working product-positioning hypothesis is:

> **Olympus is a Project Intelligence layer above the tools where project work already happens.**

This positioning intentionally avoids framing Olympus as:

- another project management tool
- another documentation platform
- another engineering dashboard
- another coding agent
- another enterprise search product

The hypothesis is that Olympus should make existing project systems **coherent**, preserving project meaning and institutional memory while applying governed judgment across them.

This is an **unvalidated hypothesis**.

RNO-003 should be consulted for current competitive/category evidence before relying on this positioning.

---

# Potential Product Maturity Model

The Brainstorms discussion proposed an early maturity path. It is preserved here as exploration only.

## Olympus Foundation

Potential focus:

- knowledge asset model
- governance
- templates and standards
- project structure
- agent operating patterns
- lightweight stewardship

## Olympus Intelligence

Potential focus:

- project-tool connectors
- change-impact reasoning
- knowledge freshness
- decision traceability
- governed search and judgment
- continuous knowledge integrity
- project-level insights

## Olympus Enterprise / Portfolio Intelligence

Potential focus:

- cross-project dependencies
- portfolio risk
- shared knowledge
- cross-project decisions
- organizational lessons
- policy consistency
- institutional memory across projects

This maturity path should not be treated as a roadmap until customer and market evidence supports it.

---

# What This Concept Does Not Decide

ACR-003 does **not** decide:

- that Olympus will become a commercial product
- that "Project Intelligence" is a new category
- that Project Intelligence is the final category name
- that a knowledge graph is required
- that Obsidian is part of the product
- that Cursor Cloud Agents are the implementation mechanism
- that pull requests are the only or primary trigger
- that CraftHaus is the final MVP design partner
- that the product should be SaaS
- that the product should be venture funded
- that an MVP should be built in five to eight weeks
- pricing, packaging, buyer, or go-to-market strategy

Those remain hypotheses or future decisions.

---

# Strategic Risks

## Architecture mistaken for customer value

Olympus may have an elegant internal architecture that customers do not care about. Mnemosyne, Metis, Muses, and Knowledge Assets are implementation and operating concepts unless they translate into outcomes customers value.

## Documentation wedge becomes the ceiling

A documentation steward may be useful but could trap Olympus in the technical documentation market if the broader intelligence value is not demonstrated.

## Project Intelligence may already be occupied

Adjacent vendors already provide engineering knowledge graphs, cross-tool enterprise graphs, code-context systems, engineering intelligence, and continuous documentation. The market position must be tested rather than assumed.

## Overreach

Attempting to understand every artifact, tool, conversation, and project state could turn Olympus into an unbounded integration problem.

## Authority dilution

If automatically inferred relationships or generated summaries are treated with the same authority as governed decisions and Knowledge Assets, Olympus loses one of its strongest conceptual advantages.

## Automation without trust

Automatically updating knowledge without clear provenance, ownership, review, and approval could create confident institutional misinformation rather than institutional memory.

---

# Design Principles Emerging from This Concept

1. **Project understanding over document maintenance.**
2. **Governed knowledge over unqualified retrieval.**
3. **Human authority over inferred approval.**
4. **Existing tools remain systems of work; Olympus becomes a system of meaning.**
5. **Change should trigger knowledge-integrity evaluation.**
6. **Agents propose and route; governed authority decides.**
7. **Project instances should share a reusable Olympus core where evidence supports reuse.**
8. **Market-facing value must be validated independently from architectural elegance.**
9. **The documentation steward is a wedge, not automatically the destination.**
10. **Do not claim category creation before customers and competitive evidence support it.**

---

# Candidate Validation Sequence

Before formal product or architecture decisions, Olympus should test the thesis in this order:

```text
1. Competitive/category research
2. Define the expensive customer problem
3. Identify target buyer/user
4. Define a narrow testable wedge
5. Validate the workflow in a real project
6. Validate with at least one external project/team
7. Decide whether the evidence supports commercialization
8. Only then formalize product scope and MVP architecture
```

RNO-003 begins Step 1.

---

# Open Questions

- Is **Project Intelligence** the right market-facing term?
- Is Olympus primarily a knowledge system, a project-intelligence platform, or an operating framework?
- What belongs in **Olympus Core** versus a project instance?
- Which project events should trigger Continuous Knowledge Integrity evaluation?
- What is the minimum governed metadata needed to make automated change-impact analysis trustworthy?
- Is the strongest wedge documentation stewardship, decision traceability, agent context, or something else?
- Which user experiences the pain most acutely: engineer, product leader, architect, CTO, PMO, compliance leader, or founder?
- Which buyer controls budget?
- How should Olympus differentiate from engineering knowledge platforms, enterprise graphs, engineering intelligence, and continuous-documentation products?
- Does portfolio-level intelligence create enough incremental value to justify a separate product tier?
- What evidence would justify promoting this concept into a Product Decision Record?

---

# Related Research

See **RNO-003 — Project Intelligence Product Hypotheses and Competitive Landscape** for market evidence and current adjacent products.

---

# Change History

| Version | Date | Change |
|---|---|---|
| 0.1.0 | 2026-08-15 | Initial exploratory concept record created from the Brainstorms session and comparison against ACR-001, ACR-002, and current Olympus governance/operating assets. |
