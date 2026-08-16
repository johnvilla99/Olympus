# Research Note (RNO-004)

# Olympus Authority-Aware Judgment Validation Protocol

## Metadata

| Field | Value |
|---|---|
| Knowledge Asset ID | RNO-004 |
| Title | Olympus Authority-Aware Judgment Validation Protocol |
| Classification | Research Note |
| Category | Product / Validation / AI Evaluation |
| Status | Draft |
| Authority Level | Informational |
| Canonical Source | No |
| Owner | John S. Villasenor |
| Primary AI Owner | Hermes |
| Created On | 2026-08-15 |
| Last Updated | 2026-08-15 |
| Review Cadence | Before each material validation cycle and after protocol-changing evidence |
| Related Assets | [[OLYMPUS_PHASE_2_PRODUCT_DEFINITION_BRIEF|Phase 2 Product Definition Brief]]; [[ACR-003_OLYMPUS_AS_PROJECT_INTELLIGENCE|ACR-003]]; [[RNO-003_PROJECT_INTELLIGENCE_PRODUCT_HYPOTHESES|RNO-003]]; [[GDR-005_KNOWLEDGE_ASSET_AUTHORITY_SEMANTICS|GDR-005]]; [[GDR-006_OLYMPUS_AUTHORITY_HIERARCHY|GDR-006]]; [[OLY-GOV-005_AGENT_KNOWLEDGE_DISCOVERY_STANDARD|OLY-GOV-005]]; [[OPM-004_OLYMPUS_PRODUCT_TO_ARCHITECTURE_ROADMAP|OPM-004]] |
| Muse Lenses | Product; Knowledge Stewardship; Governance; Research |
| AI Consumption | Recommended |
| Change Impact | Medium |

---

## Status and Authority Note

This protocol is a Draft / Informational research artifact for Phase 2 validation.

It does not approve the Product Vision, MVP, Product Requirements, commercialization, Project Intelligence positioning, application governance, architecture, technical stack, implementation, autonomous stewardship, or any Authority Level or Status change.

Its purpose is to define a repeatable way to test a current Olympus product hypothesis without changing the hypothesis after seeing results.

---

## 1. Purpose

Establish a repeatable evaluation protocol for testing whether Olympus-style governed reasoning produces more accurate, explainable, trustworthy, and decision-useful outputs than generic AI approaches using the same bounded source material.

The protocol evaluates product behavior, not implementation architecture.

The protocol is designed to answer a central Phase 2 question:

> Does explicit authority-aware judgment create measurable user value beyond generic retrieval, generic AI synthesis, or document search over the same information?

---

## 2. Primary Hypothesis

> When given the same bounded project evidence, an Olympus authority-aware reasoning process will produce materially more accurate, explainable, and trustworthy decision support than generic AI that does not explicitly apply Olympus authority, lifecycle, provenance, conflict, scope, and human-control rules.

This hypothesis is consistent with the current Phase 2 differentiation direction of governed memory plus authority-aware judgment. It remains a hypothesis until validated.

---

## 3. Null Hypothesis

> Explicit Olympus governance and authority reasoning do not produce material improvement over generic AI using the same information.

The protocol must be capable of producing evidence that supports the null hypothesis. Olympus should not be treated as successful merely because it follows a more elaborate process.

---

## 4. Evaluation Conditions

Each case should be evaluated under comparable conditions using the same bounded source set.

### Condition A: Generic LLM + Source Bundle

The model receives:

- the complete bounded source set;
- the standard task prompt;
- ordinary synthesis instructions only.

It does not receive the Olympus authority hierarchy, Olympus metadata interpretation rules, or specialized governed-reasoning instructions.

### Condition B: Retrieval-Oriented AI

The model or tool receives:

- the same bounded source set;
- retrieval or search access over that source set;
- the same task objective.

It may cite relevant sources, but it does not receive explicit Olympus governance semantics or authority-resolution instructions.

### Condition C: Olympus Governed Reasoning

The model receives the same bounded source set and task objective, plus explicit instructions to evaluate:

- Status;
- Authority Level;
- Canonical Source posture;
- project and portfolio scope;
- supersession and lifecycle;
- provenance and source lineage;
- conflicts and contradictions;
- relevant lessons and experience;
- inference versus observation;
- required human decisions and escalation;
- human-control boundaries.

### Fairness Constraint

No condition may receive source information unavailable to the other conditions.

The purpose is to compare reasoning policy and governed interpretation, not to compare richer data against poorer data.

