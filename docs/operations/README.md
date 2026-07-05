# docs/operations/

Operating models, workflows, and stewardship practices for Mt. Olympus.

## Purpose

Describe how the knowledge ecosystem is maintained, curated, reviewed, and consumed day to day.

## What belongs here

- Curator and stewardship role definitions
- Review cadences and maintenance workflows
- Agent operating models and consumption patterns
- Handoff and continuity process guidance (as governed assets)

## What does not belong here

- Raw session logs (use `logs/daily/`)
- Governance authority standards (use `docs/governance/`)
- Application deployment or CI/CD documentation
- One-off chat summaries without asset metadata

## Status

Starter directory — proposed organization.

## Current assets (Draft / Advisory)

| Asset | File | Purpose |
|---|---|---|
| Agent Operating Model | `OPM-001_OLYMPUS_AGENT_OPERATING_MODEL.md` | Draft / Advisory operating model for John / Hermes / Hephaestus coordination |
| Knowledge Capture Workflow | `OPM-002_KNOWLEDGE_CAPTURE_WORKFLOW.md` | Draft / Advisory workflow for triaging and routing captured knowledge |
| Agent Roles (short reference) | `AGENT_ROLES.md` | Quick role-name reference — supporting note, not the full operating model |
| Session Start Prompt | `session_start_prompt.md` | Paste-ready Cursor session opening |
| Session Handoff Prompt | `session_handoff_prompt.md` | Paste-ready Cursor session closing |

**OPM-001** and **OPM-002** are Draft / Advisory — not Approved, Canonical, or Governing.

**AGENT_ROLES.md** is a supporting short reference. Use **OPM-001** for full role boundaries, routing, and authority rules.

Session prompts are operating prompts, not approved Knowledge Assets. See OLY-GOV-004 and `.cursor/rules/session-continuity.mdc`.
