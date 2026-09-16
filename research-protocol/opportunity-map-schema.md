## Islamic AI Challenge — Opportunity Map Schema

This document defines how validated problems, market gaps, AI opportunities, trust constraints, feasibility findings, and cross-examination results must be synthesized into a single comparable opportunity landscape.

The Opportunity Map is the primary synthesis artifact used to understand:

- which problems are genuinely supported;
    
- who experiences them;
    
- what workflows are failing;
    
- what already exists;
    
- what remains unresolved;
    
- where AI may create meaningful value;
    
- where AI is unnecessary;
    
- what risks or constraints apply;
    
- what survived adversarial review;
    
- what remains uncertain.
    

The Opportunity Map is **not a ranking table and not a final project-selection mechanism**.

It is designed to make later decisions evidence-based.

This schema supplements:

- `AGENTS.md`
    
- `research-protocol/source-policy.md`
    
- `research-protocol/evidence-standard.md`
    
- `research-protocol/problem-card-schema.md`
    
- `research-protocol/reference-project-schema.md`
    
- `research-protocol/cross-examination-protocol.md`
    
- `agents/08-research-director.md`
    

If this schema conflicts with `AGENTS.md`, follow `AGENTS.md`.

The Research Director owns the final Opportunity Map.

---

# 1. Core Principle

The Opportunity Map must answer:

> **What opportunities remain defensible after problem validation, market research, AI analysis, trust review, and adversarial challenge?**

The map must not answer:

> “Which idea sounds most exciting?”

The required synthesis order is:

```text
Problem

→

User

→

Workflow

→

Evidence

→

Existing Solutions

→

Remaining Gap

→

AI Leverage

→

Non-AI Alternative

→

Measurement

→

Trust / Safety

→

Feasibility

→

Cross-Examination

→

Confidence
```

---

# 2. Purpose

The Opportunity Map exists to:

- place different opportunities into a common structure;
    
- expose weak evidence;
    
- expose unresolved assumptions;
    
- preserve negative findings;
    
- identify cross-agent convergence;
    
- distinguish user value from technical novelty;
    
- distinguish AI value from AI presence;
    
- make later prioritization easier;
    
- prevent premature commitment to one concept.
    

The map should make weak opportunities look weak.

It should not beautify them.

---

# 3. What Counts as an Opportunity

An Opportunity is not simply:

> an idea.

An Opportunity represents a validated or partially validated combination of:

```text
USER

+

IMPORTANT JOB

+

WORKFLOW FAILURE

+

UNRESOLVED GAP

+

POTENTIAL IMPROVEMENT
```

AI may or may not be part of that improvement.

An Opportunity should normally be linked to at least one:

```text
Problem Card
```

and where applicable:

```text
Market Gap
AI Opportunity
Reference Project
Cross-Examination Result
```

---

# 4. Opportunity IDs

Use stable IDs.

Recommended format:

```text
OPP-001
OPP-002
OPP-003
```

Do not reuse IDs.

If an opportunity is removed, preserve the ID and mark its status.

Example:

```text
OPP-004 — DISCONTINUED
```

Do not silently recycle it.

---

# 5. Opportunity Status

Use one of:

```text
EXPLORATORY

SUPPORTED

SUPPORTED WITH LIMITATIONS

REQUIRES VALIDATION

WEAKENED

HOLD

DISCONTINUED

DISCONFIRMED
```

Definitions:

### EXPLORATORY

Early evidence exists but major validation remains.

### SUPPORTED

Core claims are supported and major challenges have been addressed.

### SUPPORTED WITH LIMITATIONS

Opportunity remains credible but important limitations remain.

### REQUIRES VALIDATION

Material assumptions remain unresolved.

### WEAKENED

New evidence materially reduces confidence.

### HOLD

Cannot progress until a key dependency is resolved.

### DISCONTINUED

The team should not continue investing effort under the current framing.

### DISCONFIRMED

Evidence directly undermines the central claim.

---

# 6. Full Opportunity Record

Each major opportunity should follow this structure:

```text
# [OPP-XXX] Opportunity Title

## 1. Status

Opportunity Status:

Overall Maturity:
Early / Developing / Mature Enough for Selection Review

Last Updated:

Director:

---

## 2. Primary User

User:

User Context:

Geography:
If relevant

Language:
If relevant

Knowledge / Experience Level:
If relevant

Relevant Problem IDs:

---

## 3. Job to Be Done

What is the user trying to accomplish?

---

## 4. Current Workflow

Step 1:
...

Step 2:
...

Step 3:
...

Primary failure point:
...

---

## 5. Core Problem

Problem statement:

Why it matters:

Frequency:

Severity / consequence:

Evidence confidence:

---

## 6. Supporting Evidence

Evidence IDs / citations:

Behavioral evidence:

Academic / expert evidence:

Community evidence:

Other evidence:

---

## 7. Contradicting Evidence

...

---

## 8. Existing Workarounds

...

---

## 9. Existing Solutions

Direct competitors:

Partial competitors:

Adjacent Islamic projects:

Adjacent-domain references:

Manual / human alternatives:

Non-AI alternatives:

---

## 10. Remaining Gap

Gap ID:

Gap statement:

Gap type:

Gap status:

Evidence supporting gap:

Evidence against gap:

---

## 11. AI Opportunity

AI Opportunity ID:

AI capability:

Workflow step improved:

Why AI may help:

Why AI may be unnecessary:

---

## 12. Strongest Non-AI Alternative

...

---

## 13. Expected User Benefit

...

---

## 14. Measurement

Baseline:

Metric:

Test method:

Who validates:

Expected direction of improvement:

---

## 15. Trust / Islamic Safety

Trust risks:

Religious-boundary risks:

Source requirements:

Refusal requirements:

Human / scholar escalation:

Risk status:

---

## 16. Technical Feasibility

Data availability:

Model capability:

Implementation complexity:

Latency:

Cost:

Integration:

Evaluation feasibility:

Overall feasibility:

---

## 17. Hackathon Feasibility

Can the core value be demonstrated within the challenge period?

Prototype scope:

Critical dependencies:

Demo workflow:

---

## 18. Differentiation

What is genuinely different?

What is NOT meaningful differentiation?

Reference projects compared:

---

## 19. Critical Assumptions

A-...

A-...

---

## 20. Red Team Findings

P0 findings:

P1 findings:

Resolved challenges:

Accepted limitations:

---

## 21. Cross-Examination Result

Result:

Proceed / Proceed with Limitations / Rework / Hold / Discontinue

Surviving claims:

Revised claims:

Disconfirmed claims:

---

## 22. Confidence by Dimension

Problem Existence:

User Importance:

Market Gap:

AI Leverage:

Measurability:

Trust Mitigation:

Feasibility:

Hackathon Fit:

---

## 23. Open Questions

...

---

## 24. Required Follow-Up

...

---

## 25. Director Synthesis

[DIRECTOR SYNTHESIS]

...

---

## 26. Why This Opportunity May Be Worth Pursuing

...

---

## 27. Strongest Reason Not to Pursue It

...

```

---

# 7. Opportunity Title Rules

Titles should describe the opportunity in terms of:

- user;
    
- job;
    
- failure;
    
- gap.
    

Good:

> Source-verification workflow for Islamic content creators

Good:

> Multilingual Islamic terminology support for new Muslims

Weak:

> Islamic AI App

Weak:

> Smart Muslim Assistant

Weak:

> AI RAG Platform

Avoid technology-led titles unless the opportunity itself is technical.

---

# 8. Primary User

Each opportunity must identify a specific user.

Avoid:

> Muslims

Prefer:

> English-speaking new Muslims independently learning Islamic concepts online.

or:

> Arabic-speaking Islamic content creators who regularly verify source material before publishing.

If multiple user groups share the same root problem, identify:

```text
PRIMARY USER

SECONDARY USERS
```

Do not broaden the opportunity artificially.

---

# 9. User Context

Capture context that materially changes the problem.

Examples:

- beginner versus advanced learner;
    
- professional versus casual user;
    
- Arabic versus non-Arabic speaker;
    
- educator versus student;
    
- individual versus institution.
    

Do not add unnecessary demographic detail.

---

# 10. Problem Linkage

Each Opportunity must reference validated Problem Cards.

Example:

```text
PRIMARY PROBLEM:
P-014

RELATED PROBLEMS:
P-021
P-028
```

Do not create an Opportunity without a traceable problem basis.

If necessary:

```text
[INSUFFICIENT PROBLEM VALIDATION]
```

---

