# Architectural Concept Record (ACR-002)

# From Myth to Plumbing

## A Tangible Backend Model for the Olympus Knowledge Ecosystem

| Metadata | Value |
|---|---|
| **Knowledge Asset ID** | ACR-002 |
| **Title** | From Myth to Plumbing |
| **Classification** | Architectural Concept Record |
| **Category** | Knowledge Management / Conceptual Architecture |
| **Status** | Exploratory |
| **Authority Level** | Informational |
| **Canonical Source** | No |
| **Version** | 0.1.0 |
| **Owner** | John S. Villasenor |
| **Primary AI Owner** | Hermes |
| **Created On** | 2026-07-05 |
| **Last Updated** | 2026-07-05 |
| **Review Cadence** | As Needed |
| **Next Review Due** | TBD |
| **Date Retired** |  |
| **Retirement Reason** |  |
| **AI Consumption** | Recommended |
| **Change Impact** | High |
| **Related Assets** | ACR-001; MT_OLYMPUS_FOUNDATION_BRIEF; KNOWLEDGE_ASSET_MODEL; OLYMPUS_GOVERNANCE_STARTER; MUSE_CATALOG_STARTER; MT_OLYMPUS_DECISION_BACKLOG |
| **Tags** | olympus, mnemosyne, metis, muses, backend, knowledge-assets, memory, judgment, architecture, rag, graph, governance |

---

# Status

This document captures an emerging conceptual architecture.

It is **not** a final design specification, database schema, implementation plan, or architectural decision.

Its purpose is to make the Olympus concept tangible enough to support product and architecture design work.

Nothing in this document should be treated as implementation authority until promoted through the appropriate governance process.

---

# Purpose

ACR-001 established the conceptual relationship between Mnemosyne, Metis, the Muses, AI agents, and projects.

This record translates that concept into something more concrete:

- what gets stored
- where knowledge might live
- how experience might be captured
- how judgment might be produced
- how the system might avoid becoming just another document repository or RAG chatbot

This document exists to support the "landing approach" from 10,000-foot concept toward buildable product architecture.

---

# Core Concern

The central question raised during discussion was:

> How in the hell do we build this?

The concern is valid.

At a high level, Olympus sounds elegant:

- Mnemosyne gives us memory.
- Metis gives us judgment.
- The Muses provide specialized expertise.
- AI agents serve the Muses.
- Projects consume and contribute knowledge.

But elegance is not enough.

Unless Olympus can explain what gets stored, how it is governed, how it is retrieved, how experience is captured, and how recommendations are produced, it risks becoming a mythology-themed document library.

The system must become understandable as plumbing, not only as philosophy.

---

# Critical Clarification

Olympus should not begin as a generic "chat with documents" or RAG application.

A basic RAG system usually follows this pattern:

```text
Upload documents
        │
        ▼
Create embeddings
        │
        ▼
Ask questions
        │
        ▼
Generate answers from retrieved chunks
```

That is useful, but it is not enough.

Olympus must preserve not only content, but also:

- authority
- provenance
- ownership
- status
- decisions
- rationale
- lessons learned
- institutional memory
- experience
- domain context
- change history
- AI usage guidance

A vector database may be part of Olympus.

A vector database is not Olympus.

---

# Refined Conceptual Model

## Mnemosyne

Mnemosyne should be understood as the **governed memory layer**.

She is not merely a repository of files and not merely a RAG vector database.

Mnemosyne stores and organizes:

- artifacts
- knowledge assets
- metadata
- relationships
- provenance
- versions
- decision history
- authority status
- embeddings
- historical context
- captured experience

Mnemosyne answers:

```text
What do we have?
Where did it come from?
Who owns it?
Is it current?
Is it authoritative?
What does it relate to?
How should an AI use it?
```

## Metis

Metis should be understood as the **judgment layer**.

Metis is not passive storage.

Metis reasons over Mnemosyne.

Metis interprets memory, applies authority rules, weighs tradeoffs, detects conflicts, identifies patterns, and synthesizes recommendations.

Metis answers:

```text
What does this mean?
What matters?
What conflicts?
What should we recommend?
What tradeoffs exist?
What prior lessons apply?
How confident should we be?
```

## The Muses

The Muses should be understood as **domain lenses**.

They are not AI agents.

They are not chatbots.

They are durable disciplines that shape how knowledge should be interpreted.

The Muses answer:

```text
Which discipline governs this question?
What kind of expertise should be applied?
What criteria should judgment use?
What risks should be considered?
What would good look like in this domain?
```

## AI Agents

AI agents are **operators and interfaces**.

Agents interact with users, invoke Muse lenses, use Metis reasoning, retrieve from Mnemosyne, and produce work.

Agents answer:

```text
How do I help the user right now?
Which Muse lens applies?
What sources must I respect?
What should I produce?
What should I not assume?
```

## Projects

Projects are **contexts and contributors**.

Projects use Olympus and also generate knowledge for Olympus.

Projects answer:

```text
Where did this knowledge come from?
Which product or initiative does it affect?
Which local constraints apply?
What future work should this inform?
```

---

# Conceptual Relationship

```text
                 John / Founder
            vision, authority, approval
                         │
                         ▼
                   Olympus
        governed knowledge continuity system
                         │
        ┌────────────────┼────────────────┐
        ▼                ▼                ▼
   Mnemosyne           Metis          The Muses
 governed memory      judgment       domain lenses
        │                │                │
        └───────┬────────┴────────┬───────┘
                ▼                 ▼
           AI Agents           Projects
       Hermes, Atlas, etc.    TripNetX, CraftHaus,
                              Hobby Brain, Bank of Villasenor
```

Operationally:

```text
User asks a question
        │
        ▼
Agent identifies relevant Muse domain
        │
        ▼
Muse determines the disciplinary lens
        │
        ▼
Metis queries Mnemosyne for governed memory
        │
        ▼
Mnemosyne returns assets, metadata, authority, and relationships
        │
        ▼
Metis synthesizes judgment
        │
        ▼
Agent presents recommendation to human
```

---

# Proposed Backend Layers

Olympus likely requires five conceptual backend layers.

```text
┌────────────────────────────────────────────┐
│                 User / Agent               │
└────────────────────┬───────────────────────┘
                     │ asks, records, reviews
                     ▼
┌────────────────────────────────────────────┐
│              Application Layer             │
│  capture, search, review, promote, decide  │
└────────────────────┬───────────────────────┘
                     ▼
┌────────────────────────────────────────────┐
│                  Metis                     │
│ judgment, synthesis, conflict detection    │
└────────────────────┬───────────────────────┘
                     ▼
┌────────────────────────────────────────────┐
│                Muse Layer                  │
│ architecture, product, governance, etc.    │
└────────────────────┬───────────────────────┘
                     ▼
┌────────────────────────────────────────────┐
│                Mnemosyne                   │
│ governed memory: assets, events, links     │
└────────────────────┬───────────────────────┘
                     ▼
┌────────────────────────────────────────────┐
│        Storage / Index / Graph Layer       │
│ relational db + object store + vector index│
└────────────────────────────────────────────┘
```

---

# Mnemosyne as a Memory Subsystem

Mnemosyne should not be implemented as one simple store.

A practical implementation may require several storage patterns.

| Store | Purpose | Example Technology |
|---|---|---|
| Relational database | Canonical metadata, authority, ownership, status, and relationships | Postgres / Supabase |
| Object or document storage | Raw files, Markdown, PDFs, transcripts, screenshots, exports | GitHub, Supabase Storage, S3 |
| Vector index | Semantic retrieval over asset content and chunks | pgvector, Pinecone, Weaviate |
| Relationship layer | Asset relationships, decisions, dependencies, contradictions | Postgres tables first; graph database later if justified |

Recommended early posture:

> Start with Postgres, GitHub, and pgvector before considering a dedicated graph database.

A graph database may eventually be useful, but starting there would likely overcomplicate the foundation before the asset model is mature.

---

# Proposed Core Data Structures

This section is exploratory and intended to make the concept concrete.

The table names and fields below are not final.

## `knowledge_assets`

The central record for governed knowledge.

```text
knowledge_assets
- id
- asset_id
- title
- classification
- category
- status
- authority_level
- canonical_source
- owner
- primary_ai_owner
- created_on
- last_updated
- review_cadence
- ai_consumption
- change_impact
- source_uri
- summary
- current_version_id
```

Purpose:

```text
What is this thing?
Who owns it?
Can it be trusted?
Is it current?
Should AI agents use it?
```

## `asset_versions`

Tracks how knowledge changes over time.

```text
asset_versions
- id
- asset_id
- version
- content_hash
- source_uri
- created_at
- created_by
- change_summary
- supersedes_version_id
```

