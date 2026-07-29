# Olympus Phase 2 Product Definition Brief

> **Status:** Draft / Advisory. This working asset consolidates Phase 2 discovery and tracks progress toward the Product Gate. It does not approve the Product Vision, MVP, product requirements, application governance, architecture, technical stack, or implementation.

## Metadata

| Field | Value |
|---|---|
| Title | Olympus Phase 2 Product Definition Brief |
| Classification | Product Definition |
| Category | Product |
| Status | Draft |
| Authority Level | Advisory |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Primary AI Owner | Hermes |
| Created On | 2026-07-29 |
| Last Updated | 2026-07-29 |
| Review Cadence | At each material discovery update and before the Product Gate |
| Related Assets | [[OPM-004_OLYMPUS_PRODUCT_TO_ARCHITECTURE_ROADMAP|OPM-004]]; [[HND-001_OLYMPUS_FOUNDATION_GATE_PACKET|HND-001]]; [[MT_OLYMPUS_FOUNDATION_BRIEF|Olympus Foundation Brief]]; [[GDR-001_OLYMPUS_ID_CONVENTION|GDR-001]]; [[GDR-003_OLYMPUS_CONCEPTUAL_CAPABILITY_MODEL|GDR-003]]; [[GDR-004_EUNOMIA_ECOSYSTEM_STEWARDSHIP_ROLE|GDR-004]] |
| AI Consumption | Required |
| Change Impact | High |

---

## 1. Purpose

This brief is the durable working record for **Phase 2: Product Discovery and Definition** under [[OPM-004_OLYMPUS_PRODUCT_TO_ARCHITECTURE_ROADMAP|OPM-004]].

It exists to:

- consolidate confirmed Founder direction, working hypotheses, candidate requirements, open questions, and approvals;
- prevent conversational discovery from being mistaken for approved product scope;
- track completion of the Phase 2 required outputs and exit criteria;
- provide a coherent review package for the Product Gate;
- constrain later application-governance and architecture work only after the relevant product decisions are approved.

This brief is not a decision record. Product decisions requiring formal approval should be captured in `PDR-*` records as needed.

## 2. Phase Authority and Boundaries

OPM-004 defines the Phase 2 objective as determining what the future Olympus application should accomplish, for whom, and within what MVP boundary.

During Phase 2, participants must not:

- select the technical stack;
- design databases or APIs;
- assume each Olympus concept maps to a software service;
- let architecture convenience redefine product purpose;
- treat candidate capabilities as approved scope without Founder approval.

The Phase 1 Foundation Gate authorized progression into Phase 2 only. Application governance, Architect-agent definition, architecture discovery, technical validation, stack selection, and implementation remain outside the current authorization boundary.

## 3. Discovery Status Legend

| Label | Meaning |
|---|---|
| Founder-confirmed | Direction explicitly supplied or accepted by John during Phase 2 discovery |
| Working hypothesis | A proposed interpretation that has not been approved as final product direction |
| Candidate | A possible capability, requirement, measure, or boundary still under evaluation |
| Open | Evidence, clarification, or Founder decision is still required |
| Approved | Explicitly approved through the appropriate Product Gate or PDR |

## 4. Founder-Confirmed Discovery Direction

### 4.1 Initial users

The first intended users are:

> A small group of trusted E7CORE collaborators.

AI agents may consume governed context and assist those collaborators, but accountable humans remain the primary product users for the initial product definition.

### 4.2 Priority problems

The initial priority problems are:

1. Repeating context to AI tools.
2. Difficulty carrying lessons across projects.

### 4.3 Primary product value

The primary value direction is:

> Support decision-making and produce trustworthy work products.

The MVP may include deliberately small supporting portions of discovery, capture, health, provenance, and conflict-awareness capabilities where they are necessary to enable that primary value.

### 4.4 Human-control boundaries

The following activities must remain human-led:

- granting project access;
- resolving contradictions;
- changing Knowledge Asset Authority Level;
- changing Knowledge Asset Status.

Additional human-control boundaries remain to be defined during Phase 2 and Phase 3.

