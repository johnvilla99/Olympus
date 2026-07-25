# docs/operations/

Operating models, workflows, roadmaps, and stewardship practices for Olympus.

## Purpose

Describe how the knowledge ecosystem is maintained, curated, reviewed, sequenced, and consumed day to day.

## What belongs here

- Stewardship role definitions
- Review cadences and maintenance workflows
- Agent operating models and consumption patterns
- Phase-gated operating roadmaps
- Handoff and continuity process guidance when preserved as governed assets

## What does not belong here

- Raw session logs, which belong in `logs/daily/`
- Governance authority standards, which belong in `docs/governance/`
- Product requirements, which belong in a future `docs/product/` area when product definition begins
- Architecture definitions, which belong in a future `docs/architecture/` area when architecture work begins
- Application deployment or CI/CD documentation
- One-off chat summaries without asset metadata

## Current Status

The core operating models are **Approved / Advisory**. They are accepted for current Olympus use but are not Canonical or Governing.

Operating models apply governance rules; they do not redefine them. In particular, OLY-GOV-003 owns decision authority and hierarchy.

## Current Assets

| Asset | File | Status / Authority | Purpose |
|---|---|---|---|
| Agent Operating Model | `OPM-001_OLYMPUS_AGENT_OPERATING_MODEL.md` | Approved / Advisory | John, Hermes, Hephaestus, Eunomia, Muse, routing, and escalation boundaries |
| Knowledge Capture Workflow | `OPM-002_KNOWLEDGE_CAPTURE_WORKFLOW.md` | Approved / Advisory | Triage, capture, routing, and promotion-candidate handling |
| Decision Promotion / Approval Workflow | `OPM-003_DECISION_PROMOTION_APPROVAL_WORKFLOW.md` | Approved / Advisory | Operational path from backlog or working answer to formal decision |
| Product-to-Architecture Roadmap | `OPM-004_OLYMPUS_PRODUCT_TO_ARCHITECTURE_ROADMAP.md` | Approved / Advisory; AI Consumption Required | Phase-gated path from foundation closure through product definition, application governance, Architect agent creation, architecture discovery, validation, and proposed technical stack |
| Agent Roles | `AGENT_ROLES.md` | Supporting reference | Quick role-name reference; OPM-001 remains the full operating model |
| Session Start Prompt | `session_start_prompt.md` | Operating prompt | Session opening and required-reading workflow |
| Session Handoff Prompt | `session_handoff_prompt.md` | Operating prompt | Session closing and continuity capture |

Session prompts are operating aids, not formal Knowledge Assets. Apply OLY-GOV-004 for continuity and OLY-GOV-005 for discovery.

## Current Roadmap Position

Olympus is presently in **Phase 1: Foundation Closure** under OPM-004.

Product discovery, Architect agent construction, architecture selection, and technical-stack selection must not begin until the applicable phase gates are approved by John.
