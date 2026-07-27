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
| Last Updated | 2026-07-27 |
| Review Cadence | As Needed |
| Related Assets | GDR-001; GDR-005; GDR-006; GDR-007; OLY-GOV-001 through OLY-GOV-004; OPM-001 through OPM-004; RNO-002; Decision Backlog (OLY-DB-009) |
| AI Consumption | Recommended |
| Change Impact | High |

---

## Purpose

OLY-GOV-005 defines the minimum rules an AI agent follows when relying on Olympus-governed knowledge. Discovery is authority-aware selection and use of knowledge, not retrieval alone.

## Scope

**In scope:** discovery intent, source discovery, metadata interpretation, project boundaries, relationships, conflict handling, citation, synthesis boundaries, proportionality, escalation, and work-product integrity.

**Out of scope:** agent taxonomy, project adoption, runtime architecture, Metis or Muse implementation, asset creation and approval, application code, schemas, APIs, UI, vector search, or vendor selection.

## Core Consumption Rules

| Rule | Meaning |
|---|---|
| Relevant is not authoritative | Matching content is not binding without metadata and scope evaluation |
| Metadata dimensions together | Evaluate Status, Authority Level, and Canonical Source under GDR-005 |
| Authority basis | Resolve authority through GDR-006 and preserve applicable local governance |
| Agents do not approve | Agents discover, synthesize, and recommend |
| Proposed is not Approved | Draft and Proposed sources support review, not binding direction |
| ACRs are exploratory | Concepts inform context but are not implementation authority |
| Handoffs and logs are continuity | They do not override formal authority |
| Research is evidence | Research and lessons inform but are not decisions |
| Commit or push is not approval | Persistence does not change authority |
| Do not invent closure | Material gaps and conflicts must be surfaced |

Identifiers are governed by GDR-001. This standard does not alter Approved decisions or close OLY-DB-009.

## 1. Discovery Intent

Before deep retrieval, identify:

1. The actual question or requested work.
2. The affected project, client, or portfolio scope.
3. Applicable domain lenses.
4. The task type: fact, decision application, advice, synthesis, implementation guidance, continuity, or conflict investigation.
5. The consequence of being wrong.

Clarification depth should be proportional to impact.

## 2. Source Discovery Order

Use this practical discovery path; it is not itself an authority hierarchy:

1. Explicit current authorized human direction.
2. Governing and Canonical assets.
3. Approved decisions and guidance.
4. Applicable project-local authoritative assets.
5. Proposed and Draft governance, decisions, and operating assets.
6. Continuity sources and current-state evidence.
7. Exploratory concept records.
8. Research notes and lessons.
9. Conversation context.
10. Assistant inference or general knowledge.

A lower-authority source may be relevant but cannot silently override higher applicable authority. Observable evidence verifies current facts; it is not an Authority Level.

## 3. Authority Resolution

Use **GDR-006** as the Governing Olympus authority hierarchy and **GDR-005** for metadata semantics. OLY-GOV-005 applies those decisions and does not restate their definitions.

When authority remains unclear, surface the competing sources and escalate to John or the applicable local authority.

## 4. Metadata Interpretation

Review available ID, Classification, Category, Status, Authority Level, Canonical Source, Owner, Primary AI Owner, Last Updated, Review Cadence, Related Assets, AI Consumption, and Change Impact.

| Condition | Agent behavior |
|---|---|
| Missing material metadata | Do not assume approval or source-of-truth authority |
| Incomplete ID, owner, or relationships | Cite what exists and state uncertainty |
| Stale High-impact source | Seek fresher related evidence and flag possible staleness |
| Contradictory metadata | Flag; do not silently repair |
| Restricted asset | Do not rely on or surface without permission |
| Partial seed metadata | Use cautiously and avoid over-claiming |

## 5. Project and Portfolio Context

Knowledge created within a project, client engagement, program, or business context remains local unless explicitly reviewed and promoted for broader use. A project-local decision does not automatically become portfolio guidance.

OLY-DB-014 remains deferred; do not invent closed portfolio-versus-project rules.

## 6. Relationship Navigation