### 4.5 Leading success direction

The leading measurable success direction is:

> Answer authority questions correctly against a defined evaluation set.

Other desirable outcomes include reducing orientation time, reducing repeated context explanation, identifying stale or contradictory guidance, carrying lessons across projects, and producing useful cited work products. These additional measures remain candidates until operational definitions and targets are approved.

## 5. Working Product Hypothesis

> Olympus helps trusted E7CORE collaborators rapidly understand a project, apply the correct authority and accumulated experience, and produce a decision-ready work product with transparent sources, conflicts, assumptions, and human approval points.

**Status:** Working hypothesis. Not yet the approved Product Vision.

## 6. Candidate Product Principles

The following principles are candidates for review and approval:

1. **Decision value over document retrieval** — Olympus should help people decide and act, not merely locate files.
2. **Trust must be inspectable** — Important answers should expose sources, authority, provenance, assumptions, and conflicts.
3. **Human authority remains explicit** — Olympus may assist and recommend; humans retain consequential authority.
4. **Project boundaries must be preserved** — Cross-project learning must not silently turn local knowledge into portfolio-wide authority.
5. **Reuse lessons without erasing context** — Experience should travel with its provenance, limits, and confidence.
6. **MVP scope must remain narrow** — Supporting capabilities should exist only where they enable the primary decision-support workflow.

**Status:** Candidate. Not approved.

## 7. Candidate Flagship Experience

The strongest initial product experience is:

> **Orient me, show me what governs, bring forward relevant experience, and produce a decision-ready artifact.**

### 7.1 Flagship work product

**Authority-Aware Decision Brief**

A decision brief should help a collaborator understand:

- the decision or question;
- the project and scope;
- governing decisions, standards, and constraints;
- relevant context and evidence;
- prior lessons and analogous experience;
- conflicts, gaps, stale guidance, and assumptions;
- options and tradeoffs;
- a recommendation or decision framing;
- the human decision or approval required;
- source lineage and citations.

### 7.2 Supporting work products

1. **Instant Project Orientation Brief** — Rapidly establishes project purpose, phase, decisions, constraints, ownership, unresolved questions, risks, recent changes, and next actions.
2. **Cross-Project Lessons and Risk Review** — Identifies potentially relevant lessons while preserving original context, transfer limits, provenance, and confidence.

**Status:** Founder-confirmed as the direction to move forward with. Detailed scope and acceptance requirements remain unapproved.

## 8. Initial User Journey Hypothesis

1. A trusted collaborator selects or enters an authorized project context.
2. The collaborator asks a question or requests a work product.
3. Olympus discovers relevant governed knowledge within permitted boundaries.
4. Olympus evaluates source status, authority, scope, freshness, provenance, and conflicts.
5. Olympus brings forward relevant cross-project lessons without converting them into silent authority.
6. Olympus produces a cited orientation, analysis, or decision-ready artifact.
7. Olympus identifies assumptions, missing evidence, contradictions, and required human decisions.
8. Humans control access, resolve contradictions, and approve authority or status changes.

**Status:** Working hypothesis.

## 9. Candidate Capability Map

These capabilities are discovery candidates, not approved requirements.

### 9.1 Core value capabilities

- Authority-aware decision support
- Decision-ready work-product generation
- Project orientation and context synthesis
- Cross-project lesson discovery and contextualization

### 9.2 Supporting trust capabilities

- Source citation and provenance visibility
- Status and Authority Level interpretation
- Scope and project-boundary awareness
- Conflict, contradiction, and staleness detection
- Assumption and evidence-gap labeling
- Human approval and escalation identification

### 9.3 Supporting knowledge capabilities

- Knowledge Asset discovery
- Relationship navigation
- Limited intake or registration necessary to support the flagship workflow
- Collection-health signals necessary to warn about unreliable outputs

### 9.4 Deferred or unapproved capability areas

- Broad stewardship automation
- Autonomous contradiction resolution
- Autonomous status or authority changes
- Broad participating-project onboarding
- Application governance implementation
- Technical architecture or stack choices

