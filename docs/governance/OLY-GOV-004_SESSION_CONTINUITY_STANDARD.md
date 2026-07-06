# Session Continuity Standard

> **Status:** Draft — advisory guidance, not approved or governing policy.

## Metadata

| Field | Value |
|---|---|
| Standard ID | OLY-GOV-004 |
| Title | Session Continuity Standard |
| Status | Draft |
| Authority Level | Advisory |
| Owner | John S. Villasenor |
| Created On | 2026-07-05 |
| Last Updated | 2026-07-05 |
| Review Cadence | As Needed |
| Related Assets | Foundation Brief; Knowledge Asset Model; Governance Starter; Repository Standard; Knowledge Asset Standard; Decision Record Standard; ACR-001; ACR-002; Session Start Template; Session Handoff Template |

---

## Purpose

Session continuity preserves **working context across AI-assisted sessions** so future humans and agents can resume work safely and quickly.

Mt. Olympus exists partly because AI-assisted work suffers when:

- New sessions lack prior reasoning
- Agents rediscover old decisions
- Implementation work reopens strategy unnecessarily
- Lessons learned disappear into chat history

Session continuity should help future readers understand:

- **What happened**
- **What changed**
- **What was decided** (vs. what was merely discussed)
- **What remains open**
- **What evidence exists**
- **What risks or limitations matter**
- **What should happen next**

Continuity is a **governed practice**, not a transcript dump.

## Scope

Applies to **session artifacts** in the Olympus repository and any future participating project that **explicitly adopts** this standard.

**In scope:**

- Session starts and session handoffs
- Daily logs and evidence packets
- Continuity artifacts and session-generated candidate knowledge
- Decision and experience capture during sessions

**Out of scope:**

- Application implementation, database schemas, or automation pipelines
- Mandatory adoption by external project repositories
- Replacement of project-specific governance where it exists

## Definition of Session Continuity

**Session continuity** is:

```text
The governed practice of preserving enough context, evidence, decisions, open questions, and next steps for a future human or AI agent to safely resume work without rediscovering or reinventing prior reasoning.
```

**Clarifications:**

- Continuity is **not** a raw chat or transcript dump.
- Continuity is **not** a substitute for formal Knowledge Assets or Decision Records.
- Continuity artifacts may **generate candidate** Knowledge Assets, decisions, or lessons for promotion when they have durable value.

## Session Artifact Types

| Artifact Type | Purpose | Typical Location |
|---|---|---|
| **Session Start** | Orients an agent at the beginning of work | `templates/sessions/SESSION_START_TEMPLATE.md`; filled copies in `logs/daily/` |
| **Session Handoff** | Preserves end-of-session state and next actions | `templates/sessions/SESSION_HANDOFF_TEMPLATE.md`; Olympus filled handoffs in `logs/daily/` |
| **Daily Log** | Chronological operational record | `logs/daily/YYYY-MM-DD.md` |
| **Evidence Packet** | Structured proof of what changed and how it was validated | **Section within session handoff** (no standalone template yet) |
| **Candidate Knowledge Asset** | Session-generated knowledge that may deserve promotion | Captured in handoff or daily log; promoted to appropriate `docs/` folder |
| **Candidate Decision** | Open question or proposed decision discovered during work | `docs/decisions/MT_OLYMPUS_DECISION_BACKLOG.md` or formal decision record in `docs/decisions/` |

Templates under `templates/sessions/` are **starters** — copy before use; do not treat templates as governed artifacts.

## Session Start Rules

A session start should include:

- Date
- Agent name / role
- Project or workstream
- Required reading
- Current repository state
- Active objective
- Constraints
- Open questions
- First actions
- Explicit **Do Not Do** items

**Rules:**

- Agents **must read required source documents** before changing files.
- Agents **must identify** whether work is exploratory, draft, proposed, or approved.
- Agents **must respect** Founder direction and current governance standards (OLY-GOV-001 through OLY-GOV-004 as applicable).
- Agents **must not assume** exploratory concepts (e.g. ACR-001, ACR-002) are implementation authority.
- Agents **should state uncertainty** when source authority or status is unclear.

Use `templates/sessions/SESSION_START_TEMPLATE.md` as the starting structure.

## Session Handoff Rules

A session handoff should include:

- Session date
- Agent / role
- Repository state (branch, commit, uncommitted work)
- Work completed
- Decisions made (with status — not all are Approved)
- Files changed
- Commands run
- Validation / evidence
- Open questions
- Risks / watch items
- Recommended next steps
- Commit / PR status if applicable

**Rules:**