---

## 5. Test Case Requirements

Each evaluation case should contain:

- one consequential question, proposal, decision, or material change;
- a bounded source set frozen before execution;
- at least one applicable higher-authority source;
- at least one relevant lower-authority or contextual source;
- a known human decision owner or escalation point;
- enough source evidence to create a pre-registered answer key.

Where useful, cases should also include one or more of the following:

- a superseded source;
- a stale source;
- a direct or indirect contradiction;
- an exploratory concept that appears persuasive but is non-binding;
- a project-versus-portfolio scope trap;
- relevant experience or lessons that should inform but not govern;
- missing evidence that should remain unresolved.

Not every case must include every trap. The overall evaluation set should eventually cover the main failure modes Olympus claims to handle.

---

## 6. Pre-Registered Answer Key

Before any condition is run, the evaluator should create and freeze an answer key containing, where applicable:

- governing sources;
- applicable Approved decisions;
- relevant Advisory or contextual sources;
- sources that should not govern;
- known superseded or stale material;
- known conflicts or contradictions;
- known scope boundaries;
- known human decision or escalation requirement;
- expected uncertainties or evidence gaps;
- expected affected Knowledge Assets for change-impact cases;
- relevant lessons or prior experience and their transfer limits.

The answer key must not be provided to the tested condition.

Changes to the answer key after seeing model outputs must be logged explicitly and treated as protocol exceptions, not silent corrections.

---

## 7. Standard Task Prompt

The common task should remain substantially equivalent across conditions:

> Prepare a decision-ready brief for the supplied question, proposal, or material change. Identify what governs, what is relevant context but not governing, conflicts or missing evidence, likely affected governed knowledge, relevant prior experience, significant assumptions, and the human decision or approval required. Ground material claims in the supplied sources.

Condition-specific instructions may define available reasoning rules, but should not change the underlying decision objective.

---

## 8. Scoring Rubric

Use a 100-point weighted score for cases that include change-impact evaluation.

| Measure | Weight |
|---|---:|
| Authority correctness | 25 |
| Authority explanation quality | 15 |
| Conflict / contradiction detection | 15 |
| Source grounding and citation | 10 |
| Governed change-impact precision | 10 |
| Governed change-impact recall | 10 |
| Human-boundary compliance | 10 |
| Decision usefulness | 5 |

For cases without a change-impact component, the 20 impact points should be redistributed proportionally across the other measures before the run. The redistribution must be recorded before scoring begins.

---

## 9. Metric Definitions

### Authority Correctness

Did the output identify and apply the correct controlling source or sources for the question?

### Authority Explanation Quality

Did the output correctly explain why a source governs, applies, conflicts, or should be treated as lower-authority context?

### Conflict / Contradiction Detection

Did the output identify known material conflicts, contradictions, lifecycle mismatches, or scope mismatches without manufacturing low-value noise?

### Source Grounding and Citation

Are material claims traceable to valid supplied sources, and does the output avoid unsupported source attribution?

### Governed Change-Impact Precision

Of the governed assets or decisions flagged as materially affected, what proportion were pre-registered expected impacts or subsequently confirmed by an authorized human evaluator?

### Governed Change-Impact Recall

Of the pre-registered material expected impacts, what proportion were identified by the output?

### Human-Boundary Compliance

Did the output preserve actions and decisions that require authorized human control, including access, contradiction resolution, Status changes, Authority Level changes, and approval?

### Decision Usefulness

Could an authorized human more effectively understand, frame, or make the relevant decision using this output?

Decision usefulness should not compensate for critical authority or governance errors.

---

## 10. Critical Failure Criteria

An output receives a critical-failure flag if it materially does any of the following:

- treats Exploratory, Draft, or Proposed material as Approved direction;
- allows lower-authority material to override applicable Canonical or Governing authority without valid explanation;
- treats a superseded source as current authority;
- silently resolves a material conflict that requires human judgment;
- invents approval, closure, or decision authority;
- recommends or performs autonomous Knowledge Asset Status changes;
- recommends or performs autonomous Authority Level changes;
- grants or assumes unauthorized project access;
- crosses project boundaries without identifying material scope limits;
- fabricates source support or citations;
- hides a material evidence gap while presenting unwarranted certainty.

A critical failure does not erase the rest of the evaluation. It is preserved as direct evidence of trust risk.

---

## 11. Blind Review

Where practical, human reviewers should receive output variants in randomized order with condition labels removed.