# 11. Job to Be Done

Express what the user is trying to accomplish.

Prefer:

> Verify the Islamic source and context behind a claim before publishing it.

over:

> Use an Islamic AI tool.

The Job to Be Done should remain technology-neutral.

---

# 12. Current Workflow

Reconstruct the workflow before proposing improvement.

Example:

```text
Receive topic
→ search Google
→ search Islamic websites
→ verify hadith
→ compare sources
→ translate material
→ draft content
→ add references
→ review manually
```

Identify where:

- time is lost;
    
- errors occur;
    
- source traceability disappears;
    
- users change tools;
    
- expert support is required.
    

---

# 13. Core Problem Statement

Use:

```text
[USER]

struggles to

[TASK]

because

[WORKFLOW FAILURE],

resulting in

[CONSEQUENCE].
```

Example:

> Islamic content creators struggle to verify and preserve the provenance of religious claims because research is fragmented across multiple tools, resulting in time loss and increased risk of unsupported statements.

Do not insert the proposed solution into the problem statement.

---

# 14. Frequency

Use descriptive evidence.

Possible values:

```text
Recurring

Frequent

Occasional

Rare

Unknown
```

Only use a label if evidence supports it.

When prevalence is unknown:

```text
UNKNOWN
```

Do not guess.

---

# 15. Severity / Consequence

Describe consequences such as:

- time loss;
    
- incorrect understanding;
    
- publication errors;
    
- trust loss;
    
- accessibility barriers;
    
- expert workload;
    
- abandonment.
    

Do not exaggerate harm.

---

# 16. Evidence Strength

Use:

```text
STRONG

MODERATE

WEAK

INSUFFICIENT
```

Strong should normally require multiple high-quality or independent forms of evidence.

Follow `evidence-standard.md`.

---

# 17. Behavioral Evidence

Where possible, identify evidence that users actually change behavior.

Examples:

- use multiple tools;
    
- manually verify AI output;
    
- ask scholars;
    
- maintain spreadsheets;
    
- repeatedly search similar questions;
    
- abandon a tool.
    

Behavioral evidence may strengthen importance.

---

# 18. Contradicting Evidence

Every Opportunity Record must include contradictory evidence.

If none was found:

```text
NO MATERIAL CONTRADICTORY EVIDENCE FOUND
```

Do not write:

> None exists.

Absence of discovered contradiction is not proof of absence.

---

# 19. Existing Solutions

Reference relevant:

```text
RP-XXX
ADJ-XXX
TECH-XXX
```

Do not merely name products.

Explain whether they solve:

- the entire job;
    
- part of the job;
    
- only a related task.
    

---

# 20. Workaround Analysis

A workaround may be:

```text
Human scholar

Google search

Several apps combined

Manual spreadsheet

Private notes

General-purpose AI + manual checking
```

Workarounds reveal both:

- need;
    
- existing sufficiency.
    

A workaround that works well may weaken the opportunity.

---

# 21. Gap Statement

A gap should describe what remains unresolved.

Good:

> Existing systems retrieve Islamic sources, but users still manually compare evidence and preserve citations across separate tools.

Weak:

> There is no good AI solution.

---

# 22. Gap Types

Use one or more:

```text
NO ADEQUATE SOLUTION FOUND

PARTIALLY SOLVED

FRAGMENTED WORKFLOW

TRUST / RELIABILITY GAP

LANGUAGE GAP

LOCALIZATION GAP

ACCESSIBILITY GAP

SOURCE COVERAGE GAP

VERIFICATION GAP

WORKFLOW INTEGRATION GAP

COST / ACCESS GAP

EXPERT-DEPENDENCE GAP

TECHNICAL CAPABILITY GAP

ADOPTION GAP
```

---

# 23. Gap Status

Use:

```text
STRONGLY SUPPORTED

PARTIALLY SUPPORTED

WEAK

ALREADY SOLVED

DISCONFIRMED

UNKNOWN
```

Gap confidence must reflect Agent 05 and cross-examination evidence.

---

# 24. AI Opportunity Linkage

Reference:

```text
AI-OP-XXX
```

if Agent 06 has validated an AI opportunity.

Do not invent AI leverage during synthesis if Agent 06 has not examined it.

---

# 25. AI Capability

Specify the actual capability.

Examples:

```text
Multilingual semantic retrieval

Claim-source alignment

Cross-document comparison

Terminology-aware translation

Adaptive learning sequencing
```

Avoid:

> AI assistant

unless that description is genuinely precise enough.

---

# 26. AI Leverage

Use:

```text
STRONG

MODERATE

WEAK

UNNECESSARY

UNKNOWN
```

Strong AI leverage means:

- the task is validated;
    
- conventional alternatives are materially weaker;
    
- AI capability fits the task;
    
- improvement is plausible and measurable.
    

---

# 27. Strongest Non-AI Alternative

Every opportunity must contain this section.

Examples:

```text
Curated search engine

Keyword search + filters

Structured database

Expert service

Static learning pathway

Rules engine
```

A serious Opportunity Map should make non-AI competition visible.

---

# 28. Why AI May Be Unnecessary

Even strong opportunities should preserve this question.

Possible answers:

- current search is already sufficient;
    
- deterministic logic works;
    
- problem is UX rather than intelligence;
    
- human review dominates the workflow.
    

Do not hide this because the event is AI-focused.

---

# 29. User Benefit

Describe benefit at the task level.

Examples:

```text
Faster verification

Fewer unsupported claims

Improved comprehension

Reduced tool switching

More reliable translation

Reduced expert review burden
```

Avoid vague:

> “Better user experience.”

---

# 30. Measurement

Each Opportunity should define at least one plausible metric.

Examples:

```text
Task completion time

Top-k retrieval relevance

Citation support accuracy

Unsupported claim count

Comprehension score

Translation fidelity

Human review time

Successful task completion
```

---

# 31. Baseline

Use a real baseline.

Examples:

```text
Existing product RP-004

Google search

Keyword search

Current manual workflow

Human-only workflow
```

Do not compare against an artificially poor baseline.

---

# 32. Measurement Clarity

Use:

```text
CLEAR

PLAUSIBLE

DIFFICULT

UNCLEAR

NOT CREDIBLY MEASURABLE
```

Explain why.

---

# 33. Trust Risks

Use Agent 04 findings.

Relevant dimensions include:

```text
SOURCE

ATTRIBUTION

CITATION

CONTEXT

TRANSLATION

SCOPE

UNCERTAINTY

BOUNDARY

CORRECTION
```

Not every opportunity has the same trust profile.

---

# 34. Religious Boundary Risk

Use:

```text
LOW

MODERATE

HIGH

REQUIRES SCHOLAR / HUMAN OVERSIGHT

UNACCEPTABLE UNDER CURRENT DESIGN
```

Do not independently decide complex Islamic rulings.

---

# 35. Source Requirement

Record whether the opportunity requires:

- Qur'anic corpus;
    
- hadith corpus;
    
- fatwa corpus;
    
- Bin Baz corpus;
    
- multilingual translation;
    
- institutional sources;
    
- academic sources.
    

Also note:

```text
DATA ACCESS:
Open / Restricted / Partial / Unknown
```

---

# 36. Refusal Requirements

Where relevant, specify cases where the system should not answer.

Examples:

- personal fatwa;
    
- insufficient context;
    
- unresolved source disagreement;
    
- missing evidence.
    

Refusal behavior may itself be part of product quality.

---

# 37. Escalation Requirements

Record:

```text
ESCALATION REQUIRED?
Yes / No / Conditional

TO:
Scholar / Expert / Human reviewer

TRIGGER:
...
```

---

# 38. Technical Feasibility

Use:

```text
HIGH

MEDIUM

LOW

BLOCKED

UNKNOWN
```

Consider:

- data;
    
- AI capability;
    
- APIs;
    
- evaluation;
    
- implementation;
    
- integration.
    

---

# 39. Data Readiness

Use:

```text
STRONG

PARTIAL

WEAK

UNAVAILABLE

UNKNOWN
```

Explain major constraints.

---

# 40. Hackathon Feasibility

This differs from long-term technical feasibility.

Use:

```text
HIGH

MEDIUM

LOW
```

Ask:

> Can the core value be demonstrated as a functioning system within the challenge constraints?

---

# 41. Prototype Scope

Define the minimum meaningful demonstration.

Example:

> Retrieve, compare, and verify source passages for one defined content-creator workflow using a limited trusted corpus.

Do not require the prototype to solve the entire future product.

---

# 42. Demo Workflow

