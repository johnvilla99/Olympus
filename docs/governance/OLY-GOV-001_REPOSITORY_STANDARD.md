# Repository Standard

> **Status:** Draft — advisory guidance, not approved or governing policy.

## Metadata

| Field | Value |
|---|---|
| Standard ID | OLY-GOV-001 |
| Title | Repository Standard |
| Status | Draft |
| Authority Level | Advisory |
| Owner | John S. Villasenor |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-05 |
| Review Cadence | As Needed |
| Related Assets | Foundation Brief; Knowledge Asset Model; Governance Starter; ACR-001; ACR-002 |

---

## Purpose

Define how the Mt. Olympus repository is organized, maintained, and consumed so future humans and AI agents can find authoritative knowledge safely without treating exploratory material as implementation authority.

This standard prevents:

- Knowledge scattered at the repository root or in unstructured locations
- Duplicate or conflicting sources of truth
- Exploratory concept records mistaken for approved decisions
- Session continuity artifacts polluting governed asset directories
- Proprietary repository contents handled as if publicly licensed

## Scope

Applies to the **Olympus** Git repository (`~/dev/Olympus`) during the governed knowledge foundation phase.

In scope:

- Directory layout and responsibilities
- File placement, naming, and metadata expectations
- Template, log, and Cursor rule conventions

Out of scope:

- Application implementation, databases, APIs, or UI design
- Participating project repositories (unless they adopt this standard by explicit decision)
- Promotion of any asset to **Approved**, **Canonical**, or **Governing** status (requires Founder approval)

## Repository Structure

```text
Olympus/
├── README.md                 # Repository front door
├── LICENSE                   # Proprietary license
├── .gitignore
├── docs/                     # Governed Knowledge Assets
│   ├── foundation/
│   ├── governance/
│   ├── concepts/
│   ├── decisions/
│   ├── muses/
│   ├── operations/
│   ├── research/
│   ├── lessons/
│   └── projects/
├── templates/                # Starter templates (not governed assets)
│   ├── knowledge-assets/
│   ├── decisions/
│   ├── sessions/
│   └── governance/
├── logs/                     # Operational and session logs
│   └── daily/
└── .cursor/
    └── rules/                # Cursor agent behavior guidance
```

## Directory Responsibilities

| Path | Role |
|---|---|
| `docs/foundation/` | Ecosystem purpose, scope, conceptual model, project instructions |
| `docs/governance/` | Authority, maturity, and process standards |
| `docs/concepts/` | Exploratory concept records (ACR-*) |
| `docs/decisions/` | Decision records and decision backlog |
| `docs/muses/` | Muse catalog and domain-of-expertise definitions |
| `docs/operations/` | Operating models, workflows, stewardship |
| `docs/research/` | Research notes and evidence (cross-cutting activity) |
| `docs/lessons/` | Lessons learned and retrospective knowledge |
| `docs/projects/` | Cross-project participation and ecosystem context |
| `templates/` | Blank templates for creating new artifacts |
| `logs/daily/` | Date-oriented operational and session activity logs |
| `.cursor/rules/` | Persistent AI agent instructions for this repository |

Each directory should include a `README.md` explaining purpose, what belongs, and what does not.

## File Naming Rules

- Use **UPPER_SNAKE_CASE** for formal Knowledge Asset filenames (e.g. `OLY-GOV-001_REPOSITORY_STANDARD.md`, `GDR-001_OLYMPUS_ID_CONVENTION.md`).
- Use stable **ID prefixes** per `OLY-GOV-002_KNOWLEDGE_ASSET_STANDARD.md` (OLY-GOV-002):

  | Prefix | Asset Type |
  |---|---|
  | `ACR` | Architectural Concept Record |
  | `OLY-GOV` | Olympus Governance Standard |
  | `ADR` | Architecture Decision Record |
  | `PDR` | Product Decision Record |
  | `GDR` | Governance Decision Record |
  | `ODR` | Operating Decision Record |
  | `LLR` | Lesson Learned Record |
  | `RNO` | Research Note |
  | `OPM` | Operating Model |
  | `HND` | Handoff / Continuity Artifact |

  Use sequential three-digit numbering (e.g. `ACR-001`, `OLY-GOV-001`). Draft / Advisory until formally promoted.