Inspect material relationships such as `informs`, `references`, `depends_on`, `supersedes`, `replaces`, `contradicts`, `implements`, and `related_to`. Do not treat a retrieved document as isolated when its metadata points to dependencies, replacements, or conflicts.

## 7. Conflict Handling

Conflicts include direct contradictions, lifecycle mismatch, authority mismatch, outdated sources, duplicate Canonical claims, project-versus-portfolio mismatch, current direction versus repository assets, and continuity claims versus observable state.

Required behavior:

1. Surface the conflict.
2. Identify competing sources.
3. State material metadata and scope.
4. Do not silently choose a winner when authority is unclear.
5. Escalate when a human authority decision is required.

Current explicit authorized direction may control the immediate task under GDR-006, but durable conflicts must be routed through OPM-002 and OPM-003 rather than silently rewriting history.

## 8. Citation and Evidence

Cite or reference sources when applying approved decisions, claiming governance requirements, giving implementation guidance, reporting conflicts, grounding recommendations, producing durable work, or explaining prior rationale.

Citation density should be proportional to impact.

## 9. Synthesis and Inference Boundaries

Distinguish:

- Directly grounded fact
- Approved direction
- Advisory guidance
- Exploratory concept
- Evidence-supported inference
- Assistant recommendation
- Unresolved gap
- Unsupported invention

Do not fill material gaps merely because an output format expects completeness.

## 10. Use in Work Products

When a work product materially relies on Olympus-governed knowledge, preserve project context, source metadata, lineage, assumptions, conflicts, gaps, and required human approval points in a form appropriate to the audience.

## 11. Proportionality

| Impact | Discovery depth |
|---|---|
| Low-impact factual request | Obvious authoritative sources and light citation |
| Moderate recommendation | Metadata check and cited basis |
| High-impact decision or implementation guidance | Fuller discovery, relationship review, conflict scan, escalation points |
| Durable work product | Preserve source integrity and approval boundaries |
| Authority-changing request | Stop for authorized human approval |

## 12. Stop and Escalation

Stop or escalate when required sources are unavailable, Restricted assets appear necessary, material authority cannot be determined, competing Canonical or Governing sources exist, approval is required, a backlog item would be closed without authority, work crosses into an unapproved phase, evidence is too weak, or continuity conflicts with observable state.

Continue with labeled limitations when useful work remains possible without false certainty.

## 13. Output Expectations

When proportional, include:

```text
Conclusion or Work Product
Authority Basis
Sources Used
Conflicts or Gaps
Assumptions or Inference
Recommended Human Decision
```

## AI Consumption Guidance

Authorized agents should establish intent, discover proportionally, evaluate metadata together, inspect relationships, preserve scope boundaries, cite material sources, distinguish grounding from inference, flag conflicts, and stop or escalate when needed.

They must not treat relevance as authority, generalize local knowledge without promotion, hide gaps, silently resolve conflicts, invent unsupported content, or treat this standard as product architecture.

## Relationship to Other Governance

- OLY-GOV-001: repository structure and placement
- OLY-GOV-002: Knowledge Asset lifecycle and metadata procedure
- OLY-GOV-003: decision-record procedure
- OLY-GOV-004: continuity and resume behavior
- OPM-001: agent roles
- OPM-002: knowledge capture
- OPM-003: promotion and approval
- RNO-002: Phase 1 practical validation

## Review and Maintenance

| Activity | Owner | Cadence |
|---|---|---|
| Standard review | John S. Villasenor | As Needed |
| Practical validation | RNO-002 records Phase 1 validation; repeat when material behavior changes |
| Authority alignment | GDR-005 and GDR-006 control |

## Open Questions

- What citation density is appropriate for high-impact external work?
- What minimum metadata is required before an asset may be used for high-impact work?
- How should stale or conflicting sources affect stated confidence?
- What additional promotion, if any, should follow RNO-002 validation?

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-22 | Hephaestus under John direction | Created and refined the discovery and safe-consumption standard. |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory guidance. |
| 2026-07-27 | Hermes under explicit Founder direction | Applied GDR-005 and GDR-006 by reference, recorded RNO-002 validation, and removed pre-GDR-001 language. |
