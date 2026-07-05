# Knowledge Asset Standard

> **Status:** Draft — advisory guidance, not approved or governing policy.

## Metadata

| Field | Value |
|---|---|
| Standard ID | OLY-GOV-002 |
| Title | Knowledge Asset Standard |
| Status | Draft |
| Authority Level | Advisory |
| Owner | John S. Villasenor |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-05 |
| Review Cadence | As Needed |
| Related Assets | Foundation Brief; Knowledge Asset Model; Governance Starter; Repository Standard; ACR-001; ACR-002; Muse Catalog Starter; Decision Backlog |

---

## Purpose

Make Knowledge Assets **trustworthy, discoverable, maintainable, and safe** for humans and AI agents to consume.

A Knowledge Asset is **not merely a file**. It is a governed container for meaning — preserving not only what is known, but why it matters, who owns it, whether it is authoritative, and how future work should use it.

This standard translates `docs/foundation/KNOWLEDGE_ASSET_MODEL.md` into practical rules for the Olympus repository. It prevents:

- Notes mistaken for authoritative guidance
- Exploratory concepts treated as implementation authority
- Assets without metadata that future agents cannot evaluate safely
- Duplicate or conflicting sources of truth
- Experience and lessons lost because they were never promoted when they had decision value

## Scope

Applies to **formal Knowledge Assets** stored in the Olympus repository during the governed knowledge foundation phase.

**In scope:**

- Metadata requirements
- Asset categories and typical placement
- Status and authority levels
- AI consumption guidance
- Creation, placement, promotion, maintenance, supersession, and retirement rules
- Relationship, citation, and experience capture guidance

**Out of scope:**

- Final database schema or storage implementation
- Application UI or automation pipelines
- External project repository standards (unless explicitly adopted by decision)
- Promotion of any current asset to **Approved**, **Canonical**, or **Governing** status in this document

## Definition of a Knowledge Asset

A **Knowledge Asset** is a durable unit of preserved knowledge useful for future reasoning, decision-making, continuity, or execution.

Every formal Knowledge Asset should help future humans or AI agents understand:

- **Why** something mattered
- **Who** owns it
- **Whether** it is authoritative
- **What decisions** it informs
- **What context** would otherwise be lost
- **How** future agents should use it

If a document cannot answer these questions, it may not yet qualify as a formal Knowledge Asset.

## What Qualifies as a Knowledge Asset

Examples of content that may qualify when properly governed:

| Type | Example |
|---|---|
| Concept Record | ACR-001, ACR-002 |
| Decision Record | Approved architecture or governance decision with rationale |
| Governance Standard | OLY-GOV-001 Repository Standard |
| Product Definition | Product brief, MVP definition, scope statement |
| Architecture Definition | Architecture overview after product/governance clarity |
| Lesson Learned | Postmortem, retrospective, failure analysis |
| Research Note | Competitive or technical research with evidence |
| Operating Model | Agent operating model, stewardship workflow |
| Handoff / Continuity Artifact | Session handoff promoted for durable continuity value |

An asset qualifies when it has **future decision or continuity value**, accountable ownership, honest status, and metadata consistent with this standard.

## What Does Not Qualify as a Knowledge Asset

Examples of content that does **not** qualify as a formal Knowledge Asset:

- Scratch notes with no future decision value
- Raw chat transcripts unless curated into a useful artifact
- Duplicate copies of existing knowledge without canonical-source reference
- Temporary logs under `logs/` unless promoted to a governed asset
- Application source code, package manifests, or build artifacts
- Secrets, credentials, or environment values
- Vague ideas with no context, owner, or stated future use
- Templates under `templates/` (starters only — copy before use)
- Directory `README.md` index files (navigation, not governed assets)

## Asset Categories

| Category | Purpose | Typical Location |
|---|---|---|
| Concept Record | Preserve an emerging idea before it becomes a decision | `docs/concepts/` |
| Decision Record | Capture an approved decision and rationale | `docs/decisions/` |
| Governance Standard | Define rules for how work is done | `docs/governance/` |
| Product Definition | Define user value, scope, principles, and outcomes | Future `docs/product/` (candidate); until then `docs/foundation/` or `docs/projects/` by scope |
| Architecture Definition | Define technical structure after product/governance clarity | Future `docs/architecture/` (candidate); until then `docs/concepts/` until structure matures |
| Lesson Learned | Preserve experience from success, failure, or surprise | `docs/lessons/` |
| Research Note | Capture evidence and analysis | `docs/research/` |
| Operating Model | Define roles, responsibilities, and workflows | `docs/operations/` |
| Handoff / Continuity Artifact | Preserve current project state for session continuity | `logs/` for operational continuity; promote durable artifacts to `docs/operations/` or the relevant `docs/` folder |

