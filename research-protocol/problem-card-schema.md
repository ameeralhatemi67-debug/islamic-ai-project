# Progressive Problem Card Schema

This document defines the canonical specification for Problem Cards across their entire lifecycle in the Islamic AI Research Collective.

---

# 1. Architectural Philosophy: The Progressive Problem Card

A Problem Card is not an idea pitch, and it is not a monolithic 40-question form that every researcher must fill out immediately.

Instead, **one single Problem Card evolves progressively through four distinct maturity levels**, with strict phase separation and agent ownership:

```text
LEVEL 1: DISCOVERED PROBLEM
Authored by Discovery Researchers (Agents 01–04) during Phase 1
Focus: Real user, painful workflow, consequences, evidence, existing workarounds, disconfirmation, trust boundaries.
Strict Boundary: NO AI solution design, NO model selection, NO demo pitch.

       │
       ▼
LEVEL 2: VALIDATED PROBLEM
Audited and advanced by Research Director (Agent 08) during Phase 2
Focus: Intake validation, duplicate/merge status, evidence quality, workflow confidence, framing refinements.

       │
       ▼
LEVEL 3: MARKET-TESTED PROBLEM
Expanded by Market Landscape Researcher (Agent 05) during Phase 3
Focus: Canonical Reference Projects (RP-*), coverage analysis, strongest alternatives, canonical Gap ID (GAP-*).

       │
       ▼
LEVEL 4: OPPORTUNITY-READY PROBLEM
Expanded by AI Opportunity (Agent 06), Red Team (Agent 07), Cross-Examination, and Director (Agent 08)
Focus: Non-AI baseline vs AI leverage (AI-OP-*), adversarial stress-testing, surviving claims, synthesis disposition.
```

---

# 2. Problem ID Allocation & Filenames

To prevent identifier collisions during concurrent discovery, stable ID ranges are strictly allocated:

- **Agent 01 (Muslim User Researcher):** `P-001` through `P-099`
- **Agent 02 (New Muslim Researcher):** `P-100` through `P-199`
- **Agent 03 (Educator & Da'wah Researcher):** `P-200` through `P-299`
- **Agent 04 (Islamic Trust Researcher):** `P-300` through `P-399`
- **Director-Merged / Cross-Cutting Cards:** `P-800` through `P-899`

### Canonical Filename Pattern:
```text
research/problem-cards/P-XXX-short-descriptive-slug.md
```
Examples:
- `P-014-content-creator-source-verification.md`
- `P-103-convert-terminology-fragmentation.md`
- `P-205-madrasah-tajweed-feedback-scarcity.md`

Problem IDs remain stable once assigned. Never reuse retired IDs.

---

# 3. Canonical Progressive Problem Card Template

Every Problem Card must use this single canonical template. Sections are completed **only when the problem reaches that phase**.

```markdown
# [P-XXX] Problem Title

---

## METADATA & MATURITY

- **Problem ID:** P-XXX
- **Current Maturity Level:** LEVEL 1 — DISCOVERED | LEVEL 2 — VALIDATED | LEVEL 3 — MARKET-TESTED | LEVEL 4 — OPPORTUNITY-READY
- **Problem Status:** UNVALIDATED | PROMISING | VALIDATED | REQUIRES REFRAME | DUPLICATE-MERGED | DISCONFIRMED | WEAK | REJECTED
- **Primary Research Owner:** Agent 01 / 02 / 03 / 04
- **Date Created:** YYYY-MM-DD
- **Last Updated:** YYYY-MM-DD

---

# ==============================================================================
# LEVEL 1 — DISCOVERED PROBLEM (Phase 1: Agents 01–04)
# Required for all new cards. Completed during independent discovery.
# ==============================================================================

## 1. One-Sentence Problem Statement
[Specific user] struggles to [complete important task] because [core friction], resulting in [meaningful consequence].

## 2. Primary User & Context
- **Primary User:** (Specific role, experience level, language, geography, relevant traits. Avoid generic "Muslims".)
- **Why This User Matters:** 
- **User Context & Trigger:** (When and where does the problem occur? What triggers the task?)
- **Environmental Constraints:** (Device, connectivity, language constraints, time pressure.)
- **Existing Tools Used:** (What tools does the user currently have open?)

## 3. Secondary Users & Stakeholders
- **Secondary Users:** (People indirectly affected, e.g., students, children, congregation.)
- **Human Reviewers / Authorities Involved:** (Teachers, scholars, community mentors.)

## 4. Job to Be Done
- **When:** [Situation / Trigger]
- **I want to:** [Task / Motivation]
- **So that:** [Desired Outcome]
- **Success looks like:** [Observable, concrete success state]

## 5. Current Reconstructed Workflow
(Step-by-step sequence of what the user actually does today.)
- **Trigger:**
- **Step 1:**
- **Step 2:**
- **Step 3:**
- **Step 4:**
- **Final Outcome:**

## 6. Workflow Evidence Grounding
(Identify epistemic status of each workflow step: DIRECTLY OBSERVED | USER REPORTED | INFERRED | UNKNOWN.)
- Step 1 Status:
- Step 2 Status:
- Step 3 Status:
- Inferred / Missing Workflow Steps:

## 7. Core Pain Point
- **Exact Friction Point:** (Where in the workflow does the breakdown or lost time occur?)
- **Root Cause Hypothesis:** (Why does it occur? Differentiate root cause from superficial symptom.)

## 8. Consequences & Impact
- **Immediate Consequence:** (Wasted minutes, abandoned task, confusion.)
- **Long-term Consequence:** (Spiritual disillusionment, persistent misinformation, learning stall.)
- **Religious & Trust Consequence:** (Misattributed text, incorrect practice, ungrounded fatwa.)
- **Emotional / Cognitive Cost:** (Anxiety, guilt, cognitive overload.)

## 9. Frequency & Severity
- **Frequency:** Multiple times daily | Daily | Weekly | Seasonal | Rare
  - *Evidence & Confidence:* [High | Medium | Low]
- **Severity:** Catastrophic / Critical | High friction | Moderate annoyance | Minor
  - *Evidence & Confidence:* [High | Medium | Low]

## 10. Existing Workarounds
(What users currently do to cope without a dedicated modern solution.)
1. **Workaround 1:** (e.g., Manually searching 5 disparate websites and comparing notes.)
2. **Workaround 2:** (e.g., Asking in unverified social forums / Discord.)
- **Why Workarounds Fail:** (Cost, fatigue, errors, latency.)

## 11. Initial Reference Candidates Encountered
(Lightweight records of existing tools noticed during discovery. Formal analysis belongs to Agent 05.)
- **Candidate 1:** [Name] | [URL] | Target: [...] | What it does: [...] | Observed limitation/user complaint: [...]
- **Candidate 2:** [Name] | [URL] | Target: [...] | What it does: [...] | Observed limitation/user complaint: [...]

## 12. Supporting Evidence
- **[EVIDENCE-ID]:** Source Name | URL/Citation | Date
  - *Extracted Quote / Data:* "..."
  - *Supports:* (Specific claim supported)
  - *Confidence:* High | Medium | Low

## 13. Contradicting / Disconfirming Evidence
- **Evidence Weakening Problem:** (Findings showing problem is rare, easily bypassed, or already solved.)
- **Source & Citation:**

## 14. Disconfirmation Search Conducted
- **Falsification Hypothesis:** (What would prove this problem is NOT worth pursuing?)
- **Searches Performed:**
- **Disconfirmation Findings:**

## 15. Islamic Knowledge & Trust Considerations
- **Doctrinal Areas Involved:** Qur'an | Hadith | Classical Fiqh | Contemporary Fatwa | Arabic Pedagogy | None
- **Scholarly Disagreement (Ikhtilaf):** (Are there diverse orthodox positions? Does consensus exist?)
- **Personal Circumstance Sensitivity:** (Does this involve marriage, finance, purity, or high-stakes personal rulings?)
- **Required Governance Markers:**
  - `[REQUIRES ISLAMIC SCHOLAR REVIEW]`
  - `[REQUIRES SOURCE-BOUNDARY AUDIT]`
  - `[NO AUTONOMOUS FATWA PERMITTED]`

## 16. Assumptions, Unknowns & Evidence Gaps
- **[ASSUMPTION]:**
- **[UNKNOWN]:**
- **[EVIDENCE GAP]:** (Critical missing information needed to validate problem.)

## 17. Confidence in Problem Existence
- **Problem Existence Confidence:** High | Medium | Low
- **Justification:** (Based on triangulation of direct user reports vs observations.)

## 18. Required Next Research (Discovery Phase)
- 1.
- 2.

## 19. Early Idea Hypothesis (Optional — Strictly Non-Binding)
*(Discovery researchers are forbidden from designing AI solutions. If an intuitive idea occurred naturally during research, record it strictly as an unvalidated hypothesis here.)*
- `[HYPOTHESIS]`: (e.g., Contextual inline definition might reduce external search fragmentation.)

---

# ==============================================================================
# LEVEL 2 — VALIDATED PROBLEM (Phase 2: Agent 08 Research Director)
# Completed by Agent 08 during intake audit.
# ==============================================================================

## 20. Director Validation Audit
- **Validation Decision:** VALIDATED | PROMISING | REQUIRES REFRAME | DUPLICATE-MERGED | DISCONFIRMED | REJECTED
- **Duplicate / Merge Check:** (Is this a duplicate of another card? Merged IDs: [...])
- **Evidence Quality Audit:** (Are user quotes traceable? Is sample size sufficient?)
- **Workflow Confidence:** (Is the workflow verified or speculative?)
- **Problem Framing Critique:** (Is the problem scoped cleanly without premature solution assumptions?)
- **Critical Evidence Gaps to Resolve:**
- **Gate to Phase 3 (Market Landscape):** APPROVED | HOLD FOR TARGETED REVISION | REJECTED

---

# ==============================================================================
# LEVEL 3 — MARKET-TESTED PROBLEM (Phase 3: Agent 05 Market Landscape)
# Completed by Agent 05 after market and competitor research.
# ==============================================================================

## 21. Canonical Reference Projects Reviewed
(Links to formal reference project files in `/research/reference-projects/`.)
- `[RP-XXX]`: Project Name | Platform | Relevance
- `[RP-YYY]`: Project Name | Platform | Relevance

## 22. Existing Solution Coverage Analysis
- **Full Solvers:** (Do any existing apps completely solve this workflow?)
- **Partial Solvers:** (Which apps cover steps 1–2 but fail on step 3?)
- **Strongest Non-AI / Conventional Alternatives:** (Databases, static books, human services.)

## 23. Canonical Market / Workflow Gap
- **Assigned Gap ID:** GAP-XXX
- **Unresolved Gap Statement:** (What exact friction remains unaddressed by all existing products?)
- **Gap Confidence:** High | Medium | Low
- **Is Gap Genuine or Feature Request?** (Differentiate a true workflow gap from a missing button in App X.)
- **Market Disposition:** PROCEED TO AI EVALUATION | PROBLEM ALREADY SOLVED | COMMERCIALLY UNSUSTAINABLE

---

# ==============================================================================
# LEVEL 4 — OPPORTUNITY-READY PROBLEM (Phases 4–7: Agents 06, 07 & 08)
# Multi-agent synthesis before opportunity mapping.
# ==============================================================================

## 24. AI Opportunity Evaluation (Agent 06 — Phase 4)
- **Assigned AI Opportunity ID:** AI-OP-XXX
- **Strongest Non-AI Baseline:** (How could this be solved using deterministic code, SQL, or static UI?)
- **Specific AI Capability Justified:** (Why must AI earn its place? e.g., phoneme acoustic modeling, semantic RAG, cross-lingual entity matching.)
- **Why AI May Help:**
- **Why AI May Be Unnecessary or Inferior:**
- **Expected Measurable Improvement:** (Hypothetical testing baseline: task completion time, citation accuracy, error rate.)
- **Technical Feasibility & Data Constraints:** (Available datasets, compute requirements, offline/on-device viability.)

## 25. Adversarial Red Team Review (Agent 07 — Phase 5)
- **Assigned Challenge ID:** RT-XXX / A-XXX
- **Critical Assumptions Challenged:**
- **P0 Failure Modes (Fatal Flaws):**
- **P1 Issues (Severe Complications):**
- **Theological & Ethical Risks:** (Hallucination risk, sectarian bias, commercialization of sacred text.)

## 26. Cross-Examination & Surviving Claims (Phase 6)
- **CX Reference ID:** CX-XXX
- **Key Objections Debated:**
- **Accepted Limitations & Scoped Boundaries:**
- **Surviving Claims:** (What claims withstood rigorous council attack?)

## 27. Final Research Disposition (Agent 08 — Phase 7)
- **Final Disposition:** OPPORTUNITY-READY | EXPLORATORY | SHELVED / HOLD | REJECTED
- **Disposition Justification:**
- **Key Decision-Changing Questions for Hackathon Strategy:**
- **Eligible for Opportunity Map:** YES | NO

---

# ==============================================================================
# CHANGE LOG & AUDIT TRAIL
# ==============================================================================

| Date | Agent | Level Transition | Summary of Changes | Rationale |
|---|---|---|---|---|
| YYYY-MM-DD | Agent 01 | Created Level 1 | Initial problem discovery | Discovery phase input |
```

---

# 4. Phase-Specific Guidelines & Anti-Anchoring Rules

### Rule for Agents 01–04 (Phase 1 Discovery)
- **Focus:** Fill Sections 1 through 19.
- **Strict Boundary:** Do not propose AI models, software architectures, prompt engineering pipelines, or demo scripts.
- **Lightweight Reference Candidates:** Record candidate tools you see users complaining about or using in Section 11. Do not fill out full `RP-*` competitor files.

### Rule for Agent 08 (Phase 2 Validation)
- **Focus:** Review Sections 1–19 and complete Section 20.
- Ensure the problem is grounded in empirical user evidence, not abstract enthusiasm.

### Rule for Agent 05 (Phase 3 Market Landscape)
- **Focus:** Review validated cards and complete Sections 21 through 23.
- Map the problem against formal `RP-*` records in `/research/reference-projects/` and assign a formal `GAP-XXX`.

### Rule for Agent 06 (Phase 4 AI Opportunities)
- **Focus:** Complete Section 24.
- Force AI to "earn its place" by contrasting it against the strongest non-AI baseline.

### Rule for Agent 07 (Phase 5 Red Team)
- **Focus:** Complete Section 25.
- Identify how the problem could be exaggerated, already solved, or religiously hazardous.

### Rule for Agent 08 (Phase 7 Synthesis)
- **Focus:** Complete Sections 26 and 27 after Cross-Examination.
- Determine final readiness for the Opportunity Map.