## 10. Preliminary MVP Boundary

### 10.1 Candidate MVP outcome

The smallest useful proof should demonstrate that Olympus can take a bounded, governed source set and produce a trustworthy decision-ready work product that applies authority correctly, cites its evidence, surfaces conflicts and gaps, and preserves human approval boundaries.

### 10.2 Candidate MVP scope

- A small group of trusted E7CORE collaborators
- One or more explicitly authorized project knowledge scopes
- Authority-Aware Decision Brief as the flagship work product
- Project Orientation Brief and Cross-Project Lessons Review as supporting outputs or sections
- Authority-aware source interpretation
- Citations and provenance
- Explicit conflict, assumption, and evidence-gap reporting
- Human-controlled project access, contradiction resolution, and authority/status changes
- A defined authority-question evaluation set

### 10.3 Candidate non-goals

- A generic document chatbot
- A universal knowledge-management replacement
- Autonomous project-access grants
- Autonomous contradiction resolution
- Autonomous Authority Level or Status changes
- Full stewardship automation
- Production architecture, database, API, or technical-stack design
- Rebuilding or refactoring TripnetX as part of the Olympus product-definition phase
- Treating every Olympus conceptual role as a software service or AI agent

**Status:** Candidate. MVP boundary and non-goals require explicit Founder approval.

## 11. Evaluation Subject: Trip Builder 2.0 Refactoring Proposal

The Trip Builder 2.0 Refactoring Proposal is a representative **input case** for discovering Olympus product requirements.

Its role during Phase 2 is to help determine what Olympus must be able to do with a consequential proposal. It is not authorization to evaluate, implement, or approve the Trip Builder refactoring MVP.

The input case should help validate whether Olympus requirements address the ability to:

- recognize document type and proposal status;
- extract the decision being informed;
- distinguish observations, claims, hypotheses, recommendations, and constraints;
- discover applicable governing sources;
- identify missing evidence and unsupported claims;
- preserve explicit scope and authorization boundaries;
- connect relevant lessons without overstating transferability;
- identify the human decision owner;
- produce a trustworthy, cited work product.

## 12. Candidate Product Requirements

The following requirements are provisional and must be refined into testable product requirements.

| ID | Candidate requirement | Status |
|---|---|---|
| CPR-01 | Olympus should identify the status, authority, scope, and canonical-source posture of material sources before relying on them. | Candidate |
| CPR-02 | Olympus should distinguish source-derived facts, proposals, hypotheses, recommendations, inferences, and unresolved questions. | Candidate |
| CPR-03 | Olympus should identify the decision or work objective that a source package is intended to support. | Candidate |
| CPR-04 | Olympus should discover and prefer applicable Canonical and Governing sources over lower-authority material. | Candidate |
| CPR-05 | Olympus should cite material claims and preserve source lineage in generated work products. | Candidate |
| CPR-06 | Olympus should surface conflicts, contradictions, stale guidance, missing evidence, and scope mismatches rather than silently resolve them. | Candidate |
| CPR-07 | Olympus should preserve project boundaries and distinguish local lessons from portfolio-wide authority. | Candidate |
| CPR-08 | Olympus should identify required human decisions, approvals, or escalations. | Candidate |
| CPR-09 | Olympus should not grant project access, resolve contradictions, or change asset Status or Authority Level autonomously. | Founder-confirmed boundary; formal requirement pending |
| CPR-10 | Olympus should produce an Authority-Aware Decision Brief that is useful without hiding uncertainty or missing evidence. | Candidate |
| CPR-11 | Olympus should support progressive enrichment as additional authorized sources become available. | Candidate |
| CPR-12 | Olympus should answer authority questions correctly against a defined evaluation set. | Founder-confirmed success direction; target pending |

The `CPR-*` labels are local table identifiers only. They are not Knowledge Asset IDs and do not amend [[GDR-001_OLYMPUS_ID_CONVENTION|GDR-001]].

## 13. Candidate Success Measures