Future directories (`docs/product/`, `docs/architecture/`) are **candidates only** — do not create them in this pass unless explicitly directed.

## Required Metadata

Every formal Knowledge Asset should include the following metadata fields. Use table format in the document body or YAML front matter when creating new assets.

| Field | Meaning |
|---|---|
| **Knowledge Asset ID** | Stable identifier (e.g. ACR-001, OLY-GOV-002). Enables linking, supersession, and citation. |
| **Title** | Human-readable name describing the asset's subject. |
| **Classification** | Asset type (Concept Record, Decision Record, Governance Standard, etc.). |
| **Category** | Knowledge domain (Foundation, Governance, Architecture, Product, etc.). |
| **Status** | Maturity state — see Status Model. Must be honest and current. |
| **Authority Level** | Binding weight — see Authority Levels. |
| **Canonical Source** | Yes or No — whether this asset is the source of truth for its subject. |
| **Owner** | Accountable human owner responsible for accuracy and maintenance. |
| **Primary AI Owner** | AI role or agent responsible for stewardship, if any (e.g. proposed Curator). |
| **Created On** | Date the asset was first created (ISO date). |
| **Last Updated** | Date of the latest material update (ISO date). |
| **Review Cadence** | Expected review rhythm (As Needed, Quarterly, Annually, etc.). |
| **Related Assets** | Linked records, dependencies, or lineage (IDs or paths). |
| **AI Consumption** | How agents should treat this asset — Required, Recommended, Optional, or Restricted. |
| **Change Impact** | Low, Medium, or High — indicates scrutiny required when changing this asset. |

**Seed assets** may lack full metadata until their next substantive edit. Add missing fields when revising; do not backfill speculatively.

Recommended content sections (from `templates/knowledge-assets/KNOWLEDGE_ASSET_TEMPLATE.md`): Purpose, Context, Content, Authority Notes, AI Usage Guidance, Related Decisions, Open Questions, Change History.

## Status Model

| Status | Meaning |
|---|---|
| **Exploratory** | Captures an emerging idea; **not a decision**. Safe to read for context; unsafe to treat as binding guidance. |
| **Draft** | Being shaped into a usable artifact. Content may change substantially. |
| **Proposed** | Ready for review or approval. Stable enough for structured feedback. |
| **Approved** | Accepted as current guidance. Requires Founder approval before assignment. |
| **Canonical** | Source of truth for a defined topic. Requires Founder approval before assignment. |
| **Superseded** | Replaced by a newer asset. Preserved for history; must link to replacement. |
| **Retired** | No longer active. Preserved for history with retirement rationale. |

**Current repository assets remain at their existing statuses.** This standard does not promote any asset.

Agents must not treat **Exploratory** or **Draft** assets as final decisions or implementation authority.

## Authority Levels

| Level | Meaning | Agent behavior |
|---|---|---|
| **Informational** | Provides context only | May inform reasoning; not binding. |
| **Advisory** | Recommended guidance, not binding | Should be weighed; may be overridden by higher authority. |
| **Canonical** | Source of truth for a defined topic | Prefer over lower-authority assets on the same subject. |
| **Governing** | Controls process, standards, or authority | Highest repository-level guidance after Founder direction. |

Agents must **not** treat **Informational** assets or **Exploratory**-status content as binding. When authority is unclear, flag the conflict and defer to Founder direction.

## Canonical Source Rules

- **One canonical source per subject** unless explicitly justified and documented.
- If duplicate content exists, one asset must be identified as canonical; others must reference it.
- **Canonical** status requires explicit **Founder approval**.
- Exploratory concept records (e.g. ACR-001, ACR-002) are **not canonical**.
- Root `README.md` is a **front door** — orientation and pointers — not the canonical source for all repository content.
- `LICENSE` remains the **proprietary licensing authority** for repository usage rights.
- Governance standards at **Draft / Advisory** status (including this standard) are not canonical until promoted.

## AI Consumption Rules

AI agents working in or with this repository **must**:

1. **Check status** before relying on an asset's content.
2. **Check authority level** before using an asset as guidance.
3. **Prefer** governing and canonical assets over exploratory and informational assets.
4. **Cite or reference** source documents when making recommendations.
5. **Distinguish** approved decisions from inferred or conversational guidance.
6. **Flag conflicts** between assets rather than silently resolving them.
7. **Not use restricted assets** unless explicitly allowed by the Founder or asset owner.

**AI Consumption values:**

| Value | Meaning |
|---|---|
| **Required** | Agents should read and apply this asset when working in its domain. |
| **Recommended** | Agents should consult this asset when relevant; not mandatory for every session. |
| **Optional** | Agents may consult for additional context. |
| **Restricted** | Agents must not rely on or surface this asset without explicit permission. |

## Asset Creation Rules