Purpose:

```text
What changed?
When did it change?
Who changed it?
Which version is current?
```

## `asset_chunks`

The RAG retrieval layer, always tied back to governed assets.

```text
asset_chunks
- id
- asset_id
- version_id
- chunk_index
- chunk_text
- section_heading
- token_count
- embedding
- source_start_line
- source_end_line
```

Important rule:

> A retrieved chunk should never be used without also retrieving its parent asset metadata, status, authority level, and source.

Otherwise an exploratory idea and a governing standard can appear equally trustworthy to an AI model.

## `relationships`

The first version of the knowledge graph.

```text
relationships
- id
- source_asset_id
- target_asset_id
- relationship_type
- description
- created_at
- created_by
```

Possible relationship types:

```text
informs
supersedes
contradicts
depends_on
implements
derives_from
references
blocks
replaces
related_to
```

Purpose:

```text
What is connected?
What depends on what?
What replaced what?
What conflicts?
What decision does this inform?
```

## `decisions`

Decision records may deserve first-class treatment.

```text
decisions
- id
- decision_id
- title
- status
- authority_level
- owner
- decided_on
- decision_text
- rationale
- consequences
- source_asset_id
```

Reason:

> Decisions are where future AI agents can do the most damage if they confuse a passing mention with an approved position.

## `experience_events`

A capture structure for lessons, surprises, hard-won judgment, and institutional memory before they become polished assets.

```text
experience_events
- id
- title
- event_type
- project
- domain
- occurred_on
- captured_on
- captured_by
- raw_context
- what_happened
- why_it_mattered
- lesson_learned
- recommended_future_use
- confidence_level
- related_asset_ids
- promotion_status
```

Possible event types:

```text
lesson
observation
failure
surprise
intuition
tradeoff
pattern
risk
postmortem
```

Purpose:

```text
What did we learn?
Why did it matter?
How should future agents use this?
Should this become a formal asset?
```

This is the key structure for capturing experience.

Experience is rarely born as a polished document.

It usually starts as an observation, surprise, failure, scar, or founder intuition.

Olympus needs a way to capture that while it is still fresh.

## `muses`

The Muses as durable domain records.

```text
muses
- id
- classical_name
- discipline
- domain
- responsibility
- active
```

Purpose:

```text
Which domain lens applies?
What kind of expertise governs this question?
```

## `muse_profiles`

Optional configuration for domain-specific reasoning.

```text
muse_profiles
- muse_id
- question_patterns
- retrieval_filters
- required_asset_types
- evaluation_criteria
- prompt_instructions
- output_templates
```

Purpose:

```text
How should this Muse shape retrieval, evaluation, and response?
```

## `agent_sessions`

Tracks AI-assisted sessions and continuity.

```text
agent_sessions
- id
- session_date
- agent_name
- agent_role
- project
- active_muses
- summary
- handoff_asset_id
- created_assets
- decisions_touched
- unresolved_questions
```

Purpose:

```text
What happened in the session?
What did the agent touch?
What should the next session know?
```

---

# Metis as a Judgment Pipeline

Metis should be understood as a reasoning pipeline rather than a database table or passive agent.

When a user asks a question, Metis may eventually perform the following steps:

```text
1. Classify the question.
2. Identify relevant Muse domains.
3. Query Mnemosyne for governed memory.
4. Retrieve assets, chunks, metadata, and relationships.
5. Rank sources by authority, relevance, freshness, and domain fit.
6. Detect conflicts.
7. Separate approved decisions from exploratory ideas.
8. Generate judgment.
9. Return cited recommendations with confidence and authority notes.
```

Metis should never answer from embeddings alone.

Metis should answer from:

```text
retrieved knowledge
+ authority rules
+ domain lens
+ relationship context
+ reasoning
```

Potential Metis components:

```text
retrieval policy
ranking logic
authority resolver
conflict detector
source summarizer
decision extractor
synthesis prompt
recommendation engine
confidence estimator
```

---

# Muse Layer as Domain Lenses

The Muses should not become a collection of chatbots.

A Muse should define:

```text
- what questions belong to this domain
- which assets are relevant
- which standards apply
- what good judgment looks like
- what risks should be considered
- what output format is useful
```

Examples:

## Urania / Architecture

Questions Urania asks:

```text
What systems are affected?
What constraints exist?
What decisions already govern this?
What tradeoffs are structural?
What breaks if we choose wrong?
```

