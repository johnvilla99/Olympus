# Agent Knowledge Discovery Standard

> **Status:** Approved / Advisory. Accepted for current Olympus use; not Canonical or Governing.

## Metadata

| Field | Value |
|---|---|
| Standard ID | OLY-GOV-005 |
| Title | Agent Knowledge Discovery Standard |
| Classification | Governance Standard |
| Category | Governance / Knowledge Stewardship |
| Status | Approved |
| Authority Level | Advisory |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Primary AI Owner | Hermes |
| Created On | 2026-07-22 |
| Last Updated | 2026-07-25 |
| Review Cadence | As Needed |
| Related Assets | OLY-GOV-001; OLY-GOV-002; OLY-GOV-003; OLY-GOV-004; OPM-001; OPM-002; OPM-003; GDR-001; ACR-001; ACR-002; Decision Backlog (OLY-DB-009); RNO-001 |
| AI Consumption | Required |
| Change Impact | High |

---

## Purpose

OLY-GOV-005 defines the minimum rules an AI agent must follow when relying on Olympus-governed knowledge to answer questions, make recommendations, or produce work.

Its purpose is to ensure that **relevant** knowledge is not mistaken for **authoritative** knowledge, and that agents preserve Status, Authority Level, provenance, scope, relationships, conflicts, assumptions, and approval boundaries when using Olympus sources.

This standard governs the **safe consumption** of Olympus-governed knowledge. It does not define agent roles, repository maintenance, project participation, runtime architecture, or knowledge-system implementation.

Discovery is not retrieval alone. Discovery is authority-aware selection and use of knowledge.

## Scope

### In scope

- Discovery intent
- Source discovery order
- Status and Authority Level evaluation
- Metadata interpretation
- Project and portfolio boundaries
- Relationship navigation
- Conflict handling
- Citation and evidence expectations
- Synthesis and inference boundaries
- Proportionality
- Stop and escalation conditions
- Integrity of knowledge use within answers and work products

### Out of scope

- Agent role definitions
- Project participation or adoption rules
- Runtime or product agents
- Metis implementation
- Muse invocation mechanics
- Asset creation, placement, promotion, or approval
- Repository editing and continuity procedures
- Application code, schemas, APIs, UI, vector search, vendors, or technical architecture
- Closure of OLY-DB-009, which remains open for practical validation

## Applicability

This standard applies whenever an AI agent is authorized to consume Olympus-governed knowledge.

Authorization determines whether an agent may access and use knowledge. It does not determine the authority of that knowledge.

An agent’s role, project, organization, or operating environment may vary. Authorization to access Olympus knowledge does not confer authority to approve, modify, promote, generalize, or redistribute it.

Agent roles and stewardship responsibilities are defined by OPM-001 and related operating models. Project participation and adoption rules require separate governance. Future runtime behavior remains a product and architecture concern.

Mnemosyne, Metis, and the Muses remain conceptual context in ACR-001 and ACR-002 unless later promoted. Research is a cross-cutting activity, not a tenth Muse.

## Governing References

OLY-GOV-005 does not define its own authority hierarchy.

- **OLY-GOV-003** is the authoritative source for decision authority, status, approval, hierarchy, and conflict treatment.
- **OLY-GOV-002** defines Knowledge Asset metadata, Status, Authority Level, Canonical Source, AI Consumption, and lifecycle rules.
- **OLY-GOV-004** defines continuity-source and session-resume behavior.
- **OPM-001** defines agent roles and operating boundaries.
- **GDR-001** defines the Canonical Olympus identifier convention.

This standard applies those rules to discovery and consumption.

## Core Consumption Rules

| Rule | Meaning |
|---|---|
| Relevant does not mean authoritative | A matching passage is not binding without Status and Authority Level evaluation |
| Status and Authority Level work together | Neither field alone is sufficient |
| John is final Olympus authority | Explicit Founder direction has highest authority within the Founder’s authority; project or client authority remains local |
| Agents do not approve | Agents discover, interpret, recommend, and escalate; they do not promote assets or close decisions |
| Proposed is not Approved | Proposed sources guide review, not current authority |
| Draft is not current guidance | Draft sources may provide context but remain unfinished |
| ACRs are exploratory | Concept records inform reasoning but are not implementation authority |
| Handoffs and logs are continuity aids | They explain recent work but do not override formal assets |
| Research is evidence | Research notes and lessons inform decisions but are not decisions themselves |
| Commit or push is not approval | Persistence does not change Status or Authority Level |
| Do not invent closure | Material gaps and conflicts must be surfaced |