- **Start from the appropriate template** in `templates/` when possible.
- **Assign a stable ID** using established prefix conventions (ACR-*, OLY-GOV-*, decision IDs TBD).
- **Complete metadata** before treating the document as a formal Knowledge Asset.
- **Set initial status honestly** — default to Exploratory or Draft for new concepts and standards.
- **Include** purpose, context, authority notes, AI usage guidance, related decisions, open questions, and change history where applicable.
- **Do not create an asset** unless it will help future reasoning, decision-making, continuity, or execution.
- **One primary concern per asset** — link related content instead of duplicating.

## Asset Placement Rules

Align with `docs/governance/REPOSITORY_STANDARD.md` (OLY-GOV-001):

- Formal Knowledge Assets belong under **`docs/`** in the appropriate subdirectory — not repository root.
- **Templates** stay under `templates/` (copy before filling in).
- **Operational logs** stay under `logs/` until promoted.
- Match category to directory per the Asset Categories table above.
- Use directory `README.md` files for navigation; governed content lives in named asset files.

## Asset Promotion Rules

**Promotion path:**

```text
Exploratory idea → Concept Record → Proposed Decision or Standard → Approved Artifact → Canonical Source, where appropriate
```

**Promotion requirements:**

- Not every concept should be promoted. Many should remain preserved but non-binding.
- Promotion requires: clear problem, known owner, downstream value, and maintenance responsibility.
- **Founder approval is required** for **Approved**, **Canonical**, or **Governing** status.
- Promotion should update **Related Assets** on affected documents and the **Decision Backlog** (`docs/decisions/MT_OLYMPUS_DECISION_BACKLOG.md`) when applicable.
- Do not promote assets silently — record the promotion in Change History and, for significant promotions, in a decision record.

## Asset Review and Maintenance

- **Review cadence** should be explicit in metadata (default: As Needed during foundation phase).
- Update **Last Updated** on every material change.
- Record meaningful changes in **Change History** (date, author, summary).
- **Review stale assets** before relying on them — check Last Updated and Review Cadence.
- Assets with **High** change impact should receive more scrutiny before and after edits.
- Owner is accountable for keeping status and authority level accurate.

## Supersession and Retirement

- **Superseded** assets remain in the repository for historical continuity.
- Superseded assets must **point to the replacement** asset (ID and path).
- **Retired** assets must explain why they are no longer active.
- Do **not delete** historical assets casually — prefer supersession or retirement with rationale.
- When superseding, update Related Assets on both old and new documents.

## Relationship and Citation Rules

- **Related Assets** should identify dependencies, source lineage, and relevant decisions.
- Use **citations or links** (asset ID and path) when making recommendations based on governed content.
- **Flag conflicts** between assets — do not silently merge or override.
- Exploratory **relationship types** (no graph implementation in this pass) may include:

| Type | Meaning |
|---|---|
| `informs` | Source provides context for target |
| `supersedes` | Source replaces target |
| `contradicts` | Source conflicts with target — flag for resolution |
| `depends_on` | Source requires target to be understood |
| `references` | Source cites target |
| `replaces` | Source is the successor to target |
| `related_to` | General association |

Relationship modeling beyond markdown links is **exploratory** — see Decision Backlog (graph-based relationships deferred).

## Experience Capture Rules

Drawing on exploratory concepts in ACR-002 — **not approved architecture**:

- Experience is often captured first as **lessons, observations, failures, surprises, tradeoffs, or patterns** — not as polished documents.
- **Not every experience event** is a formal Knowledge Asset. Session handoffs and daily logs may hold raw capture under `logs/`.
- Experience should be **promoted** to a Lesson Learned or related asset when it has **future decision value**.
- When promoting captured experience, include:
  - **What happened**
  - **Why it mattered**
  - **Lesson learned**
  - **Future use** — what decision or work this should inform
  - **Related assets**
  - **Confidence** — how strongly the lesson should be weighed (exploratory framing)

Do **not** implement `experience_events` schema, database tables, or application design in this pass. ACR-002's capture structures remain conceptual exploration only.

## Prohibited Practices

- Treating every note as authoritative
- Creating formal assets with **missing metadata**
- Creating **duplicate assets** without canonical-source references
- Treating **exploratory ACRs** as implementation authority
- **Promoting assets** to Approved, Canonical, or Governing without Founder approval
- **Deleting superseded assets** without preservation rationale
- Storing **secrets or credentials** in Knowledge Assets
- Creating **paperwork** that does not help future decision quality
- Assigning **Canonical Source: Yes** to multiple conflicting documents on the same subject

## Exceptions

- Exceptions require **Founder approval** only.
- Document exceptions in the affected asset's Change History or in a decision record.
- Temporary placement exceptions (e.g. seed assets during directory migration) should be noted in the relevant directory `README.md` until resolved.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial draft (OLY-GOV-002) |