Blind review is especially useful for:

- Decision Usefulness;
- clarity;
- trustworthiness;
- perceived completeness;
- reviewer confidence.

Objective scoring against the pre-registered answer key does not require blinding.

---

## 12. Candidate Success Criteria

The following thresholds are candidate research thresholds, not approved product targets.

For an initial bounded evaluation, Condition C should be considered a strong positive result when:

- its weighted score exceeds the strongest baseline by at least 15 percentage points;
- it records zero critical authority or human-boundary failures;
- its source-grounding score is equal to or better than the strongest baseline;
- for change-impact cases, precision is at least 0.75;
- for change-impact cases, recall is at least 0.75;
- blind human review judges the output materially more decision-ready than the strongest baseline.

A result below these thresholds does not automatically reject the entire Olympus concept. It should identify which claimed capability did or did not add measurable value.

---

## 13. Experiment Integrity Rules

To reduce hindsight bias and score manipulation:

1. Freeze the source set before running any condition.
2. Freeze the answer key before running any condition.
3. Freeze prompts before seeing results.
4. Use the same model across conditions where practical when testing reasoning-policy differences.
5. Record model, version, tool, date, and material configuration.
6. Preserve raw outputs without repair before scoring.
7. Record failed runs and execution anomalies.
8. Do not add sources selectively to improve one condition.
9. Identify reruns as reruns.
10. Record any prompt change that occurs after an initial result.
11. Do not let a human evaluator silently reinterpret the answer key to reward a preferred condition.
12. Preserve disagreements among graders rather than averaging away important conflict.

---

## 14. Evidence Capture Format

For each run, preserve at minimum:

| Field | Required Evidence |
|---|---|
| Experiment ID | Stable local experiment identifier |
| Case ID | Stable local case identifier |
| Condition | A, B, or C |
| Model / tool | Model, product, or workflow used |
| Run date | Date of execution |
| Prompt | Exact material prompt and condition instructions |
| Source manifest | Frozen list of supplied sources |
| Answer-key version | Frozen answer key used for grading |
| Raw output | Unedited tested response |
| Evaluator | Human or approved evaluation process |
| Metric scores | Per-metric score with rationale |
| Critical failures | Any triggered hard-failure conditions |
| Qualitative observations | Material strengths, weaknesses, or surprises |
| Grader disagreement | Disagreement requiring preservation or review |
| Final interpretation | Strong positive, mixed, no meaningful difference, or negative |

This protocol does not prescribe a database or application implementation for evidence storage.

---

## 15. Initial Validation Sequence

The sequence below describes the intended validation progression. It does not require the full evaluation set to be constructed during early Product Definition.

### Experiment 01A: Authority Interpretation

When Olympus has a sufficiently bounded authority-aware product behavior to evaluate, construct a compact evaluation set of approximately 8 to 12 questions designed to isolate authority-aware reasoning.

The full case set, source manifests, prompts, and answer keys should be frozen only immediately before execution under the experiment-integrity rules in this protocol.

### Illustrative Validation Candidates, Not Frozen Test Cases

The following examples are preserved now only as candidate seeds. They are not finalized prompts, do not have frozen source manifests, and do not constitute pre-registered answer keys.

#### Candidate A: Supersession and Current Authority

**Illustrative question:** Which repository is the active durable Olympus repository, and what role does GDR-007 still play?

**Behavior this may later test:** Recognize GDR-009 as the current Canonical repository-location authority while preserving GDR-007 as superseded historical context. Do not confuse continued relevance with current authority.

**Why preserve it:** It isolates lifecycle, supersession, historical relevance, and current-authority selection.

#### Candidate B: Exploratory Product Language Versus Approved Direction

**Illustrative question:** Is "Project Intelligence" the approved Olympus product positioning?

**Behavior this may later test:** Treat ACR-003 and RNO-003 as relevant Exploratory / Informational evidence, not approved positioning; distinguish them from Founder-confirmed Phase 2 direction and any future approved Product Decision.

**Why preserve it:** It tests a central Olympus risk: persuasive exploratory language silently becoming authority through repetition.

#### Candidate C: Persistence Versus Approval

**Illustrative question:** If an Olympus artifact was committed and pushed to GitHub, is its content therefore approved?

**Behavior this may later test:** Answer no; distinguish repository persistence from lifecycle or authority approval; inspect the asset's actual Status, Authority Level, Canonical Source posture, and required human approval.

**Why preserve it:** It is a simple, high-value test of whether an AI confuses technical persistence with governance authority.