## 1. Discovery Intent

Before deep retrieval, identify:

1. The user’s actual question or requested work.
2. The affected project, portfolio, client, or business context.
3. The relevant domain lenses.
4. The task type: fact, decision application, recommendation, synthesis, implementation guidance, continuity, conflict investigation, or work-product creation.
5. The consequence of being wrong.

If intent is unclear and the consequence is material, ask a proportional clarifying question. Low-impact ambiguity should not become procedural theater.

## 2. Source Discovery Order

Use this practical search order to locate candidate sources. It is a discovery path, not an independent hierarchy of truth.

| Order | Source Class | Examples |
|---|---|---|
| 1 | Explicit current Founder direction | Current John direction for Olympus governance or Olympus-owned knowledge |
| 2 | Governing and Canonical assets | Assets whose Status and Authority Level permit reliance |
| 3 | Approved decisions and Approved guidance | ADR, PDR, GDR, ODR, OLY-GOV, OPM, and other accepted assets |
| 4 | Relevant project-local authoritative assets | Approved project decisions, local governance, designated client or business sources |
| 5 | Proposed and Draft assets | Review candidates and unfinished guidance |
| 6 | Operational continuity and observable current state | Handoffs, logs, git state, evidence packets, current repository facts |
| 7 | Exploratory concept records | ACRs and other Exploratory / Informational assets |
| 8 | Research notes and lessons learned | Research evidence and preserved experience |
| 9 | Conversation context | Current and prior chat turns |
| 10 | Assistant inference or general knowledge | Model priors not grounded in Olympus sources |

### Discovery order versus authority

Discovery order helps locate candidate material. Authority is resolved under OLY-GOV-003 and OLY-GOV-002.

- A lower-authority source may be highly relevant.
- Relevance never authorizes silent override.
- Continuity artifacts explain recent work.
- Observable evidence verifies current state.
- Formal assets establish authority.
- None should be silently substituted for another.

## 3. Authority Resolution

For every material source, evaluate both:

- **Status**, which describes maturity or lifecycle
- **Authority Level**, which describes binding weight

Apply the hierarchy and conflict rules defined by OLY-GOV-003. Do not reproduce or reinterpret the hierarchy inside this standard.

Observable current-state evidence is not an Authority Level. It may confirm or contradict operational claims but does not override valid Governing, Canonical, or Approved direction.

When authority remains unclear:

1. Identify the competing sources.
2. State their Status, Authority Level, and Canonical Source value where relevant.
3. Check supersession, specificity, and local-versus-portfolio scope.
4. Surface the conflict.
5. Escalate when a human authority decision is required.

## 4. Metadata Interpretation

Read available metadata before relying on an asset.

| Field | Discovery Use |
|---|---|
| Knowledge Asset ID | Stable citation and asset-class signal |
| Classification | Standard, decision, concept, research, continuity, etc. |
| Category | Domain placement and lens selection |
| Status | Maturity and whether content is safe as current guidance |
| Authority Level | Binding weight |
| Canonical Source | Whether the asset is the source of truth for its subject |
| Owner | Accountable human owner |
| Primary AI Owner | Stewardship role only; does not confer approval power |
| Last Updated | Staleness signal |
| Review Cadence | Whether review may be overdue |
| Related Assets | Dependencies, lineage, supersession, and context |
| AI Consumption | Required, Recommended, Optional, or Restricted |
| Change Impact | Required depth and scrutiny |

### Metadata conditions

| Condition | Required Behavior |
|---|---|
| Missing Status or Authority Level | Do not assume Approved or Canonical; flag the gap |
| Incomplete ID, owner, or relationships | Cite what exists and note uncertainty |
| Stale high-impact asset | Seek fresher related sources and flag risk |
| Contradictory metadata | Flag; do not silently repair during consumption |
| AI Consumption = Restricted | Do not rely on or surface without permission |
| Partial seed metadata | Use cautiously for context; do not over-claim authority |

## 5. Project and Portfolio Context