## Clio / Knowledge Stewardship

Questions Clio asks:

```text
Is this knowledge preserved correctly?
Is the source authoritative?
Does the asset have metadata?
Is this duplicated elsewhere?
Should this be promoted, linked, or retired?
```

## Polyhymnia / Governance

Questions Polyhymnia asks:

```text
Who has authority?
What is the status?
Is this decision approved or merely proposed?
What standard applies?
Is this process compliant?
```

---

# Capturing Experience

The central product challenge is not document storage.

The central product challenge is capturing experience.

Olympus should not ask users to fill out heavy forms every time something is learned.

Instead, it should support small capture moments.

## Capture Path 1: Session Handoff

At the end of an AI-assisted work session, Olympus should capture:

```text
What changed?
What did we learn?
What surprised us?
What should future agents know?
What mistakes should not be repeated?
```

Output may become:

```text
Handoff artifact
Experience event
Lesson learned candidate
Decision candidate
```

## Capture Path 2: Decision Creation

When a decision is made, Olympus should capture:

```text
What did we decide?
Why?
What alternatives were rejected?
What risks remain?
What future work does this affect?
```

Output may become:

```text
Decision record
Related asset links
Authority update
```

## Capture Path 3: Lesson Learned

When something fails or surprises the team, Olympus should capture:

```text
What happened?
Why did it matter?
What assumption was wrong?
What should we do differently?
Where should this warning appear in the future?
```

Output may become:

```text
Lesson Learned asset
Experience event
Risk note
Governance candidate
```

## Capture Path 4: Inline Capture Command

A user should be able to say:

```text
Capture this as a lesson learned.
```

Olympus should ask only the minimum needed:

```text
Which project?
Which Muse/domain?
Is this informational, advisory, or a proposed standard?
```

Output may become:

```text
Captured experience event
Draft knowledge asset
Review queue item
```

## Capture Path 5: Agent-Generated Candidate Knowledge

After a long session, an agent may propose candidate assets:

```text
I found 3 candidate knowledge assets:
1. A new reporting UI pattern
2. A limitation in agent QA capabilities
3. A recurring handoff requirement
```

The human can approve, edit, defer, or reject each candidate.

Output may become:

```text
Promoted asset
Dismissed capture
Deferred review item
```

---

# MVP Loop

The first product version should prove one loop:

```text
Capture knowledge
        │
        ▼
Classify it
        │
        ▼
Retrieve it later
        │
        ▼
Apply judgment better than generic AI
```

That is the core Olympus value proposition.

## MVP Backend

```text
Postgres / Supabase
- knowledge_assets
- asset_versions
- asset_chunks with pgvector
- relationships
- experience_events
- muses
- agent_sessions
```

## MVP Workflows

```text
1. Add Knowledge Asset
2. Add Experience Event
3. Search / Ask Olympus
4. Promote captured experience into formal asset
5. Generate session handoff
```

## MVP Interface Areas

```text
Dashboard
- recent assets
- open decisions
- captured experience needing review
- active projects

Asset View
- metadata
- content
- relationships
- authority/status
- related experience

Ask Olympus
- question box
- selected Muse lens
- answer with citations
- authority notes
- conflicts found

Capture Experience
- quick form
- project
- domain/Muse
- what happened
- why it mattered
- future guidance

Review Queue
- candidate assets
- captured lessons
- proposed decisions
- stale or conflicting knowledge
```

---

# Practical Early Architecture

A practical early architecture could look like:

```text
Frontend
- Next.js application
- Asset browser
- Ask Olympus
- Capture Experience
- Review Queue

Backend
- Supabase Postgres
- Supabase Auth
- Supabase Storage or GitHub-backed documents
- pgvector for embeddings

AI Layer
- ingestion worker
- embedding generator
- retrieval service
- Metis synthesis service
- Muse prompt/profile layer

Source Control
- GitHub remains canonical for Markdown assets at first
- Database stores metadata, chunks, embeddings, relationships, and review state
```

Recommended posture:

> Begin GitHub-first for formal Markdown assets, because the project already uses repositories, commits, handoffs, and evidence packets.

The database can index, govern, and relate those assets.

Later, the application may create or edit assets directly and open pull requests to GitHub.

---

# Important Product Warning

Do not try to capture "all knowledge."

That phrase is a trap.

Olympus should capture knowledge with future decision value.

Suggested capture rule:

> Olympus does not preserve everything.  
> Olympus preserves what future judgment needs.

This protects the system from becoming an expensive junk drawer.

---

# Proposed First Product Primitives

For design work, Olympus can be framed around four user-facing primitives:

## 1. Assets

Durable knowledge objects.

Examples:

```text
Concept Record
Decision Record
Governance Standard
Product Definition
Architecture Definition
Lesson Learned
Research Note
Operating Model
Session Handoff
```

## 2. Questions

What a user or agent is trying to answer.

Examples:

```text
What did we decide about CraftHaus reporting filters?
Which governance standard applies to agent handoffs?
What lessons have we learned about AI-assisted QA?
```

## 3. Lenses

The Muse/domain perspective applied to the question.

Examples:

```text
Architecture
Product
Governance
Knowledge Stewardship
User Experience
Operations
```

## 4. Judgments

Metis-generated synthesis grounded in Mnemosyne.

Examples:

```text
Recommendation
Tradeoff analysis
Conflict warning
Authority note
Confidence statement
Suggested next action
```

---

# Example Future Flow

Question:

```text
What did we decide about CraftHaus reporting filters?
```

Olympus should be able to respond with something like:

```text
Relevant Muses:
- User Experience
- Governance
- Product

Memory:
- source docs
- decision records
- handoffs
- evidence packets

Authority:
- approved guidance outranks exploratory discussion
- founder direction outranks assistant inference

Judgment:
- apply the Owner Sales Breakdown pattern incrementally
- do not refactor all reports at once
- preserve report-local period controls
- distinguish approved standards from inferred patterns

Risks:
- accidental global refactor
- inconsistent period semantics
- UI drift between reports

Sources:
- linked Knowledge Assets
- handoff records
- decision records
```

This illustrates the difference between Olympus and generic document chat.

Olympus does not merely retrieve text.

Olympus produces governed, domain-aware judgment.

---

# Candidate Data Model Summary

```text
Project
  has many Knowledge Assets
  has many Sessions
  has many Experience Events

Knowledge Asset
  has Metadata
  has Versions
  has Chunks
  has Relationships
  may be linked to Decisions
  may be linked to Experience Events

Muse
  classifies Assets
  filters Retrieval
  shapes Judgment

Metis
  retrieves from Mnemosyne
  applies Authority Hierarchy
  detects Conflicts
  produces Recommendations

Agent Session
  creates Handoffs
  captures Experience
  proposes Assets
```

---

# Landing Strip Summary

```text
Mnemosyne is the governed memory database.
It stores assets, metadata, relationships, chunks, versions, and experience events.

Metis is the judgment pipeline.
It retrieves from Mnemosyne, applies authority rules, detects conflicts, and synthesizes recommendations.

The Muses are domain lenses.
They determine which expertise framework applies to a question.

Agents are operators.
They interact with users, invoke Muse lenses, use Metis reasoning, and produce work.

Projects are contexts.
They contribute knowledge and consume knowledge.
```

The first real Olympus product is not:

```text
chat with documents
```

The first real Olympus product is:

```text
a governed knowledge capture and judgment system
```

---

# Open Questions

- Should formal Knowledge Assets remain GitHub-first indefinitely, or should the application eventually become the primary editor?
- Should `decisions` be a separate table or a specialized `knowledge_assets` type?
- How much of Metis should be deterministic policy logic versus LLM reasoning?
- Should Research remain a cross-cutting activity or become a formal Muse discipline?
- What is the minimum viable `experience_event` capture form?
- How should captured experience be reviewed, promoted, dismissed, or linked?
- What must be cited in every Metis-generated judgment?
- How should Olympus handle conflicts between canonical assets?
- How should project-specific knowledge be separated from portfolio-wide knowledge?
- When, if ever, does the relationship layer require a true graph database?

---

# Design Guidance

For the next phase of product design, do not start with the chat screen.

Start with the following flows:

1. Knowledge Asset creation and browsing
2. Experience capture
3. Review and promotion
4. Ask Olympus / Metis judgment
5. Session handoff generation

These flows are where the product proves whether the plumbing works.

If Olympus cannot capture knowledge, classify it, retrieve it, and apply authority-aware judgment, the chat interface will only decorate a weak foundation.

---

# Change History

| Version | Date | Change |
|---|---|---|
| 0.1.0 | 2026-07-05 | Initial exploratory record created from discussion on translating Olympus from conceptual model into tangible backend and product architecture. |
