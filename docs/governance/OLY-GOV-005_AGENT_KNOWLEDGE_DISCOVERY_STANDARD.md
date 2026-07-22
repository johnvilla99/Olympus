# Agent Knowledge Discovery Standard

> **Status:** Draft — advisory guidance, not approved or governing policy.

## Metadata

| Field | Value |
|---|---|
| Standard ID | OLY-GOV-005 |
| Title | Agent Knowledge Discovery Standard |
| Classification | Governance Standard |
| Category | Governance / Knowledge Stewardship |
| Status | Draft |
| Authority Level | Advisory |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Primary AI Owner | Hermes |
| Created On | 2026-07-22 |
| Last Updated | 2026-07-22 |
| Review Cadence | As Needed |
| Related Assets | OLY-GOV-001; OLY-GOV-002; OLY-GOV-003; OLY-GOV-004; OPM-001; OPM-002; OPM-003; ACR-001; ACR-002; Decision Backlog (OLY-DB-009); GDR-001 (Proposed); RNO-001 |
| AI Consumption | Recommended |
| Change Impact | High |

---

## Purpose

OLY-GOV-005 defines the **minimum rules** an AI agent must follow when relying on Olympus-governed knowledge to answer questions, make recommendations, or produce work.

Its purpose is to ensure that **relevant** knowledge is not mistaken for **authoritative** knowledge, and that agents preserve status, authority, provenance, scope, relationships, conflicts, assumptions, and approval boundaries when using Olympus sources.

This standard governs the **safe consumption** of Olympus-governed knowledge. It does **not** define agent roles, repository maintenance, project participation, runtime architecture, or knowledge-system implementation.

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
- Formal approval of this standard, **GDR-001**, or closure of **OLY-DB-009** / **OLY-DB-017**

## Applicability

This standard applies whenever an AI agent is **authorized** to consume Olympus-governed knowledge.

Authorization determines whether an agent may **access and use** the knowledge. It does **not** determine the authority of the knowledge itself.

The agent’s role, project, organization, or operating environment may vary. Authorization to access Olympus knowledge does **not** confer authority to approve, modify, promote, generalize, or redistribute that knowledge.

Agent roles and stewardship responsibilities remain governed by **OPM-001** and related operating models.

Project participation and adoption rules require separate governance and are **not** defined by this standard.

Future Olympus runtime behavior remains a product and architecture concern, not a rule established here.

Olympus may eventually use Metis and Muse concepts to support reasoning and domain evaluation, but this standard does **not** define their implementation. See ACR-001 and ACR-002 for exploratory conceptual context only.

## Core Consumption Rules

| Rule | Meaning |
|---|---|
| Relevant ≠ authoritative | A matching passage is not binding without Status and Authority Level evaluation |
| Status and Authority Level together | Neither field alone is sufficient |
| John is final Olympus authority | Explicit Founder direction has highest authority for Olympus governance and Olympus-owned knowledge. Project- or client-specific authority remains subject to the applicable local governance. |
| Agents do not approve | Agents discover and recommend; they do not promote assets or close decisions |
| Proposed ≠ Approved | Proposed and Draft sources guide review; they are not binding |
| ACRs are exploratory | Concept records inform context; they are not implementation authority |
| Handoffs and logs are continuity aids | They do not override formal assets |
| Research is evidence | Research notes and lessons inform; they are not decisions |
| Commit / push ≠ approval | Persistence does not change Status or Authority Level |
| Do not invent closure | Material gaps must be surfaced, not papered over |

`OLY-GOV-005` uses the current Draft / Advisory ID working convention. This standard does **not** approve **GDR-001** or close **OLY-DB-017**.

---

## 1. Discovery Intent

Before deep retrieval, the agent must identify:

1. **The user’s actual question or requested work** — not only the first phrasing.
2. **Affected project or portfolio context** — Olympus-wide vs a named project, client, or engagement.
3. **Applicable domain lenses** — Product, Governance, Architecture, Operations, Engineering, UX, Marketing, Knowledge Stewardship, or other named lenses as relevant. Research remains cross-cutting (working answer; see Decision Backlog), not a tenth Muse.
4. **Task type** — facts, decision application, advice, synthesis, implementation guidance, work-product support, continuity, or conflict investigation.
5. **Consequence of being wrong** — incomplete or low-authority knowledge may mislead recommendations or treat Exploratory content as binding.

If intent is unclear, ask a clarifying question proportional to impact.

## 2. Source Discovery Order

Use this practical search order when locating candidate sources. It is a discovery path, not an automatic ranking of truth.

| Order | Source class | Typical locations / examples |
|---|---|---|
| 1 | Explicit current Founder direction | John’s current instruction for Olympus governance, Olympus-owned knowledge, or a task where John is the authorized decision-maker; durable Founder direction captured in approved Olympus decisions when available |
| 2 | Governing and Canonical assets | Olympus assets with Authority Level **Governing** or **Canonical**, with Status that permits reliance |
| 3 | Approved decision records and approved guidance | Approved ADR/PDR/GDR/ODR and Approved standards/guidance |
| 4 | Relevant project-local authoritative assets | Approved project decisions, project governance, and other explicitly designated local authoritative sources |
| 5 | Proposed and Draft governance, decision, and operating assets | Draft or Proposed OLY-GOV, OPM, decision records, and related operating guidance (including this standard) |
| 6 | Operational continuity sources and current-state evidence | Session handoffs; daily logs; git or repository state; current evidence packets; other observable current-state evidence |
| 7 | Exploratory concept records | ACR-001, ACR-002 and similar Exploratory / Informational assets |
| 8 | Research notes and lessons learned | `RNO-*`, `docs/research/`, `docs/lessons/` |
| 9 | Conversation context | Current and prior chat turns |
| 10 | Assistant inference or general knowledge | Model priors not grounded in Olympus sources |

### Discovery order versus authority order

**Discovery order is not always the same as authority order.**

- A lower-authority source may be highly relevant.
- Relevance does **not** authorize silent override of a higher-authority source.
- When a lower-authority source conflicts with a higher-authority source, **surface the conflict**.

Formal governance and decision assets determine **authority**.

Continuity artifacts explain **recent work**.

Observable evidence verifies **current state**.

None of these should be silently substituted for another. Continuity sources and repository state are **not** decision authority.

Session resume priority for continuity sources is defined in **OLY-GOV-004**. That resume order complements this discovery order; it does not replace Founder authority over Olympus governance and Olympus-owned knowledge.

## 3. Authority Resolution

Agents must evaluate sources using **both**:

- **Status** (maturity / lifecycle)
- **Authority Level** (binding weight)

Neither field alone is sufficient. See Core Consumption Rules for Proposed ≠ Approved and ACR exploratory treatment.

### Working authority comparison (Draft / Advisory working discovery aid)

Highest to lowest for ordinary conflict resolution, subject to Status checks. This is a **Draft / Advisory working discovery aid**, not an approved final hierarchy.

1. Explicit current Founder (John) direction for Olympus governance, Olympus-owned knowledge, or tasks where John is the authorized decision-maker
2. Governing assets (when Status permits reliance)
3. Canonical assets (when Status permits reliance)
4. Approved decision records and Approved guidance
5. Proposed decisions and Proposed assets
6. Draft / Advisory standards and operating models (including this standard)
7. Exploratory / Informational concept records
8. Continuity artifacts
9. Conversation context
10. Assistant inference / general knowledge

Observable current-state evidence is not an authority level. It verifies operational facts and may confirm or contradict continuity claims, but it does not override governing, canonical, or approved direction.

If existing Olympus assets express inconsistent authority hierarchies, the agent must **flag the inconsistency** and defer to the most specific applicable approved or higher-authority source. If no clear resolution exists, escalate to John.

## 4. Metadata Interpretation

Before relying on an asset, read available metadata, especially:

| Field | Discovery use |
|---|---|
| Knowledge Asset ID | Stable citation; prefix signals asset class |
| Classification | Standard, decision, concept, research, etc. |
| Category | Domain placement for lens selection |
| Status | Whether content is safe as current guidance |
| Authority Level | Binding weight |
| Canonical Source | Whether this claims source-of-truth for its subject |
| Owner | Accountable human owner |
| Primary AI Owner | Stewardship role only; does not confer approval power |
| Last Updated | Staleness signal |
| Review Cadence | Overdue review may reduce confidence |
| Related Assets | Navigate when material |
| AI Consumption | Required / Recommended / Optional / Restricted — respect Restricted |
| Change Impact | Higher impact → deeper discovery and stricter citation |

| Condition | Agent behavior |
|---|---|
| Missing Status or Authority Level | Do not assume Approved or Canonical; flag gap |
| Incomplete ID / owner / related assets | Cite what exists; note uncertainty |
| Stale Last Updated on High Change Impact | Seek fresher related assets; flag possible outdated guidance |
| Contradictory metadata | Flag; do not silently “fix” |
| AI Consumption = Restricted | Do not rely on or surface without explicit Founder/owner permission |
| Partial seed metadata | Use cautiously for context; do not over-claim authority |

## 5. Project and Portfolio Context

| Context | Treatment |
|---|---|
| Olympus-wide knowledge | Portfolio foundation guidance |
| Project-specific knowledge | Bound to that project, engagement, or business context unless explicitly generalized |
| Local authoritative sources | Approved project decisions, project governance, and explicitly designated local sources — apply locally; do not auto-promote to portfolio guidance |
| Project continuity artifacts | Handoffs and logs explain recent local work; they are not authoritative merely because they are local |
| Cross-project lessons | May inform other work when framed as evidence with provenance |
| Non-generalizable context | Client, personnel, pricing, or temporary constraints that must stay local |

Knowledge created within a project, client engagement, program, or business context remains **local to that context** unless explicitly reviewed and promoted for broader use.

A project-local decision must **not** automatically become portfolio-wide guidance.

Broader portfolio-versus-project scope rules remain open (**OLY-DB-014** — Deferred). Do not invent a closed rule set here.

## 6. Relationship Navigation

When metadata or content identifies relationships, inspect related assets where material.

Relationship types recognized in OLY-GOV-002 / OLY-GOV-003 (link practice; graph implementation deferred):

| Relationship | Discovery implication |
|---|---|
| `informs` | Upstream context; cite when it shapes the conclusion |
| `references` | Supporting source; verify still current |
| `depends_on` | Check the dependency before applying the dependent asset |
| `supersedes` / `replaces` | Prefer the successor |
| `contradicts` | Mandatory conflict handling |
| `implements` | Realization of a decision/standard — not higher authority by itself |
| `related_to` | Adjacent context; use proportionally |

A single retrieved document must **not** be treated as isolated when its metadata identifies dependencies, replacements, or contradictions.

## 7. Conflict Handling

| Category | Example |
|---|---|
| Direct contradiction | Incompatible rules on the same subject |
| Status conflict | Approved guidance vs Exploratory content treated as decisive |
| Authority conflict | Advisory Draft vs claimed Canonical Source without matching Status |
| Outdated source | Older asset retained without supersession after newer guidance |
| Duplicate source-of-truth claim | Multiple Canonical Source Yes claims for one subject |
| Project-local vs portfolio-wide | Local decision treated as ecosystem rule (or the reverse) |
| Founder direction vs existing Olympus assets | Current John instruction for Olympus governance or Olympus-owned knowledge conflicts with repository documents |
| Continuity vs observable state | Handoff or log claims conflict with git state, evidence packets, or other current evidence |

Required behavior:

1. Surface the conflict.
2. Identify competing sources (IDs/paths).
3. State each source’s Status and Authority Level (and Canonical Source if relevant).
4. Do not silently choose a winner when authority is unclear.
5. Escalate to John when an Olympus authority decision is required.