- Prefer descriptive suffixes over opaque abbreviations.
- Do not rename assets casually; record supersession when replacing an asset.
- `README.md` is reserved for directory index files.

## Knowledge Asset Placement Rules

- Formal Knowledge Assets belong under the appropriate `docs/` subdirectory — not at repository root.
- Match asset type to directory:
  - Concept records → `docs/concepts/`
  - Governance standards → `docs/governance/`
  - Decision records and backlog → `docs/decisions/`
  - Research notes → `docs/research/`
  - Lessons learned → `docs/lessons/`
- Every formal Knowledge Asset should include metadata consistent with `docs/foundation/KNOWLEDGE_ASSET_MODEL.md`.
- Check **Status** and **Authority Level** before relying on content.
- Do not promote exploratory records to **Approved** or **Canonical** without explicit Founder approval.

## Source Document Rules

- Root `README.md` is the **front door** — orientation, scope, and pointers — not the full knowledge base.
- `LICENSE` must remain **proprietary / all rights reserved** unless the Founder explicitly changes it.
- Prefer linking to canonical sources over duplicating content.
- When duplication is necessary, one document must clearly identify the canonical source.
- Seed assets at legacy paths should be relocated to appropriate subdirectories when structure matures.
- Founder direction outranks all repository documents.

## Template Rules

- Templates live under `templates/` and are **draft starters**, not governed assets.
- Copy a template into the appropriate `docs/` subdirectory before filling it in.
- Assign an ID, set initial status to **Draft** or **Exploratory**, and complete metadata before treating the result as a formal asset.
- Do not edit templates in place to store completed work; create a new asset file instead.

## Logs and Session Continuity Rules

- Operational logs and daily session activity belong under `logs/` — primarily `logs/daily/`.
- Use date-oriented filenames where practical (e.g. `YYYY-MM-DD.md`).
- Individual `*.log` files under `logs/` are gitignored; markdown logs and README files are tracked.
- Session handoff and session start artifacts begin from `templates/sessions/`.
- **Olympus-specific filled handoffs** belong in `logs/daily/` unless promoted to a governed asset under `docs/`.
- **Project-specific handoffs** belong in the relevant project repository — do not centralize all project handoffs in Olympus unless a future participating-repository standard says otherwise.
- Promote durable decisions to `docs/decisions/`; durable lessons or standards to appropriate `docs/` folders.
- Logs are continuity aids, not substitutes for governed Knowledge Assets.

## Cursor Rules

- Repository-specific AI behavior guidance belongs in `.cursor/rules/` (`.mdc` files).
- Cursor rules should align with governed documents — not invent finalized governance decisions.
- Rules may reference `docs/` assets by path; update references when assets move.
- Do not store secrets, credentials, or environment values in `.cursor/` configuration.

## Prohibited Practices

- Storing active formal Knowledge Assets in the repository root
- Treating exploratory concept records (e.g. ACR-001, ACR-002) as implementation authority
- Creating application code, package manifests, database schemas, or UI artifacts in this repository during the foundation phase
- Duplicating the same knowledge across multiple documents without canonical-source reference
- Embedding secrets, credentials, or `.env` values in any tracked file
- Silently resolving conflicts between assets — flag them instead
- Creating paperwork that does not help a future human or agent make a better decision
- Assuming external redistribution rights contrary to `LICENSE`

## Review / Maintenance

| Activity | Owner | Cadence |
|---|---|---|
| Standard review | John S. Villasenor | As Needed |
| Directory README accuracy | Asset contributors | On substantive change |
| Cursor rule alignment | Knowledge Stewardship / Governance | When assets move or mature |
| Template freshness | Governance | When asset model changes |

During foundation setup, review this standard when repository structure or placement rules change materially.

## Exceptions

Exceptions require explicit Founder approval and should be recorded as a decision or noted in the affected asset's change history.

Temporary exceptions (e.g. seed assets at `docs/` root during migration) should be documented in the relevant directory `README.md` until resolved.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial draft (OLY-GOV-001) |
| 2026-07-05 | John S. Villasenor | Tier 1/2 working answers: full ID convention, filled handoff location |