- Handoffs **must distinguish decisions from observations**.
- Handoffs **must identify uncommitted work** clearly.
- Handoffs **must not claim validation** that was not performed.
- Handoffs **should preserve limitations and failed attempts** — failures are continuity value.
- Handoffs **should flag** candidate Knowledge Assets and candidate decisions for promotion review.

Use `templates/sessions/SESSION_HANDOFF_TEMPLATE.md` as the starting structure.

## Daily Log Rules

- Daily logs belong under **`logs/daily/`**.
- Use **`YYYY-MM-DD.md`** naming when practical.
- Daily logs are **chronological continuity aids** — lightweight, scannable, date-oriented.
- Daily logs are **not automatically** formal Knowledge Assets.
- Durable lessons, decisions, or standards discovered in logs should be **promoted** to proper `docs/` assets.
- Logs should remain **concise enough to be useful** — avoid bloated narrative nobody will read.
- Individual `*.log` files under `logs/` are gitignored; markdown daily logs are tracked.

**Daily log AI Consumption (working guidance):**

| Artifact | AI Consumption when resuming |
|---|---|
| Latest session handoff | **Required** when resuming the same workstream |
| Daily logs | **Recommended** when a handoff exists |
| Daily logs (no handoff) | **Required** — relevant daily logs become primary continuity source |
| Formal decisions & governance standards | Outrank logs and handoffs for authority |

## Evidence Packet Rules

Evidence packets document **what changed and how it was validated**. For now they remain a **section within session handoffs** — do not create a standalone evidence packet template until repeated workflows require it.

**Should include when applicable:**

- Branch / repository state
- Files changed
- Commands run
- Test results
- Validation performed
- Known limitations
- Artifacts produced
- Screenshots or QA notes when available
- Commit / PR references

**Rules:**

- **Do not invent evidence.**
- **Do not claim tests passed** unless actually run.
- If validation was **not possible**, state **why**.
- If an agent **lacks a capability** (e.g. browser QA, screenshot capture), the evidence packet **must say so** and provide **clear human QA instructions** instead.
- Evidence packets should be **proportional** to the work — a README edit does not need a full QA matrix.

**Specific note:** If an agent cannot perform screenshots or direct product/browser QA, evidence packets **must not require agent-created screenshots**. They may include exported files, command output, or explicit QA steps for the Founder to execute.

## Decision Capture Rules

- **Not every session observation is a decision.**
- Decisions **discovered during a session** should be added to the **decision backlog** (`docs/decisions/MT_OLYMPUS_DECISION_BACKLOG.md`) unless explicitly approved in the same session.
- **Approved durable decisions** should become Decision Records under `docs/decisions/` per `OLY-GOV-003_DECISION_RECORD_STANDARD.md` (OLY-GOV-003).
- **Founder approval must be explicit** for **Approved** status — only Founder may approve (Curator and agents may recommend, not approve).
- Session handoffs **may mention** decisions, but the **formal decision source** for durable guidance is a decision record, not the handoff alone.

## Experience Capture Rules

Drawing on exploratory concepts in ACR-002 — **not approved architecture**:

Sessions often reveal experience through **surprises, failures, tradeoffs, warnings, and patterns**.

**Handoffs should flag** candidate experience worth preserving.

When capturing experience (in handoff, log, or promoted asset), include:

- **What happened**
- **Why it mattered**
- **What was learned**
- **How future agents should use it**
- **Related assets or projects**
- **Confidence level** if relevant (exploratory framing)

**Rules:**

- **Not every experience note** becomes a Knowledge Asset.
- **Durable experience** should be promoted to `docs/lessons/`, `docs/operations/`, or another relevant `docs/` folder per `OLY-GOV-002_KNOWLEDGE_ASSET_STANDARD.md` (OLY-GOV-002).
- Do **not** implement `experience_events` schema or application capture pipelines in this pass.

## Agent Capability and Limitation Rules

- Agents **must not claim capabilities they do not have**.
- Agents **must distinguish** inspection, recommendation, implementation, validation, and human QA.
- Agents **should state tool/environment limitations** when they affect evidence or continuity claims.
- If an agent **cannot perform** requested validation, it **must provide clear human validation instructions**.
- **Capability limits** that affect repeatable workflows should be captured in handoff or operating guidance when they matter for the next session.

**Examples of limitations to disclose:**

- Cannot run browser or visual QA
- Cannot access external services without credentials
- Cannot push to remote without explicit instruction
- Sandbox or environment constraints affecting test execution

## Source Reading Rules

- **Required reading** should be explicit in session start prompts or handoff next steps.
- Agents should **prefer** governing, canonical, and approved assets over exploratory context.
- Agents **must check status and authority** before relying on a source document.
- Agents **should cite or reference** source assets when making recommendations.
- If sources **conflict**, agents **must flag the conflict** — do not silently resolve.