If current explicit John direction conflicts with existing Olympus assets, follow that direction for the Olympus task and route the conflict through capture / promotion workflows (OPM-002 / OPM-003). Do not silently rewrite assets to match conversation. Project- or client-specific authority remains subject to applicable local governance.

## 8. Citation and Evidence Expectations

Cite or reference sources when:

- stating or applying an approved decision
- claiming a rule or governance requirement
- generating implementation guidance
- resolving or reporting a conflict
- producing a recommendation substantially grounded in Olympus knowledge
- producing work that materially relies on Olympus sources
- describing why a prior direction was chosen

Prefer Knowledge Asset ID, path when helpful, and section location when practical.

Do **not** require citation clutter on every ordinary sentence. Prefer proportion: low-impact orientation may need light citation; high-impact claims should cite.

## 9. Synthesis and Inference Boundaries

Distinguish, as appropriate:

| Mode | Meaning |
|---|---|
| Directly grounded fact | Stated in a cited source with adequate Status/Authority for the claim |
| Approved direction | Approved decisions/guidance or explicit Founder direction |
| Advisory guidance | Draft/Advisory standards or Recommended operating models |
| Exploratory concept | ACR or Exploratory content — context only |
| Evidence-supported inference | Reasonable conclusion from cited evidence; labeled as inference |
| Assistant recommendation | Agent proposal not yet Founder-approved |
| Unresolved gap | Missing or conflicted knowledge — surface it |
| Unsupported invention | Fluent fill-in without grounding — avoid or label as speculation for human review |

Do not paper over material gaps merely because the output format expects completeness.

## 10. Use in Work Products

When an answer, recommendation, plan, proposal, assessment, handoff, or other work product **materially relies** on Olympus-governed knowledge, the agent must preserve:

- applicable project or business context
- Status and Authority Level of material sources
- source lineage
- material assumptions
- unresolved conflicts
- known gaps
- required human approval points

These elements may be expressed explicitly or incorporated into the work product in a form appropriate to its audience and impact. Ordinary low-impact answers need not expose raw metadata; proportionality (Section 11) still applies.

Illustrative work that may rely on Olympus knowledge includes SOWs, proposals, plans, risk assessments, recommendations, and handoffs. Examples are illustrative only.

This standard governs the **integrity of knowledge use** within the work product. It does **not** define the product, service, workflow, template, or runtime mechanism used to generate that work product.

## 11. Proportionality

Discovery must not become a bureaucratic scavenger hunt.

| Impact class | Discovery depth |
|---|---|
| Low-impact factual request | Obvious governing/approved sources; light citation |
| Moderate-impact recommendation | Status/authority check on primary sources; cite basis |
| High-impact decision or implementation guidance | Fuller discovery; relationship navigation; conflict scan; escalation points |
| Durable work product | Preserve integrity elements in Section 10 |
| Governance or authority-changing request | Stop for Founder approval |

**Depth scales with the consequence of being wrong.**

## 12. Stop and Escalation Conditions

**Stop** when proceeding would create false authority or unsupported certainty.

**Continue with labeled limitations** when useful work remains possible despite gaps or uncertainty.

**Escalate** when a human authority decision is required.

Conditions that typically require stop and/or escalate:

- Required sources are unavailable or unreadable
- Restricted assets appear necessary
- Authority cannot be determined for a material claim
- Competing Canonical or Governing sources exist without a clear supersession path
- Founder approval would be required for Olympus governance or Olympus-owned knowledge
- The request would resolve an open backlog item without authorization
- The task crosses into unapproved product or architecture scope unless John explicitly scopes it
- Evidence is too weak for the requested certainty
- Continuity claims conflict with observable state and proceeding would bake in false context

Escalate Olympus authority decisions to **John**. Coordination roles may recommend; they do not approve. See OPM-001. Local project or client authority remains subject to applicable local governance.

## 13. Output Expectations

When appropriate and proportional, structure responses with some or all of:

```text
Conclusion or Work Product
Authority Basis
Sources Used
Conflicts or Gaps
Assumptions / Inference
Recommended Human Decision
```