Capture:

```text
BEFORE:

...

AFTER:

...

MEASURED CHANGE:

...
```

The demo should expose user value.

Not merely AI output.

---

# 43. Differentiation

Describe differentiation relative to relevant projects.

Potential meaningful differentiation:

- claim-level provenance;
    
- cross-lingual semantic retrieval;
    
- disagreement visualization;
    
- workflow integration;
    
- safer human escalation.
    

Avoid:

- AI-powered;
    
- modern;
    
- smart;
    
- innovative;
    
- all-in-one;
    

unless supported by something specific.

---

# 44. Critical Assumptions

Reference:

```text
A-XXX
```

Every serious Opportunity should identify at least one critical assumption.

Example:

> Users value faster source verification enough to adopt a new workflow.

---

# 45. Critical Assumption Status

Use:

```text
SUPPORTED

PARTIALLY SUPPORTED

UNVERIFIED

DISCONFIRMED
```

An opportunity cannot be considered mature if central assumptions remain completely unverified.

---

# 46. Red Team Findings

Reference:

```text
CX-XXX
A-XXX
```

Capture:

```text
P0 challenges

P1 challenges

Resolved findings

Open findings

Accepted limitations
```

Do not summarize:

> Red Team approved.

Show what survived.

---

# 47. Cross-Examination Status

Use:

```text
PROCEED

PROCEED WITH LIMITATIONS

REWORK

HOLD

DISCONTINUE
```

This status should come from the Research Director.

---

# 48. Confidence by Dimension

Each Opportunity must separately report:

```text
PROBLEM EXISTENCE:
Strong / Moderate / Weak

USER IMPORTANCE:
Strong / Moderate / Weak

MARKET GAP:
Strong / Moderate / Weak

AI LEVERAGE:
Strong / Moderate / Weak / Unnecessary

MEASURABILITY:
Clear / Plausible / Difficult

TRUST MITIGATION:
Strong / Partial / Weak

TECHNICAL FEASIBILITY:
High / Medium / Low

HACKATHON FEASIBILITY:
High / Medium / Low
```

Avoid one overall confidence score.

---

# 49. No Composite Score

Do not calculate:

```text
Opportunity Score = 83/100
```

unless a later explicitly defined selection framework requires it.

Composite scoring creates false precision and can hide fatal weaknesses.

---

# 50. Opportunity Map Summary Table

The Director should maintain a high-level comparison table.

Recommended structure:

```text
| ID | Opportunity | User | Problem Evidence | Gap | AI Leverage | Measurement | Trust Risk | Feasibility | Cross-Examination | Status |
|---|---|---|---|---|---|---|---|---|---|---|
```

Use descriptive values.

---

# 51. Optional Extended Table

Where useful:

```text
| ID | User | Job | Pain | Evidence | Existing Solutions | Gap | AI | Non-AI | Metric | Trust | Feasibility | P0 Risk |
```

Do not overload the summary table with every detail.

Use individual Opportunity Records for depth.

---

# 52. Opportunity Clusters

Group opportunities into meaningful clusters where patterns emerge.

Possible examples:

```text
TRUST & PROVENANCE

KNOWLEDGE RETRIEVAL

LEARNING

MULTILINGUAL / LOCALIZATION

CONTENT CREATION

VERIFICATION

ACCESSIBILITY

RESEARCH WORKFLOW
```

Clusters must emerge from findings.

Do not force artificial categories.

---

# 53. Root-Problem Clustering

Where several opportunities share one root failure, show that relationship.

Example:

```text
ROOT:
Weak source provenance

↓

OPP-003:
Content creator verification

OPP-008:
Learner trust

OPP-011:
Research assistant workflow
```

This may reveal broader strategic directions later.

---

# 54. Cross-Segment Opportunities

Some opportunities may serve multiple segments.

Do not assume that makes them stronger.

Record:

```text
PRIMARY USER:

SECONDARY USER:

SHARED ROOT PROBLEM:

IMPORTANT DIFFERENCES:
```

A broad opportunity may require different workflows per user.

---

# 55. Preserve Segment-Specific Differences

Example:

```text
New Muslims:
Need explanation and terminology.

Researchers:
Need provenance and source comparison.
```

Do not merge because both involve Islamic knowledge.

---

# 56. Cross-Agent Convergence

Use:

```text
[CROSS-AGENT CONVERGENCE]
```

when independently supported findings reinforce an opportunity.

Capture:

```text
Agents:

Independent evidence:

Shared conclusion:

Confidence impact:
```

---

# 57. Shared-Source Warning

If agents rely on the same underlying evidence:

```text
[SHARED-SOURCE DEPENDENCY]
```

Do not count this as independent convergence.

---

# 58. Negative Opportunities

The Opportunity Map should preserve major directions found to be poor.

Create a section:

```text
## Disconfirmed / Discontinued Opportunities
```

Include:

```text
ID

Original opportunity

Reason discontinued

Evidence

What we learned
```

This prevents repetition.

---

# 59. AI-Rejected Opportunities

Create:

```text
## Problems Where AI Was Unnecessary
```

Examples:

- deterministic search sufficient;
    
- better UX sufficient;
    
- manual expert service appropriate.
    

This is valuable evidence.

---

# 60. Already-Solved Problems

Create:

```text
## Problems Adequately Addressed by Existing Solutions
```

This prevents reinventing existing products.

---

# 61. High-Risk Opportunities

Create:

```text
## High-Risk / Boundary-Sensitive Opportunities
```

Include:

- opportunity;
    
- risk;
    
- mitigation;
    
- whether the risk is structural.
    

Do not hide risk in footnotes.

---

# 62. Strong Non-AI Alternatives

Create a section where important:

```text
## Strong Non-AI Alternatives
```

This improves later strategic decisions.

---

# 63. Open Questions

Every Opportunity should link to relevant:

```text
Q-XXX
```

from:

```text
/synthesis/open-questions.md
```

Open questions should remain visible in the map.

---

# 64. Disagreements

Reference:

```text
DAGR-XXX
```

or the chosen disagreement ID format.

Do not resolve genuine disagreement through summary compression.

---

# 65. Opportunity Maturity

Optional maturity labels:

```text
LEVEL 0 — Hypothesis

LEVEL 1 — Problem Evidenced

LEVEL 2 — Gap Evidenced

LEVEL 3 — AI / Intervention Evidenced

LEVEL 4 — Adversarially Reviewed

LEVEL 5 — Selection Ready
```

These labels describe research maturity.

They are not quality rankings.

---

# 66. Maturity Level Rules

### LEVEL 0

Problem mostly hypothetical.

### LEVEL 1

Problem has meaningful evidence.

### LEVEL 2

Existing-solution landscape supports an unresolved gap.

### LEVEL 3

Intervention / AI leverage has credible basis.

### LEVEL 4

Red Team + cross-examination completed.

### LEVEL 5

No unresolved P0 issues and enough evidence exists for later selection.

An opportunity can be mature but unattractive.

Maturity does not mean “best.”

---

# 67. Opportunity Readiness Gate

Before an opportunity is marked `Selection Ready`, require:

```text
Validated problem

Defined user

Workflow understood

Gap investigated

Strongest competitor known

Non-AI baseline known

AI leverage analyzed

Measurement plausible

Trust risk documented

Feasibility plausible

P0 challenges resolved

Limitations documented
```

---

# 68. Opportunity Promotion

The Director may promote an opportunity to:

```text
SELECTION READY
```

when enough evidence exists for later decision-making.

This does not mean:

> selected.

---

# 69. Opportunity Demotion

New evidence may move:

```text
Selection Ready
→
Requires Validation
```

Example:

> new competitor discovered.

The Opportunity Map must be updateable.

---

# 70. Version Tracking

Each Opportunity Record should include:

```text
VERSION:

LAST UPDATED:

CHANGE SUMMARY:
```

Important changes should note:

```text
Previous status:

New status:

Reason:
```

---

# 71. Decision History

Where helpful, link to the Director's decision ledger.

Example:

```text
DECISION:
D-014

Effect:
Merged OPP-006 into OPP-002.
```

---

# 72. Research Limitations

Every Opportunity Map should include:

```text
## Research Limitations
```

Possible limitations:

- limited Arabic evidence;
    
- missing private-product data;
    
- unavailable app reviews;
    
- limited scholar review;
    
- geographic gaps;
    
- small behavioral sample.
    

Do not present the map as exhaustive.

---

# 73. Search-Coverage Transparency

For market-sensitive opportunities, include:

```text
SEARCH COVERAGE:

Languages:

Regions:

Product sources:

Academic sources:

GitHub searched:

Known gaps:
```

This helps interpret absence claims.

---

# 74. Opportunity Map Must Remain Evidence-First

Do not write:

> “This would be an amazing project.”

Write:

> `[DIRECTOR SYNTHESIS]` This opportunity combines strong problem evidence, a partially unresolved workflow gap, measurable verification outcomes, and manageable trust risk.

Keep language analytical.

---

# 75. Director Synthesis

Each Opportunity should contain a concise Director synthesis.

Recommended structure:

```text
[DIRECTOR SYNTHESIS]

What appears true:

...

What remains uncertain:

...

Why the opportunity matters:

...

Why it may fail:

...

Current research status:

...
```

---

# 76. Strongest Reason to Pursue

Include:

```text
## Strongest Reason to Pursue
```

This should be evidence-based.

Example:

> The same verification workflow failure appears independently across content-creator research and trust analysis, while current systems solve retrieval but not claim-level provenance.

---

# 77. Strongest Reason Not to Pursue

Include:

```text
## Strongest Reason Not to Pursue
```

Example:

> Users may already consider current manual verification acceptable, and behavioral evidence for switching remains limited.

This forces balanced synthesis.

---

# 78. Opportunity Comparison Should Not Become Advocacy

When comparing opportunities:

do not describe one in rich language and another superficially.

Use the same schema.

The structure should reduce presentation bias.

---

# 79. No Winner During Opportunity Mapping

Do not label:

```text
#1
Top Idea
Winner
Best
```

The Opportunity Map's purpose is to prepare for later prioritization.

Selection requires a separate decision process.

---

# 80. Later Selection Compatibility

The schema should preserve dimensions likely to matter later:

- problem importance;
    
- AI value;
    
- reliability;
    
- measurable impact;
    
- feasibility;
    
- differentiation;
    
- UX;
    
- operational realism;
    
- hackathon fit.
    

But it should not collapse them into a score yet.

---

# 81. Hackathon Alignment

Once problem validity is established, record relevant Islamic AI Challenge alignment.

Possible fields:

```text
LIKELY TRACK:

TRACK FIT:
Strong / Moderate / Weak

RELEVANT SUCCESS CRITERION:

WHY:
```

Track fit must not drive problem discovery backward.

---

# 82. Challenge Track Fit

If the opportunity could fit several tracks, record:

```text
PRIMARY TRACK:

SECONDARY TRACK:

WHY PRIMARY:
```

Do not force a track before understanding the product.

---

# 83. Innovation Interpretation

Record innovation as:

> what changes for the user or system,

not:

> what technologies are fashionable.

Potential innovation may come from:

- workflow;
    
- source integrity;
    
- user segment;
    
- interaction model;
    
- cross-domain transfer;
    
- evaluation methodology.
    

---

# 84. Operational Realism

Include:

```text
REQUIRES:

Source maintenance:
Yes / No

Scholar review:
Yes / No / Conditional

Human moderation:
Yes / No

Frequent model evaluation:
Yes / No

Corpus updates:
Yes / No
```

This helps distinguish demo feasibility from sustainable product viability.

---

# 85. Dependency Register

For important opportunities record:

```text
DEPENDENCY ID:

DEPENDENCY:

TYPE:
Data / API / Expert / Legal / Technical / Product

STATUS:

IMPACT IF UNAVAILABLE:
```

---

# 86. Blocking Dependency

Use:

```text
[BLOCKING DEPENDENCY]
```

where progress cannot continue without resolution.

A flashy idea with a blocking dependency should not appear selection-ready.

---

# 87. Risk Register Linkage

Where needed, record:

```text
RISK ID:

RISK:

LIKELIHOOD:

SEVERITY:

DETECTABILITY:

MITIGATION:
```

Do not overbuild a risk register for low-risk opportunities.

---

# 88. Opportunity Map File

The main artifact should be:

```text
/synthesis/opportunity-map.md
```

The Research Director owns this file.

Individual detailed opportunity records may live in a future directory only if defined by orchestration.

Do not create extra directories independently.

---

# 89. Recommended Opportunity Map Structure