**Suggested required reading for Olympus foundation work:**

- Root `README.md`
- `docs/foundation/MT_OLYMPUS_PROJECT_INSTRUCTIONS.md`
- Relevant OLY-GOV standards for the workstream
- Active concept records only when explicitly in scope

## Resume Rules

A future session should be able to resume from:

- Latest **session handoff** (if any)
- Relevant **daily log** (`logs/daily/`)
- Current **git state** (branch, status, recent commits)
- **Decision backlog** and any approved decision records
- Relevant **governance standards**
- Stated **active workstream objective**

**Rules for resuming:**

- **Verify** whether prior work was committed or pushed — do not assume.
- **Do not assume** uncommitted work exists unless shown in handoff or git status.
- **Confirm** current branch and repository status before editing when applicable.
- Treat handoff claims as **continuity hints** — verify against repository state and formal assets.
- **Formal decisions and governance standards outrank** handoffs and daily logs.

## Promotion Rules

Continuity artifacts may produce:

- Knowledge Assets
- Decision Records
- Lessons Learned
- Governance standard updates
- Product or architecture definitions (when appropriate and approved)

**Rules:**

- **Promote only** when **future decision value** exists.
- **Do not promote** raw logs wholesale.
- **Preserve links** from promoted assets back to session source (handoff date, log path) when useful.
- **Update** related README files, backlog items, and Related Assets when promotion occurs.
- Follow promotion paths in `OLY-GOV-002_KNOWLEDGE_ASSET_STANDARD.md` and `OLY-GOV-003_DECISION_RECORD_STANDARD.md`.

## Placement and Naming Rules

Align with `OLY-GOV-001_REPOSITORY_STANDARD.md` (OLY-GOV-001):

| Content | Location |
|---|---|
| Session templates | `templates/sessions/` |
| Filled Olympus handoffs | `logs/daily/` (unless promoted to `docs/`) |
| Project-specific handoffs | Relevant **project repository** — not centralized in Olympus by default |
| Daily logs | `logs/daily/` (`YYYY-MM-DD.md`) |
| Durable operating models | `docs/operations/` |
| Decision records | `docs/decisions/` |
| Lessons learned | `docs/lessons/` |
| Governance standards | `docs/governance/` |
| Formal Knowledge Assets | Appropriate `docs/` subdirectory |

- Use **date-oriented names** for logs.
- Use **stable IDs** for formal Knowledge Assets and decision records.
- Filled session starts and handoffs for **Olympus work** belong in `logs/daily/` unless promoted.
- Durable cross-project lessons or standards discovered in handoffs should be promoted into Olympus `docs/`.

## AI Consumption Rules

AI agents **must**:

- **Read session continuity artifacts** when resuming work in the same workstream
- **Distinguish handoff claims** from formal decisions and approved standards
- **Verify current repository state** before acting on old handoffs
- **Cite formal sources** when recommendations depend on governed content
- **Identify candidate knowledge** from sessions worth promotion review
- **Respect status and authority metadata** on all source documents
- **Avoid re-litigating settled decisions** unless new evidence or Founder direction requires it

**Continuity artifact consumption priority when resuming:**

1. Relevant **governance standards** and **approved decision records**
2. Latest **session handoff** for the workstream (**Required** AI Consumption)
3. Relevant **daily logs** (**Recommended** if handoff exists; **Required** if no handoff)
4. Current **git state**

**AI Consumption values** (when assigned to continuity-related assets):

| Value | Meaning |
|---|---|
| **Required** | Agents should read when resuming related work. |
| **Recommended** | Agents should consult when relevant. |
| **Optional** | Agents may consult for additional context. |
| **Restricted** | Agents must not rely on without explicit permission. |

## Prohibited Practices

- Dumping **raw transcripts** as continuity
- Treating **handoffs as approved decisions**
- **Hiding failed attempts** or limitations
- **Omitting uncommitted work** state
- **Claiming tests or validation** not performed
- Creating **bloated logs** nobody will use
- **Requiring evidence** an agent cannot produce (e.g. mandatory agent screenshots when tooling does not support it)
- **Silently resolving conflicts** between handoff claims and formal assets
- **Replacing formal decisions** with chat or handoff summaries
- **Turning every note** into a formal Knowledge Asset
- Promoting exploratory session ideas to **Approved** without Founder approval

## Exceptions

- Exceptions require **Founder approval** only.
- Document exceptions in the affected handoff, daily log, or governance standard Change History.

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-07-05 | John S. Villasenor | Initial draft (OLY-GOV-004) |
| 2026-07-05 | John S. Villasenor | Tier 1/2 working answers: handoff location, daily log AI Consumption, evidence packet as handoff section |
