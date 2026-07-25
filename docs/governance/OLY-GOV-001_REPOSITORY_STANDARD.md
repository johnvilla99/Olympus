# Repository Standard

> **Status:** Approved / Governing. This standard controls Olympus repository structure, placement, and maintenance rules.

## Metadata

| Field | Value |
|---|---|
| Standard ID | OLY-GOV-001 |
| Title | Repository Standard |
| Status | Approved |
| Authority Level | Governing |
| Owner | John S. Villasenor |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-25 |
| Review Cadence | As Needed |
| Related Assets | Foundation Brief; Knowledge Asset Model; Governance Starter; GDR-001; ACR-001; ACR-002 |

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
- Participating project repositories unless they adopt this standard by explicit decision
- Promotion of other assets to Approved, Canonical, or Governing status

## Repository Structure

```text
Olympus/
├── README.md
├── LICENSE
├── .gitignore
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
│   ├── knowledge-assets/
│   ├── decisions/
│   ├── sessions/
│   └── governance/
├── logs/
│   └── daily/
└── .cursor/
    └── rules/
```

## Directory Responsibilities

| Path | Role |
|---|---|
| `docs/foundation/` | Ecosystem purpose, scope, conceptual model, project instructions |
| `docs/governance/` | Authority, maturity, and process standards |
| `docs/concepts/` | Exploratory concept records |
| `docs/decisions/` | Decision records and decision backlog |
| `docs/muses/` | Muse catalog and domain definitions |
| `docs/operations/` | Operating models, workflows, stewardship |
| `docs/research/` | Research notes and evidence; Research is cross-cutting, not a Muse |
| `docs/lessons/` | Lessons learned and retrospective knowledge |
| `docs/projects/` | Cross-project participation and ecosystem context |
| `templates/` | Blank starter templates |
| `logs/daily/` | Date-oriented operational and session activity logs |
| `.cursor/rules/` | Persistent AI-agent instructions for this repository |

Each directory should include a `README.md` explaining purpose, what belongs, and what does not.

## File Naming Rules

- Use **UPPER_SNAKE_CASE** for formal Knowledge Asset filenames.
- Use the Approved / Canonical identifier convention defined by **GDR-001**.
- Prefer descriptive suffixes over opaque abbreviations.
- Do not rename assets casually; record supersession when replacing an asset.
- `README.md` is reserved for directory index files.

## Knowledge Asset Placement Rules

- Formal Knowledge Assets belong under the appropriate `docs/` subdirectory, not at repository root.
- Concept records belong in `docs/concepts/`.
- Governance standards belong in `docs/governance/`.
- Decision records and backlog belong in `docs/decisions/`.
- Research notes belong in `docs/research/`.
- Lessons learned belong in `docs/lessons/`.
- Every formal Knowledge Asset should include metadata consistent with OLY-GOV-002.
- Check Status and Authority Level before relying on content.
- Do not promote assets without explicit Founder approval.

## Source Document Rules

- Root `README.md` is the front door, not the full knowledge base.
- `LICENSE` remains proprietary unless the Founder explicitly changes it.
- Prefer linking to authoritative sources over duplicating content.
- When duplication is necessary, identify the authoritative source.
- Founder direction outranks repository documents within the Founder’s authority.

## Template Rules

- Templates are starters, not governed assets.
- Copy a template into the correct `docs/` directory before filling it in.
- Assign an ID under GDR-001 and complete metadata.
- Do not edit templates in place to store completed work.

## Logs and Session Continuity Rules

- Operational logs and daily activity belong under `logs/`, primarily `logs/daily/`.
- Use date-oriented filenames where practical.
- Olympus filled handoffs belong in `logs/daily/` unless promoted.
- Project-specific handoffs belong in the relevant project repository by default.
- Logs are continuity aids, not substitutes for governed Knowledge Assets.

## Cursor Rules

- Repository-specific AI guidance belongs in `.cursor/rules/`.
- Cursor rules must reference and align with governed documents rather than redefine them.
- Do not store secrets or environment values in `.cursor/` configuration.

## Prohibited Practices

- Storing active formal Knowledge Assets at repository root
- Treating exploratory ACRs as implementation authority
- Creating application code or technical implementation artifacts during foundation-only work
- Duplicating authoritative rules without identifying the owning source
- Embedding secrets or credentials
- Silently resolving asset conflicts
- Creating paperwork without future decision value
- Assuming redistribution rights contrary to `LICENSE`

## Review / Maintenance

| Activity | Owner | Cadence |
|---|---|---|
| Standard review | John S. Villasenor | As Needed |
| Directory README accuracy | Asset contributors | On substantive change |
| Cursor rule alignment | Knowledge Stewardship / Governance | When assets move or mature |
| Template freshness | Governance | When asset model changes |

## Exceptions

Exceptions require explicit Founder approval and should be recorded in the affected asset or an appropriate decision record.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial draft |
| 2026-07-25 | John S. Villasenor | Approved as current Advisory guidance; aligned naming authority to GDR-001 and Research placement to the cross-cutting model |
| 2026-07-25 | John S. Villasenor | Promoted to Governing authority as the controlling repository structure and placement standard |