```text
# Islamic AI Challenge — Opportunity Map

## 1. Executive Research Summary

## 2. Scope

## 3. User Groups

## 4. Recurring Jobs to Be Done

## 5. Root Problem Clusters

## 6. Opportunity Summary Table

## 7. Detailed Opportunities

### OPP-001
...

### OPP-002
...

## 8. Cross-Agent Convergence

## 9. Important Disagreements

## 10. AI-Unnecessary Problems

## 11. Already-Solved Problems

## 12. Disconfirmed Opportunities

## 13. High-Risk Opportunities

## 14. Cross-Domain Lessons

## 15. Open Questions

## 16. Research Limitations

## 17. Selection-Ready Opportunities
```

The last section should contain no ranking.

---

# 90. Selection-Ready Section

Use:

```text
## Selection-Ready Opportunities
```

Each entry should include:

```text
OPPORTUNITY ID:

WHY READY:

UNRESOLVED LIMITATIONS:

P0 STATUS:

MATURITY:
```

Do not choose among them.

---

# 91. Disconfirmed Section

Use:

```text
## Disconfirmed / Discontinued Opportunities
```

Include why each failed.

Examples:

```text
Problem not supported

Strong competitor found

AI unnecessary

Trust risk excessive

Data unavailable

Unable to measure benefit
```

---

# 92. Open Question Priority

Open questions should use:

```text
P0 — Could change whether opportunity survives

P1 — Could significantly change scope

P2 — Important for later design

P3 — Optional
```

Selection-ready opportunities should generally have no unresolved P0 questions.

---

# 93. Opportunity Map Quality Check

Before finalizing, the Director should ask:

```text
Does every opportunity have a real user?

Does every opportunity link to validated problems?

Is current workflow understood?

Were competitors searched?

Is the gap clearly stated?

Was AI necessity tested?

Is a non-AI alternative visible?

Is measurement plausible?

Are trust risks explicit?

Did Red Team review occur?

Did cross-examination occur?

Are open questions visible?

Are negative findings preserved?

Are confidence labels justified?
```

---

# 94. Bias Audit

Before publishing the map ask:

- Did the most verbose agent influence the map disproportionately?
    
- Did one source dominate several opportunities?
    
- Are Arabic-language findings underrepresented?
    
- Are AI-heavy ideas receiving unfair attention?
    
- Are visually impressive ideas being favored?
    
- Are weak problems being protected because they have good demos?
    
- Are trust concerns being minimized?
    

Record material bias risks.

---

# 95. Comparative Fairness

Every opportunity should receive comparable scrutiny.

Do not perform deep competitor search for one idea and shallow search for another while treating confidence equally.

Research depth should be visible.

---

# 96. No Artificial Opportunity Count

Do not force:

> Top 10 opportunities

if only four survive.

Do not remove opportunities merely to reach a smaller number unless evidence supports elimination.

---

# 97. No Artificial Diversity

Do not intentionally include one idea from every hackathon track merely for variety.

The map should reflect evidence.

---

# 98. Preserve Unexpected Findings

If research reveals a strong problem outside the initially expected categories, preserve it.

Do not discard it because it differs from early assumptions.

---

# 99. Definition of Done

The Opportunity Map is complete when another informed reviewer can understand:

**Who the important users are.**

**What they are trying to accomplish.**

**What problems are strongly evidenced.**

**What problems were disproved.**

**What existing products already solve.**

**What gaps remain.**

**Where AI has strong, weak, or unnecessary leverage.**

**What non-AI alternatives exist.**

**How value could be measured.**

**What Islamic trust and boundary risks apply.**

**What is technically and operationally feasible.**

**What survived Red Team and cross-examination.**

**What remains uncertain.**

**Which opportunities are mature enough for a later selection process.**

If these cannot be determined from the map, the synthesis is incomplete.

---

# 100. Final Principle

The Opportunity Map exists to turn a large body of research into a decision-ready landscape without pretending the research is more certain than it is.

Its objective is not:

> “Produce a list of impressive ideas.”

Its objective is:

> **Show, in one traceable structure, which human problems are real, which gaps remain, where AI can responsibly create value, what evidence supports those conclusions, and what could still prove them wrong.**

Map problems before products.

Show evidence before excitement.

Expose alternatives.

Expose uncertainty.

Preserve failed ideas.

Keep trust visible.

Keep AI accountable.

Do not rank until the evidence is ready.

And make every later decision traceable back to the research that justified it.