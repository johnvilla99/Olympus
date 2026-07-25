# docs/governance/

Authority, maturity, and process standards for the Mt. Olympus ecosystem.

## Purpose

Define how knowledge becomes trustworthy, how assets mature, and who has authority over what.

## What belongs here

- Governance charters and standards
- Authority and maturity models
- Documentation and asset lifecycle rules
- Review cadence and stewardship definitions

## What does not belong here

- Individual decisions, which belong in `docs/decisions/`
- Exploratory concepts, which belong in `docs/concepts/`
- Application or infrastructure standards for other repositories
- Binding policy without the appropriate Status and Authority Level

## Current Status

The core OLY-GOV suite is **Approved / Advisory**. These standards are accepted for current Olympus use but are not Canonical or Governing unless explicitly stated.

OLY-GOV-003 owns decision authority, hierarchy, approval, and conflict treatment. Supporting artifacts should reference it rather than restating its hierarchy.

## Current Assets

| Asset | File | Status / Authority | Purpose |
|---|---|---|---|
| Governance Starter | `OLYMPUS_GOVERNANCE_STARTER.md` | Seed reference | Early authority and maturity framing; defer to approved standards where they differ |
| Repository Standard | `OLY-GOV-001_REPOSITORY_STANDARD.md` | Approved / Advisory | Repository layout, placement, and naming references |
| Knowledge Asset Standard | `OLY-GOV-002_KNOWLEDGE_ASSET_STANDARD.md` | Approved / Advisory | Metadata, categories, lifecycle, promotion, and AI Consumption |
| Decision Record Standard | `OLY-GOV-003_DECISION_RECORD_STANDARD.md` | Approved / Advisory | Decision authority, hierarchy, lifecycle, approval, and backlog discipline |
| Session Continuity Standard | `OLY-GOV-004_SESSION_CONTINUITY_STANDARD.md` | Approved / Advisory | Session starts, handoffs, logs, evidence, and resume behavior |
| Agent Knowledge Discovery Standard | `OLY-GOV-005_AGENT_KNOWLEDGE_DISCOVERY_STANDARD.md` | Approved / Advisory | Authority-aware discovery, citation, synthesis, conflict handling, and safe consumption |

## Related Canonical Decision

**GDR-001** is the Approved / Canonical source for Olympus identifier prefixes and numbering. Governance standards reference it rather than maintaining separate provisional ID rules.