| Context | Treatment |
|---|---|
| Olympus-wide knowledge | Portfolio foundation guidance |
| Project-specific knowledge | Bound to that project, engagement, or business context unless explicitly promoted |
| Local authoritative sources | Apply locally; do not auto-promote to portfolio guidance |
| Project continuity artifacts | Useful for recent context; not authoritative merely because they are local |
| Cross-project lessons | May inform other work when provenance and limits are preserved |
| Non-generalizable context | Client, personnel, pricing, legal, or temporary constraints that must remain local |

Knowledge created within a project or client context remains local unless explicitly reviewed and promoted. A project-local decision must not automatically become Olympus-wide guidance.

Broader participation and portfolio-scope rules remain open under existing backlog items. Do not invent a closed participation model here.

## 6. Relationship Navigation

Inspect related assets when relationships are material.

| Relationship | Discovery Implication |
|---|---|
| `informs` | Upstream context; cite when it shapes the conclusion |
| `references` | Supporting source; verify that it remains current |
| `depends_on` | Review the dependency before applying the dependent asset |
| `supersedes` / `replaces` | Prefer the successor when the relationship is explicit |
| `contradicts` | Mandatory conflict handling |
| `implements` | Realizes a decision or standard but does not gain higher authority by itself |
| `related_to` | Adjacent context; use proportionally |

A retrieved document must not be treated as isolated when its metadata identifies dependencies, replacements, or contradictions.

## 7. Conflict Handling

Common conflicts include:

| Category | Example |
|---|---|
| Direct contradiction | Incompatible rules on the same subject |
| Status conflict | Exploratory content treated as decisive against Approved guidance |
| Authority conflict | Lower-authority guidance conflicts with Canonical or Governing direction |
| Outdated source | Older asset retained without supersession after newer guidance |
| Duplicate source-of-truth claim | Multiple Canonical Source = Yes claims for one subject |
| Project-local versus portfolio-wide | Local decision treated as ecosystem rule or vice versa |
| Founder direction versus repository asset | Current direction conflicts with recorded guidance |
| Continuity versus observable state | Handoff claim conflicts with git state or current evidence |

Required behavior:

1. Surface the conflict.
2. Identify competing sources by ID or path.
3. State Status and Authority Level.
4. Check local scope, specificity, freshness, and supersession.
5. Do not silently choose when authority remains unclear.
6. Escalate to John for Olympus authority decisions.

If explicit Founder direction conflicts with repository assets, follow the current direction for the immediate Olympus task and route the durable conflict through OPM-002 and OPM-003. Do not pretend the repository already says what the conversation says.

## 8. Citation and Evidence Expectations

Cite or reference sources when:

- Applying an approved decision
- Claiming a governance rule
- Generating implementation guidance
- Reporting or resolving a conflict
- Producing a recommendation materially grounded in Olympus knowledge
- Creating a durable work product
- Explaining prior rationale

Prefer Knowledge Asset ID, path when useful, and section location when practical.

Citation should be proportional. Ordinary orientation does not require citation confetti; high-impact claims require clear lineage.

## 9. Synthesis and Inference Boundaries

Distinguish among:

| Mode | Meaning |
|---|---|
| Directly grounded fact | Stated in a source with adequate Status and Authority for the claim |
| Approved direction | Approved decisions, approved guidance, or explicit Founder direction |
| Advisory guidance | Approved / Advisory standards or operating models |
| Proposed direction | Ready for review but not current guidance |
| Draft content | Unfinished material; context only |
| Exploratory concept | ACR or other Exploratory content; context only |
| Evidence-supported inference | Reasonable conclusion from cited evidence, labeled as inference |
| Assistant recommendation | Agent proposal not yet Founder-approved |
| Unresolved gap | Missing or conflicted knowledge that must be surfaced |
| Unsupported invention | Fluent fill-in without grounding; avoid |

Do not paper over material gaps because an output template expects completeness.

## 10. Use in Work Products

When a recommendation, plan, proposal, assessment, handoff, SOW, or other work product materially relies on Olympus-governed knowledge, preserve:

- Applicable project or business context
- Status and Authority Level of material sources
- Source lineage
- Material assumptions
- Unresolved conflicts
- Known gaps
- Required human approval points

These may be explicit or incorporated in a form appropriate to the audience and impact.

This standard governs the integrity of knowledge use. It does not define the product, service, template, or runtime mechanism used to create the work product.