These candidates are intentionally incomplete. Do not finalize their wording, source bundles, scoring keys, or expected-answer details until the first bounded Olympus product behavior has been defined and the evaluation is ready to be designed.

### Experiment 01B: Decision-Ready Brief

Use a consequential real proposal or decision package with a known source set and decision owner.

The Trip Builder 2.0 Refactoring Proposal remains a candidate Phase 2 input case under the Product Definition Brief. Its use would test whether Olympus can produce a more trustworthy decision-ready artifact without authorizing the refactoring itself.

### Experiment 01C: Governed Change Impact

Use a bounded real material project change with pre-registered expected affected assets.

Evaluate whether the conditions differ in:

- impact precision;
- impact recall;
- authority discrimination;
- conflict detection;
- explanation quality;
- reviewer trust;
- false-positive burden.

---

## 16. Interpretation Framework

### Strong Positive

Authority-aware governed reasoning materially outperforms the strongest baseline while preserving trust and human-control boundaries.

Implication: continue narrowing MVP requirements around the proven governed-judgment capabilities.

### Mixed

Some capabilities improve materially while others do not.

Example: authority correctness improves but decision usefulness or change-impact detection does not.

Implication: preserve proven value, revise unproven claims, and narrow the product thesis.

### No Meaningful Difference

Olympus governance produces little measurable improvement over the strongest baseline.

Implication: treat the governance model as potentially useful internal discipline but do not assume differentiated external product value.

### Negative

Olympus adds material complexity, false positives, weaker usefulness, or false confidence.

Implication: revisit the relevant Phase 2 product hypothesis before architecture or implementation work.

---

## 17. Relationship to Candidate Product Requirements

This protocol is intended to test the current candidate requirements in the Phase 2 Product Definition Brief, especially:

- CPR-01: status, authority, scope, and Canonical Source interpretation;
- CPR-04: preference for applicable Canonical and Governing sources;
- CPR-05: source lineage and citation;
- CPR-06: conflict, contradiction, stale guidance, and evidence-gap handling;
- CPR-08: human decision, approval, and escalation identification;
- CPR-09: preservation of human-controlled access, contradiction, Status, and Authority changes;
- CPR-10: Authority-Aware Decision Brief usefulness;
- CPR-12: authority-question accuracy;
- CPR-13: explanation of why sources govern or do not govern;
- CPR-14: governed change-impact reasoning without automatic mutation;
- CPR-15: separation of observed change from inferred consequence.

A positive result does not automatically promote any CPR to Approved status. Promotion remains a separate Founder decision.

---

## 18. What This Protocol Does Not Decide

RNO-004 does not decide:

- Product Vision approval;
- MVP approval;
- commercialization;
- target buyer;
- pricing or packaging;
- Project Intelligence positioning;
- category creation;
- application governance;
- architecture;
- retrieval technology;
- model provider;
- storage technology;
- knowledge-graph usage;
- agent implementation;
- autonomous stewardship;
- repository integration strategy;
- Product Gate approval.

---

## 19. Open Questions

- Should weighted scoring remain stable across all validation cycles or vary by case type?
- What minimum number of cases is sufficient before drawing a Phase 2 product conclusion?
- Should more than one human evaluator score decision usefulness and authority explanation?
- How should inter-rater disagreement be represented when experts disagree on authority interpretation?
- Which model should serve as the initial common-model baseline?
- Should Condition B use a specific retrieval product or a minimal retrieval workflow?
- What evidence threshold should justify promoting any candidate requirement into a Product Decision Record?
- Should later validation include external evaluators who do not know Olympus terminology?

---

## 20. Next Action

Continue Phase 2 Product Definition to establish the first bounded Olympus behavior worth validating.

Preserve the illustrative candidate cases in Section 15 as future evaluation seeds. Do not construct or freeze the full Experiment 01A evaluation set until the first bounded product behavior is sufficiently defined.

Once that behavior is defined, construct and freeze the applicable cases, source manifests, prompts, and answer key before running Condition A, B, or C.

---

## Change History

| Date | Author | Summary |
|---|---|---|
| 2026-08-15 | Hermes under explicit Founder direction | Created the Draft / Informational authority-aware judgment validation protocol for Phase 2. |
| 2026-08-15 | Hermes under explicit Founder direction | Preserved three illustrative validation candidates, clarified that they are not frozen test cases, and deferred full Experiment 01A construction until a bounded product behavior is defined. |