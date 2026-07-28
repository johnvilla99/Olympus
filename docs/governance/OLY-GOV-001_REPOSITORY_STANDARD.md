# Repository Standard

> **Status:** Approved / Governing. This standard controls Olympus repository structure, placement, and maintenance rules.

## Metadata

| Field | Value |
|---|---|
| Standard ID | OLY-GOV-001 |
| Title | Repository Standard |
| Status | Approved |
| Authority Level | Governing |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-27 |
| Review Cadence | As Needed |
| Related Assets | GDR-001; GDR-005; GDR-006; GDR-007; GDR-008; OLY-GOV-002; OPM-004 |
| AI Consumption | Required |
| Change Impact | High |

---

## Purpose

Define how the Olympus repository is organized, maintained, and consumed so humans and AI agents can locate authoritative knowledge safely.

The active durable repository is governed by **GDR-007**. The official ecosystem name is governed by GDR-002; GDR-008 permits “Mt. Olympus” as a display alias.

## Scope

**In scope:** directory layout, file placement, naming, templates, logs, indexes, and Cursor rules.

**Out of scope:** application implementation, databases, APIs, UI design, participating-project adoption, and authority definitions owned by GDR-005 and GDR-006.

## Repository Structure

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
│   ├── operations/
│   ├── research/
│   ├── lessons/
│   └── projects/
├── templates/
├── logs/daily/
└── .cursor/rules/
```

## Directory Responsibilities

| Path | Role |
|---|---|
| `docs/foundation/` | Ecosystem purpose, scope, models, and project instructions |
| `docs/governance/` | Governing standards and authority procedures |
| `docs/concepts/` | Exploratory concept records |
| `docs/decisions/` | Decision records and Decision Backlog |
| `docs/muses/` | Muse/domain definitions |
| `docs/operations/` | Operating models, workflows, and durable handoffs |
| `docs/research/` | Research notes and evidence |
| `docs/lessons/` | Lessons learned and retrospective knowledge |
| `docs/projects/` | Cross-project participation and context |
| `templates/` | Blank starters, not completed assets |
| `logs/daily/` | Date-oriented continuity artifacts |
| `.cursor/rules/` | Persistent repository-agent guidance |

Each governed directory should maintain an index describing what belongs and what does not.

## Naming and Identifiers

- Use UPPER_SNAKE_CASE for formal Knowledge Asset filenames.
- Use identifiers and numbering defined by **GDR-001**; do not reproduce the prefix catalog here.
- Do not reuse retired or superseded IDs.
- Do not rename formal assets casually; use supersession where appropriate.
- Reserve `README.md` for navigation and orientation.

## Placement Rules

- Formal Knowledge Assets belong under the appropriate `docs/` directory.
- Templates remain under `templates/` and are copied before use.
- Operational logs remain under `logs/` until promoted.
- Directory READMEs are navigation aids, not automatically Canonical assets.
- Historical handoffs and concept records are not modernized merely because terminology changes.

## Source and Authority Rules

- Use **GDR-007** for the active repository location.
- Use **GDR-005** for metadata semantics.
- Use **GDR-006** for authority resolution.
- Root README is the repository front door, not the source of truth for every topic.
- Prefer references to controlling assets over synchronized copies.
- `LICENSE` remains the repository-usage authority.

## Template Rules

Templates are starters, not governed completed assets. Copy a template, assign an ID, set honest metadata, and place the completed artifact in the proper governed directory.

## Logs and Continuity

- Olympus daily logs and filled handoffs normally belong in `logs/daily/`.
- Project-specific handoffs remain in the relevant project repository unless an explicit standard says otherwise.
- Durable decisions, lessons, or operating guidance should be promoted to the appropriate `docs/` location.
- Logs do not replace formal authority.

## Cursor Rules

Repository-specific AI guidance belongs in `.cursor/rules/`. Rules must reference controlling decisions and standards rather than invent or duplicate authority. Do not place secrets in Cursor configuration.

## Prohibited Practices

- Storing active formal assets at repository root
- Treating exploratory concepts as implementation authority
- Creating later-phase application or architecture artifacts before OPM-004 permits them
- Duplicating authoritative rules without a controlling-source reference
- Embedding secrets or environment values
- Silently resolving conflicts
- Treating commit or push as approval
- Rewriting historical records solely to modernize terminology

## Exceptions

Exception authority and approval follow GDR-006 and OPM-003. Record approved exceptions in the affected asset or a decision record.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial repository standard. |
| 2026-07-25 | John S. Villasenor | Approved as Governing repository guidance. |
| 2026-07-27 | Hermes under explicit Founder direction | Aligned repository identity, active location, metadata, and authority references to GDR-005 through GDR-008. |