## 11. Proportionality

Discovery must not become a bureaucratic scavenger hunt.

| Impact Class | Discovery Depth |
|---|---|
| Low-impact factual request | Check obvious authoritative sources; light citation |
| Moderate-impact recommendation | Check Status and Authority on primary sources; cite the basis |
| High-impact decision or implementation guidance | Fuller discovery, relationship navigation, conflict scan, and escalation points |
| Durable work product | Preserve authority, lineage, assumptions, conflicts, and gaps |
| Governance or authority-changing request | Stop for Founder approval |

Depth scales with the consequence of being wrong.

## 12. Stop and Escalation Conditions

**Stop** when proceeding would create false authority or unsupported certainty.

**Continue with labeled limitations** when useful work remains possible despite gaps.

**Escalate** when a human authority decision is required.

Typical conditions:

- Required sources are unavailable or unreadable
- Restricted assets appear necessary
- Authority cannot be determined for a material claim
- Competing Canonical or Governing sources exist without a clear supersession path
- Founder approval is required
- The request would resolve an open backlog item without authorization
- The task crosses into unapproved product or architecture scope
- Evidence is too weak for the requested certainty
- Continuity claims conflict with observable state

Escalate Olympus authority decisions to John. Coordination roles may recommend but do not approve.

## 13. Output Expectations

When appropriate and proportional, a response may include:

```text
Conclusion or Work Product
Authority Basis
Sources Used
Conflicts or Gaps
Assumptions or Inference
Recommended Human Decision
```

Do not require every heading for every response.

## AI Consumption Guidance

Authorized agents should:

1. Establish discovery intent.
2. Discover proportionally.
3. Evaluate Status and Authority Level together.
4. Apply OLY-GOV-003 for authority.
5. Inspect relationships when material.
6. Preserve project and portfolio boundaries.
7. Cite material sources.
8. Distinguish grounding from inference.
9. Flag conflicts.
10. Stop or escalate when authority is unclear.

Authorized agents must not:

- Treat relevance as authority
- Treat Draft, Proposed, Exploratory, logs, or conversation as Approved
- Generalize project-local knowledge without promotion
- Hide material gaps
- Resolve conflicts silently
- Invent unsupported content
- Treat this standard as product architecture or an agent operating model
- Duplicate the authority hierarchy owned by OLY-GOV-003

## Relationship to Other Governance

| Asset | Relationship |
|---|---|
| OLY-GOV-001 | Repository structure and source placement |
| OLY-GOV-002 | Knowledge Asset metadata, Status, Authority Level, relationships, and AI Consumption |
| OLY-GOV-003 | Decision authority, hierarchy, approval, and conflict treatment |
| OLY-GOV-004 | Continuity sources and session resume behavior |
| OPM-001 | Agent roles and authority boundaries |
| OPM-002 | Capture and routing of knowledge discovered during work |
| OPM-003 | Promotion and approval routing |
| GDR-001 | Canonical identifier convention |
| ACR-001 / ACR-002 | Exploratory conceptual context |

When discovery identifies a conflict, missing decision, or candidate asset, route it through the owning governance or operating artifact rather than resolving it inside OLY-GOV-005.

## Review and Maintenance

| Activity | Owner | Cadence |
|---|---|---|
| Standard review | John S. Villasenor | As Needed |
| Practical validation | Hermes coordination; implementation agents under John direction | During real use |
| Cross-reference alignment | Knowledge Stewardship / Governance | When owning sources change |

## Open Questions

- What practical validation is required before OLY-DB-009 can be closed?
- What citation density is appropriate for high-impact external work?
- What minimum metadata is required before an asset may be used for high-impact work?
- How should stale or conflicting sources affect stated confidence?

## Exceptions

Exceptions require explicit Founder approval and should be recorded in an appropriate decision or change history.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-22 | Hephaestus under John direction | Initial Draft / Advisory standard for OLY-DB-009 |
| 2026-07-22 | Hephaestus under John direction | Clarified consumption versus build-time stewardship and removed premature runtime and participation models |
| 2026-07-22 | Hephaestus under John direction | Refined discovery classes, authorization versus authority, project-local boundaries, conflict handling, and stop / escalate behavior |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory guidance; retained practical validation under OLY-DB-009; removed duplicate authority hierarchy and made OLY-GOV-003 the authoritative reference |