Do **not** mandate all headings for every response. Apply by impact class (Section 11).

---

## AI Consumption Guidance

Authorized agents **should**:

1. Establish discovery intent.
2. Discover proportionally.
3. Evaluate Status and Authority Level together.
4. Inspect relationships when material.
5. Preserve project and portfolio boundaries.
6. Cite material sources.
7. Distinguish grounding from inference.
8. Flag conflicts.
9. Stop or escalate when authority is unclear.

Authorized agents **must not**:

- Treat relevance as authority
- Treat Draft, Proposed, Exploratory, logs, or conversation as Approved
- Generalize project-local knowledge without explicit promotion
- Hide material gaps
- Resolve conflicts silently
- Invent unsupported content
- Treat this standard as product architecture or an agent operating model

## Relationship to Other Governance

OLY-GOV-005 governs how Olympus-governed knowledge is **consumed**.

OLY-GOV-001 through OLY-GOV-004 govern repository structure, Knowledge Assets, decisions, and session continuity.

OPM-001 through OPM-003 govern agent roles, capture, promotion, and approval workflows.

When discovery identifies a conflict, missing decision, or candidate asset, route the issue through those standards rather than resolving it inside OLY-GOV-005.

## Relationship to Other Standards

| Asset | Relationship |
|---|---|
| OLY-GOV-001 | Repository structure and source placement |
| OLY-GOV-002 | Knowledge Asset metadata, status, authority, relationships, and AI Consumption |
| OLY-GOV-003 | Decision records and decision authority |
| OLY-GOV-004 | Continuity sources and session resume behavior |
| OPM-001 | Agent roles and authority boundaries |
| OPM-002 | Capture and routing of knowledge discovered during work |
| OPM-003 | Promotion and approval routing |
| ACR-001 / ACR-002 | Exploratory conceptual context for memory, judgment, Muses, and activation |

## Prohibited Practices

- Claiming this Draft is Approved, Canonical, or Governing
- Using this standard to define agent taxonomies, project adoption, or runtime architecture
- Equating semantic similarity or retrieval relevance with authority
- Treating Muse names as agent identities
- Inferring Founder approval from commit, push, or silence
- Closing backlog items by implication
- Creating paperwork that does not improve safe knowledge use

## Review / Maintenance

| Activity | Owner | Cadence |
|---|---|---|
| Standard review | John S. Villasenor | As Needed |
| Practical validation during foundation work | Hermes coordination; Hephaestus implementation under John | As Needed |
| Hierarchy-language alignment | Governance | When John decides to unify hierarchy wording |

## Exceptions

Exceptions require explicit Founder approval and should be recorded as a decision or noted in change history.

## Open Questions

- Should authority hierarchy language across OLY-GOV-003, Governance Starter, and OPM-001 be formally unified?
- What citation density is appropriate for high-impact external work?
- What minimum metadata is required before an asset may be used for high-impact work?
- How should stale or conflicting sources affect stated confidence?
- What practical validation is required before OLY-DB-009 moves beyond Partially Addressed?

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-22 | Hephaestus (under John direction) | Initial Draft / Advisory standard for OLY-DB-009 working answer: agent discovery, authority resolution, citation, conflict handling, and knowledge activation boundaries. Not Approved. |
| 2026-07-22 | Hephaestus (under John direction) | Clarified consumption vs build-time stewardship; introduced temporary agent-context and adoption language later removed. Not Approved. |
| 2026-07-22 | Hephaestus (under John direction) | Reframed the standard around safe consumption of Olympus-governed knowledge. Removed premature agent-context, project-participation, and runtime-agent definitions; reduced duplication with existing governance and operating models; preserved the core discovery, authority, citation, conflict, and synthesis rules. No approval or promotion. |
| 2026-07-22 | Hephaestus (under John direction) | Final Draft refinement: removed overlap in source discovery classes, clarified formal authority versus continuity and observable state, separated authorization from source authority, and tightened Olympus versus local governance boundaries. Discovery model preserved. No approval or promotion. |