| Measure | Intended evidence | Status |
|---|---|---|
| Authority-question accuracy | Correct answer, governing source, and explanation against a defined test set | Priority candidate |
| Source-grounding quality | Material claims supported by valid citations | Candidate |
| Conflict-detection quality | Known contradictions and authority conflicts surfaced without silent resolution | Candidate |
| Orientation-time reduction | Time required for a collaborator or AI session to become productively oriented | Candidate |
| Repeated-context reduction | Reduction in manual restatement of settled project context | Candidate |
| Cross-project lesson usefulness | Relevant lessons identified with context and transfer limits | Candidate |
| Work-product usefulness | Human review score for clarity, decision readiness, and trustworthiness | Candidate |
| Human-boundary compliance | No unauthorized access, contradiction resolution, or authority/status mutation | Candidate |

Targets, baselines, evaluation methods, and acceptance thresholds remain open.

## 14. Phase 2 Required Output Tracker

| Required output from OPM-004 | Current state | Completion evidence needed |
|---|---|---|
| Product Vision | Working hypothesis exists | Founder-approved Product Vision, likely captured through this brief and/or a PDR |
| Product Principles | Candidate principles drafted | Founder review and approval |
| Stakeholder and user definitions | Initial primary user defined | Secondary users, stakeholders, responsibilities, and boundaries |
| Problem statements | Initial priority problems defined | Refined problem statements with evidence and scope |
| User journeys | Initial journey hypothesis drafted | Validated priority journeys and exception paths |
| Capability map | Initial candidate map drafted | Prioritization and approval of MVP-relevant capabilities |
| MVP definition | Preliminary boundary drafted | Explicit Founder approval |
| Non-goals | Preliminary non-goals drafted | Explicit Founder approval |
| Success measures | Candidate measures identified | Definitions, targets, test method, and prioritization |
| Product requirements | Initial candidates drafted | Refinement into sufficient, testable requirements that constrain architecture |
| PDRs as needed | None created for Phase 2 yet | Create only where durable product decisions require formal records |

## 15. Phase 2 Exit-Criteria Tracker

| Exit criterion from OPM-004 | Status | Notes |
|---|---|---|
| Product Vision is approved | Not satisfied | Working hypothesis only |
| Primary users and priority problems are defined | Partially satisfied | Initial user and problems are Founder-confirmed; formal completeness review remains |
| MVP boundary and non-goals are approved | Not satisfied | Candidate boundary exists; no approval yet |
| Prioritized capabilities and measurable outcomes are defined | Partially satisfied | Flagship experience and leading measure identified; full prioritization and targets remain |
| Product requirements are sufficient to constrain architecture | Not satisfied | Candidate requirements require refinement and validation |
| John approves entry into Application Governance | Not satisfied | Product Gate has not occurred |

## 16. Open Questions

1. Who are the secondary users and non-user stakeholders?
2. Which two or three user journeys must the MVP support end to end?
3. What minimum authorized source set is required for a trustworthy decision brief?
4. What makes an Authority-Aware Decision Brief acceptable, excellent, or unsafe?
5. Which capabilities are mandatory for the MVP versus deferred?
6. What explicit non-goals are necessary to protect scope?
7. What authority-question test set should be used, and what accuracy threshold is required?
8. How should usefulness, trust, and decision readiness be measured?
9. Which Phase 2 decisions warrant dedicated `PDR-*` records?
10. What evidence is required before the Product Gate can be approved?

## 17. Approval Record

No Phase 2 Product Gate approval has been granted.

| Field | Value |
|---|---|
| Approver | John S. Villasenor |
| Approval status | Not submitted for Product Gate approval |
| Approval date | N/A |
| Approved Product Vision | N/A |
| Approved MVP boundary | N/A |
| Approved non-goals | N/A |
| Authorization to enter Phase 3 | No |

Repository persistence, commit, merge, or publication of this Draft does not constitute approval.

## 18. Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-29 | Hermes / Hephaestus workflow | Created the Phase 2 working brief from Founder-confirmed discovery and OPM-004 requirements; retained Draft / Advisory status |
