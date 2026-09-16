## Islamic AI Challenge — Evidence Standard

This document defines the minimum evidence quality required for research findings produced by the agent research lab.

It applies to:

- problem discovery;
    
- user pain validation;
    
- workflow reconstruction;
    
- competitor analysis;
    
- Islamic trust and source analysis;
    
- technical feasibility claims;
    
- AI opportunity claims;
    
- market observations;
    
- final opportunity synthesis.
    

This document supplements:

- `AGENTS.md`
    
- `research-protocol/source-policy.md`
    

The purpose of this standard is to prevent attractive hypotheses from becoming accepted conclusions without sufficient evidence.

---

# 1. Core Principle

A research claim becomes more credible when it is supported by:

**relevant evidence + independent corroboration + clear context + disconfirmation testing**

The objective is not to collect the maximum number of sources.

The objective is to determine:

> How strongly does the available evidence justify this conclusion?

---

# 2. Evidence Is Not Binary

Evidence should not be treated as simply:

> proven / not proven

Research often contains degrees of confidence.

Every important conclusion should instead be evaluated according to:

- relevance;
    
- directness;
    
- reliability;
    
- independence;
    
- consistency;
    
- representativeness;
    
- freshness;
    
- methodological strength;
    
- contradiction;
    
- remaining uncertainty.
    

---

# 3. Evidence Objects

Important evidence should be represented as an individual **Evidence Object**.

Recommended structure:

```text
EVIDENCE ID:

CLAIM SUPPORTED:

SOURCE TYPE:

SOURCE:

URL:

DATE:

TARGET USER / POPULATION:

GEOGRAPHY:

LANGUAGE:

DIRECT OR INDIRECT:

PRIMARY OR SECONDARY:

KEY EVIDENCE:

LIMITATIONS:

CONTRADICTING EVIDENCE:

STRENGTH:
Strong / Moderate / Weak

CONFIDENCE IN INTERPRETATION:
High / Medium / Low
```

Evidence IDs should follow a consistent naming convention.

Example:

```text
EVID-001
EVID-002
EVID-003
```

---

# 4. Evidence Strength Is Claim-Specific

A source may be strong evidence for one claim and weak evidence for another.

Example:

An app review stating:

> “I cannot find where this answer came from.”

may be:

**Strong evidence** that this specific user experienced a source-transparency problem.

It is:

**Weak evidence** that all Muslims experience the same problem.

Always evaluate evidence relative to the exact claim.

---

# 5. Evidence Strength Levels

Use three primary evidence-strength labels.

## STRONG

Evidence is considered strong when most of the following are true:

- directly addresses the claim;
    
- comes from a credible or appropriate source;
    
- is traceable;
    
- contains sufficient context;
    
- is independently verifiable;
    
- has limited ambiguity;
    
- is current enough for the claim;
    
- is methodologically sound where methodology matters;
    
- is corroborated where appropriate.
    

Examples may include:

- direct official documentation confirming a product feature;
    
- an original scholarly source establishing a scholar's stated position;
    
- repeated detailed user complaints across independent platforms;
    
- a well-designed academic study directly investigating the issue;
    
- reproducible testing of a technical capability.
    

---

## MODERATE

Evidence is moderate when it supports the claim but has meaningful limitations.

Examples:

- a small but relevant academic study;
    
- several user reports from one platform;
    
- reliable secondary reporting;
    
- product documentation without independent validation;
    
- an older study that may still apply;
    
- a detailed expert opinion without empirical testing.
    

Moderate evidence is useful but should generally be corroborated before supporting major conclusions.

---

## WEAK

Evidence is weak when one or more major limitations exist.

Examples:

- a single anecdote;
    
- an anonymous unsupported claim;
    
- a search snippet;
    
- promotional marketing language;
    
- an undated blog;
    
- a social post without context;
    
- speculative commentary;
    
- an AI-generated answer;
    
- copied information with an unclear original source.
    

Weak evidence may justify further investigation.

It should rarely determine a major conclusion by itself.

---

# 6. Evidence Confidence Is Different from Evidence Strength

Evidence strength concerns the source and its relationship to the claim.

Confidence concerns the researcher's certainty in the interpretation.

Example:

A strong source may contain ambiguous language.

The source strength may be:

> Strong

while interpretation confidence may be:

> Medium

Always keep these concepts separate.

---

# 7. Major Claims Require Higher Evidence

Not every statement requires the same level of validation.

### Low-impact claim

Example:

> Product X has a mobile application.

A single official source may be sufficient.

### Major research claim

Example:

> New Muslims struggle significantly to distinguish religious teachings from cultural practices.

This requires stronger validation.

Major claims should ideally involve:

- multiple independent sources;
    
- more than one evidence type;
    
- disconfirmation research;
    
- explicit limitations;
    
- defined population and context.
    

---

# 8. Problem Validation Standard

A problem should not be considered meaningfully validated merely because an agent can imagine it.

A promising problem should ideally establish:

```text
USER:
Who experiences it?

TASK:
What are they trying to accomplish?

WORKFLOW:
What do they currently do?

PAIN:
Where does the problem occur?

EVIDENCE:
How do we know?

CONSEQUENCE:
Why does it matter?

CURRENT SOLUTION:
How is it handled today?

GAP:
What remains unresolved?

DISCONFIRMATION:
What evidence argues against its importance?

CONFIDENCE:
How certain are we?
```

---

# 9. Minimum Problem Evidence

Before a problem is promoted into a serious Problem Card, aim to obtain at least:

### A. One direct problem signal

Examples:

- detailed user complaint;
    
- workflow observation;
    
- repeated user question;
    
- interview response;
    
- direct expert statement;
    
- usability problem.
    

### B. One independent corroborating signal

Examples:

- another platform;
    
- another user population;
    
- academic research;
    
- product limitation;
    
- institutional observation.
    

### C. Existing-solution research

Determine whether the problem is already adequately solved.

### D. Disconfirmation search

Actively investigate whether the problem may be less important than initially assumed.

This is a quality guideline, not a quota.

One exceptionally strong source may sometimes provide more information than many weak sources.

---

# 10. Strong Problem Validation

A problem becomes particularly credible when several independent evidence layers agree.

For example:

```text
USER REPORTS
+
WORKFLOW EVIDENCE
+
ACADEMIC RESEARCH
+
EXISTING PRODUCT LIMITATIONS
+
EXPERT OBSERVATION
```

Not every problem requires every layer.

But convergence across different evidence types should increase confidence.

---

# 11. Evidence Triangulation

Triangulation means verifying a conclusion through different evidence paths.

Example:

### Hypothesis

Islamic content creators spend significant time manually verifying references.

### Possible triangulation

**User evidence**  
Creators describe repeated verification work.

**Workflow evidence**  
Observed workflow contains multiple manual search and comparison steps.

**Product evidence**  
Existing content-generation tools provide weak source traceability.

**Academic/expert evidence**  
Research highlights reliability problems in generative AI religious content.

Together these provide stronger validation than any one source alone.

---

# 12. Source Independence

Multiple sources must not automatically be counted as independent.

Investigate whether they share the same upstream origin.

Examples of non-independent evidence:

- ten websites copying one news article;
    
- several posts quoting the same study;
    
- multiple accounts reposting one complaint;
    
- different articles repeating one vendor press release.
    

Label these as:

> `DEPENDENT EVIDENCE CLUSTER`

when relevant.

---

# 13. Evidence Diversity

Strong research should avoid dependence on one evidence class.

For user problems, useful evidence categories include:

```text
USER SIGNAL

WORKFLOW SIGNAL

EXPERT SIGNAL

ACADEMIC SIGNAL

PRODUCT SIGNAL

TECHNICAL SIGNAL

BEHAVIORAL SIGNAL
```

Diversity improves confidence because different evidence types fail in different ways.

---

# 14. Direct vs Indirect Evidence

### Direct Evidence

Directly observes or documents the phenomenon.

Example:

> A user explains that verifying references takes 45 minutes during their normal workflow.

### Indirect Evidence

Suggests the phenomenon without observing it directly.

Example:

> A report states that Islamic content verification is important.

Direct evidence should generally receive more weight for workflow and user-problem claims.

Indirect evidence remains useful for context.

---

# 15. Primary vs Secondary Evidence

Primary evidence originates close to the phenomenon.

Examples:

- original scholarly text;
    
- direct user review;
    
- product documentation;
    
- interview transcript;
    
- original research paper.
    

Secondary evidence interprets or summarizes another source.

Examples:

- article discussing a paper;
    
- blog summarizing a fatwa;
    
- review describing product documentation.
    

Prefer primary evidence where reasonably accessible.

---

# 16. Evidence Freshness

Ask:

> Could this fact have materially changed?

Fresh evidence is particularly important for:

- AI capabilities;
    
- product features;
    
- active competitors;
    
- pricing;
    
- APIs;
    
- app quality;
    
- user interface;
    
- current community behavior;
    
- repository status.
    

Older evidence may remain appropriate for:

- historical facts;
    
- established scholarship;
    
- foundational research;
    
- stable user behaviors.
    

Always consider time context.

---

# 17. Population Fit

Evidence must match the population being discussed.

Do not generalize evidence collected from:

> English-speaking Muslim university students in the United Kingdom

into:

> Muslims globally

without additional support.

Record relevant dimensions such as:

- age;
    
- language;
    
- location;
    
- education;
    
- role;
    
- religious knowledge level;
    
- convert status;
    
- profession.
    

Use precise language.

---

# 18. Geographic Fit

Research conclusions should preserve geography when relevant.

Example:

Prefer:

> “Several Saudi Arabic-speaking users reported…”

rather than:

> “Muslims report…”

unless broader evidence exists.

Geographic differences may materially affect:

- source preferences;
    
- legal questions;
    
- language;
    
- educational systems;
    
- cultural practices;
    
- digital products.
    

---

# 19. Language Fit

A problem discovered in one language community may not exist in another.

Agents must record:

- language of evidence;
    
- language of user;
    
- language of product;
    
- translation limitations.
    

Do not assume Arabic and English Islamic information ecosystems behave identically.

---

# 20. Frequency Evidence

A problem can be:

- severe but rare;
    
- common but minor;
    
- both common and severe;
    
- neither.
    

Separate frequency from severity.

Useful frequency evidence may include:

- repeated questions;
    
- recurring reviews;
    
- support-ticket patterns;
    
- survey prevalence;
    
- repeated workflow occurrence.
    

Avoid assigning numerical frequency without evidence.

---

# 21. Severity Evidence

Severity concerns the consequence of the problem.

Possible consequences include:

- incorrect religious information;
    
- wasted time;
    
- user confusion;
    
- inability to complete a task;
    
- loss of trust;
    
- accessibility barriers;
    
- reputational damage;
    
- need for expert correction.
    

Agents must distinguish evidence of severity from assumptions about severity.

---

# 22. Recurrence

Recurring problems generally deserve more attention than one-time inconveniences.

Ask:

- Does the user encounter this daily?
    
- Weekly?
    
- Only during special situations?
    
- Once in their lifetime?
    
- During every research task?
    

Frequency should be documented where evidence permits.

---

# 23. Workflow Evidence

Workflow claims should ideally capture:

```text
TRIGGER:

USER GOAL:

STEP 1:

STEP 2:

STEP 3:

FRICTION POINT:

WORKAROUND:

RESULT:

TIME / EFFORT WHERE KNOWN:
```

Prefer actual observed or reported workflows over imagined workflows.

---

# 24. Do Not Invent Workflow Steps

If only part of the user's workflow is known, label missing portions:

> `[WORKFLOW GAP]`

Do not invent logical-looking steps to make the workflow complete.

---

# 25. Existing-Solution Evidence

Every serious problem must undergo solution-landscape research.

For each relevant solution, gather evidence about:

- target user;
    
- core workflow;
    
- supported features;
    
- limitations;
    
- adoption;
    
- user complaints;
    
- project status;
    
- technical approach where relevant.
    

Avoid claiming:

> “Nothing solves this.”

unless research genuinely supports it.

---

# 26. Gap Evidence

A gap exists when evidence shows:

1. users have a meaningful need;
    
2. solutions exist or workarounds are used;
    
3. current approaches leave an important requirement unresolved.
    

A gap should not be inferred merely because a product lacks a feature.

Ask:

> Do users actually care about the missing capability?

---

# 27. Feature Gap vs Problem Gap

These are different.

### Feature Gap

> Existing application does not provide voice search.

### Problem Gap

> Users in the target population cannot efficiently use text input and repeatedly fail to complete the search task.

Do not confuse missing features with meaningful unmet needs.

---

# 28. Disconfirming Evidence Is Mandatory

For every serious hypothesis, actively search for evidence that would weaken it.

Examples:

- existing products solve it well;
    
- users report satisfaction;
    
- workflow is easier than assumed;
    
- problem occurs rarely;
    
- target users reject AI assistance;
    
- simpler solutions already exist.
    

Record disconfirming evidence even if it hurts the idea.

---

# 29. Disconfirmation Template

Use:

```text
HYPOTHESIS:

WHAT WOULD MAKE IT FALSE OR UNIMPORTANT?

SEARCH PERFORMED:

EVIDENCE AGAINST:

EVIDENCE FOR:

CURRENT ASSESSMENT:

REMAINING UNCERTAINTY:
```

---

# 30. Failure to Find Contradiction Is Not Proof

If no contradictory evidence is found, do not automatically conclude the hypothesis is true.

Possible reasons include:

- poor search terms;
    
- limited accessible data;
    
- niche population;
    
- language barrier;
    
- publication bias.
    

Write:

> “No meaningful contradictory evidence was identified in the completed search.”

rather than:

> “There is no contradictory evidence.”

---

# 31. Contradiction Handling

When credible evidence conflicts, classify the conflict.

Possible categories:

### Population Difference

The evidence concerns different user groups.

### Time Difference

The product or behavior changed.

### Context Difference

The same problem behaves differently in another situation.

### Methodological Difference

Studies measured different things.

### Genuine Uncertainty

Evidence remains unresolved.

Document the reason where possible.

---

# 32. Contradiction Template

```text
CONTRADICTION ID:

CLAIM:

SOURCE A:

SOURCE B:

TYPE OF CONFLICT:

POSSIBLE EXPLANATION:

CAN IT BE RESOLVED?

CURRENT INTERPRETATION:

CONFIDENCE:
```

---

# 33. Confidence Levels

Every major conclusion should have a confidence label.

## HIGH CONFIDENCE

Use when:

- several strong independent sources agree;
    
- evidence directly addresses the claim;
    
- contradictory evidence is weak or well explained;
    
- important context is understood.
    

## MEDIUM CONFIDENCE

Use when:

- relevant evidence exists;
    
- some corroboration exists;
    
- meaningful uncertainty remains;
    
- population or methodology may be limited.
    

## LOW CONFIDENCE

Use when:

- evidence is sparse;
    
- mostly anecdotal;
    
- indirect;
    
- contradictory;
    
- poorly matched to the population;
    
- dependent on assumptions.
    

Confidence is not enthusiasm.

---

# 34. Confidence Should Be Claim-Level

Do not assign one confidence level to an entire report.

Different conclusions may have different confidence.

Example:

```text
Problem exists:
High

Problem is widespread:
Medium

Problem affects Saudi users:
Low

AI is the best solution:
Low
```

This is more informative than:

> Overall confidence: High

---

# 35. Confidence Should Decrease When Scope Expands

Evidence may strongly support a narrow claim.

Example:

> English-speaking converts report confusion around Islamic terminology.

Expanding the claim to:

> Converts worldwide cannot understand Islamic terminology.

should lower confidence unless additional evidence exists.

Broader claims require broader evidence.

---

# 36. No Arbitrary Numeric Confidence

Do not write:

> 87% confident

unless the number comes from a defined statistical or probabilistic method.

Use:

- High
    
- Medium
    
- Low
    

for qualitative research confidence.

---

# 37. Evidence Saturation

Research reaches saturation when additional investigation produces little materially new information.

Signs include:

- new sources repeat established themes;
    
- no major new competitor appears;
    
- user complaints become repetitive;
    
- contradictory searches return similar results;
    
- the workflow is consistently documented.
    

Saturation is not the same as certainty.

---

# 38. Saturation Rule

Agents may stop a research branch when:

1. core questions are answered;
    
2. evidence is sufficiently diverse;
    
3. major contradiction searches have been performed;
    
4. two consecutive search iterations add no material insight.
    

Record:

> `[EVIDENCE SATURATION REACHED]`

where useful.

---

# 39. Saturation Exceptions

Continue research beyond apparent saturation when:

- the claim is high risk;
    
- Islamic correctness is involved;
    
- sources conflict;
    
- evidence is dominated by one platform;
    
- important populations remain unrepresented;
    
- current information may have changed recently.
    

---

# 40. User Complaint Sampling

When analyzing reviews or discussions, avoid cherry-picking.

Agents should record where practical:

```text
PLATFORM:

SEARCH / SELECTION METHOD:

NUMBER REVIEWED:

NUMBER RELEVANT:

RECURRING THEMES:

POSITIVE THEMES:

NEGATIVE THEMES:

LIMITATIONS:
```

Do not only copy the most dramatic comments.

---

# 41. Qualitative Theme Threshold

One complaint creates a lead.

Several independent similar complaints create a pattern.

A repeated pattern across multiple environments creates stronger evidence.

Avoid artificial thresholds such as:

> five complaints = proven problem.

Context matters.

---

# 42. Quantitative Evidence

Quantitative evidence should preserve:

- denominator;
    
- sample;
    
- population;
    
- measurement method;
    
- date;
    
- uncertainty where reported.
    

Avoid claims such as:

> “80% struggle with this”

without knowing:

> 80% of whom?

---

# 43. Surveys

Before trusting survey evidence, examine:

- sample size;
    
- recruitment;
    
- representativeness;
    
- wording;
    
- response bias;
    
- geography;
    
- language.
    

A poll on a social-media account is not equivalent to a representative population survey.

---

# 44. Interviews

Interview evidence is valuable for discovering:

- workflows;
    
- motivations;
    
- emotional pain;
    
- terminology;
    
- workarounds.
    

It is weaker for establishing population prevalence unless the interview sample is appropriately designed.

Use interviews for depth.

Use broader evidence for frequency.

---

# 45. Academic Evidence

For academic studies, capture:

```text
RESEARCH QUESTION:

POPULATION:

N:

METHOD:

MAIN FINDING:

LIMITATIONS:

RELEVANCE TO OUR CLAIM:
```

Do not use the abstract's conclusion without understanding what was actually measured.

---

# 46. Statistical Significance Is Not Practical Importance

A statistically significant difference may have little real-world importance.

Where relevant, distinguish:

- statistical significance;
    
- effect size;
    
- practical impact.
    

Do not overstate academic results.

---

# 47. Correlation vs Causation

Do not convert:

> X is associated with Y

into:

> X causes Y

unless the research design supports causal inference.

---

# 48. Vendor Evidence

Official product claims should be labeled:

> `[VENDOR CLAIM]`

when they concern performance, quality, accuracy, scale, or impact and have not been independently verified.

Example:

```text
[VENDOR CLAIM]
Product X reports 98% accuracy on its internal benchmark.
```

---

# 49. Technical Evidence

Technical feasibility claims should preferably be supported by:

- official model documentation;
    
- API documentation;
    
- benchmarks;
    
- papers;
    
- reproducible experiments;
    
- GitHub repositories;
    
- actual prototypes.
    

Avoid statements such as:

> “AI can easily do this.”

Replace with evidence.

---

# 50. Feasibility Evidence

For a technical opportunity, investigate:

```text
INPUT DATA AVAILABLE?

MODEL CAPABILITY EXISTS?

RETRIEVAL POSSIBLE?

LATENCY ACCEPTABLE?

COST PLAUSIBLE?

EVALUATION POSSIBLE?

RELIABILITY CONTROLS POSSIBLE?

DEMO IMPLEMENTABLE?

KNOWN FAILURE MODES?
```

Unanswered questions should be recorded.

---

# 51. AI Opportunity Evidence

An AI opportunity requires more than a problem plus an LLM.

Agents should establish:

### Task suitability

Does the task involve something AI is meaningfully good at?

### Value

Does AI reduce an important pain?

### Advantage

Why is AI better than simpler software?

### Risk

What new failure modes does AI introduce?

### Measurement

Can its benefit be tested?

---

# 52. Non-AI Baseline

Every serious AI opportunity should include a non-AI baseline.

Examples:

- keyword search;
    
- database lookup;
    
- manual workflow;
    
- rule-based filtering;
    
- static educational pages;
    
- forms;
    
- deterministic software.
    

Ask:

> What would we build if generative AI did not exist?

The AI approach should demonstrate a meaningful advantage.

---

# 53. Benchmark Against Current Workflow

The most useful comparison is often not:

> our AI vs another AI

but:

> current user workflow vs proposed workflow.

Potential measures:

```text
TIME

NUMBER OF STEPS

ERROR RATE

CITATION ACCURACY

TASK SUCCESS

EXPERT REVIEW LOAD

USER COMPREHENSION

SOURCE TRACEABILITY
```

---

# 54. Religious Reliability Evidence

Claims involving Islamic correctness require stronger evidence standards.

The evidence should preserve:

- source attribution;
    
- scope;
    
- context;
    
- disagreement where relevant;
    
- confidence;
    
- escalation need.
    

Do not evaluate religious correctness using popularity metrics.

---

# 55. Islamic Safety Claims

If an opportunity claims:

> “Our system is safer”

the claim must be measurable.

Possible measures include:

- unsupported claim rate;
    
- citation correctness;
    
- citation coverage;
    
- source retrieval accuracy;
    
- refusal accuracy;
    
- disagreement-handling accuracy;
    
- expert review outcomes.
    

Avoid vague safety language.

---

# 56. Evidence for Scholarly Disagreement

Do not label a topic disputed merely because two internet pages differ.

Seek credible evidence of recognized scholarly disagreement.

Likewise, do not label a topic consensus merely because multiple sites agree.

Follow `source-policy.md`.

---

# 57. Evaluation Sets

When a technical project eventually emerges, research agents should identify possible evaluation cases.

Useful categories may include:

- straightforward questions;
    
- ambiguous questions;
    
- conflicting-source questions;
    
- out-of-scope requests;
    
- multilingual inputs;
    
- misleading premises;
    
- citation requests;
    
- context-dependent questions.
    

These may later become benchmark datasets.

---

# 58. Edge Cases Are Evidence

A system may appear excellent on normal cases and fail dangerously on edge cases.

Agents should record known high-risk cases.

Example:

```text
NORMAL CASE:
Definition of a general Islamic term.

EDGE CASE:
Personal divorce ruling requiring factual circumstances.
```

Edge-case failure may materially affect opportunity viability.

---

# 59. Evidence Against Automation

A valid conclusion may be:

> This workflow should not be fully automated.

Evidence supporting this may include:

- high consequence of error;
    
- deeply contextual judgments;
    
- lack of reliable source coverage;
    
- need for human discretion;
    
- unclear responsibility.
    

Such findings can still inspire tools that assist humans rather than replace them.

---

# 60. Human-in-the-Loop Evidence

When proposing human review, identify:

- who reviews;
    
- at what point;
    
- why;
    
- what information they receive;
    
- what happens if review is unavailable.
    

Do not use:

> “human in the loop”

as a vague safety phrase.

---

# 61. Measurement Quality

A good metric should be:

- relevant;
    
- observable;
    
- reproducible;
    
- understandable;
    
- tied to user value.
    

Bad metric:

> number of AI responses generated.

Better metric:

> percentage of factual claims with correctly traceable sources.

---

# 62. Proxy Metrics

Sometimes direct impact cannot be measured during a hackathon.

Proxy metrics are acceptable when clearly identified.

Example:

True long-term impact:

> improved learning retention over six months.

Hackathon proxy:

> comprehension accuracy immediately after interaction.

Label proxy metrics honestly.

---

# 63. Avoid Vanity Metrics

Examples of weak evidence:

- number of features;
    
- number of models;
    
- number of database records;
    
- number of screens;
    
- number of sources ingested.
    

These may describe the system.

They do not necessarily demonstrate value.

---

# 64. Before-and-After Evidence

Strong opportunities often support a clear comparison.

Example:

```text
BEFORE:
Researcher manually checks 12 pages.

AFTER:
System retrieves 5 relevant passages with source provenance.

MEASURE:
Time to locate acceptable evidence.
```

Do not invent the performance improvement.

It must eventually be tested.

---

# 65. Evidence for Adoption

A useful solution also needs realistic adoption.

Research may examine:

- existing user habits;
    
- switching costs;
    
- trust;
    
- device access;
    
- willingness to use AI;
    
- institutional integration;
    
- language preferences.
    

A technically strong solution may fail if adoption barriers are ignored.

---

# 66. Behavioral Evidence Beats Stated Preference When Available

What users say they want and what they actually do may differ.

Prefer observed behavior where possible.

Example:

Stated preference:

> “I want detailed citations.”

Behavioral evidence:

> users consistently open and inspect cited sources.

Both are useful.

Behavior may provide stronger validation.

---

# 67. Negative Findings Must Be Preserved

If research weakens an idea, record it.

Examples:

```text
PROBLEM APPEARS LOW FREQUENCY

EXISTING PRODUCT ALREADY SOLVES CORE NEED

AI ADDS LITTLE VALUE

USER GROUP TOO NARROW

RELIABILITY RISK TOO HIGH
```

Negative evidence prevents repeated wasted work.

---

# 68. Evidence Conflict with Team Expectations

Agents must never modify evidence because it conflicts with the team's preferred direction.

If evidence indicates:

> the idea is weak

report that conclusion.

Research integrity takes precedence over enthusiasm.

---

# 69. Opportunity Promotion Gates

A problem should normally pass several gates before reaching final opportunity synthesis.

## Gate 1 — Reality

Is there credible evidence that the problem exists?

## Gate 2 — User

Is the affected user clearly identified?

## Gate 3 — Workflow

Do we understand where the pain occurs?

## Gate 4 — Importance

Is there evidence that the pain matters?

## Gate 5 — Gap

Are current solutions insufficient?

## Gate 6 — AI Relevance

Could AI create meaningful value?

## Gate 7 — Reliability

Could the problem be addressed responsibly?

## Gate 8 — Measurement

Can improvement be demonstrated?

Failure at one gate does not necessarily permanently eliminate an opportunity.

It identifies what remains unresolved.

---

# 70. Opportunity Status Labels

Use:

### `VALIDATED`

Strong enough for serious solution exploration.

### `PROMISING`

Good evidence exists but important questions remain.

### `UNVALIDATED`

Interesting hypothesis with insufficient evidence.

### `WEAK`

Evidence suggests low value or weak fit.

### `REJECTED`

Strong evidence indicates it should not currently proceed.

These statuses must be justified.

---

# 71. Do Not Rank Too Early

A `VALIDATED` problem is not automatically the best project.

Validation only means:

> the problem appears real and worth considering.

Final selection occurs later using:

- evidence;
    
- impact;
    
- AI leverage;
    
- hackathon fit;
    
- feasibility;
    
- differentiation;
    
- trust;
    
- demonstrability.
    

---

# 72. Problem Card Confidence

Every Problem Card should contain confidence assessments for separate dimensions.

Recommended:

```text
Problem existence:
High / Medium / Low

Problem severity:
High / Medium / Low

Problem frequency:
High / Medium / Low

Current-solution gap:
High / Medium / Low

AI opportunity:
High / Medium / Low

Measurability:
High / Medium / Low

Overall evidence maturity:
High / Medium / Low
```

Avoid collapsing them prematurely.

---

# 73. Evidence Maturity Levels

Use the following optional maturity framework.

## Level 0 — Speculation

Idea exists but evidence is absent.

## Level 1 — Signal

One or more relevant signals exist.

## Level 2 — Pattern

Independent evidence suggests recurrence.

## Level 3 — Validated Problem

Multiple evidence types establish the problem and gap.

## Level 4 — Solution-Ready

Problem, workflow, gap, user, measurable outcome, and likely intervention point are sufficiently understood for solution design.

Agents should not imply Level 4 when research remains at Level 1.

---

# 74. Evidence Ledger

Maintain an evidence ledger for major research tracks where practical.

Example:

```text
| ID | Claim | Source | Type | Strength | Supports / Contradicts |
|----|-------|--------|------|----------|------------------------|
| EVID-001 | Users struggle with citations | App reviews | User | Moderate | Supports |
| EVID-002 | Product X provides citations | Official docs | Product | Strong | Contradicts gap |
```

The ledger helps identify:

- overreliance on one evidence type;
    
- unsupported conclusions;
    
- contradictions;
    
- duplicate sources.
    

---

# 75. Claim-to-Evidence Mapping

Every major conclusion in final synthesis should be traceable to evidence IDs.

Example:

```text
CLAIM:
English-speaking converts struggle with unfamiliar Arabic terminology.

SUPPORT:
EVID-014
EVID-019
EVID-027

CONTRADICT:
EVID-031

CONFIDENCE:
Medium
```

---

# 76. No Citation Dumping

Do not attach ten citations to a sentence without understanding them.

Every source must contribute something meaningful.

Citation volume does not compensate for weak reasoning.

---

# 77. Evidence Summaries Must Preserve Limitations

Bad:

> Research proves converts struggle to access Islamic knowledge.

Better:

> Two small studies and recurring reports from English-speaking converts indicate difficulty navigating terminology and source credibility; broader geographic validation remains limited.

The second version is more scientifically useful.

---

# 78. Avoid Absolute Language

Use language proportional to evidence.

Prefer:

- suggests;
    
- indicates;
    
- recurring;
    
- observed;
    
- appears;
    
- within the sampled users;
    
- according to;
    
- evidence supports.
    

Use words like:

- proves;
    
- always;
    
- never;
    
- everyone;
    
- universally;
    

only when the evidence genuinely justifies them.

---

# 79. Strong Evidence Can Still Be Narrow

An official product page may strongly establish:

> Product X supports Arabic.

It does not establish:

> Product X provides high-quality Arabic.

Do not extend claims beyond the evidence.

---

# 80. Researcher Judgment Must Be Visible

When an agent makes an interpretation, mark it appropriately.

Example:

```text
[EVIDENCE]
Three products require users to open separate source pages.

[OBSERVATION]
Source verification adds workflow steps.

[HYPOTHESIS]
Reducing these steps could materially improve research speed.
```

This prevents interpretation from masquerading as evidence.

---

# 81. Assumptions

Any assumption materially affecting a conclusion should be explicit.

Use:

```text
[ASSUMPTION]
The target user has internet access during the workflow.
```

Assumptions requiring testing should be added to open questions.

---

# 82. Unknowns

Record unknowns explicitly.

Example:

```text
[UNKNOWN]
How frequently mosque educators prepare multilingual material.

VALIDATION NEEDED:
Interviews or survey with educators.
```

Unknowns are research outputs.

Do not hide them.

---

# 83. Evidence Gaps

Use:

```text
[EVIDENCE GAP]

Question:

Why it matters:

Evidence currently available:

What would resolve it:
```

The Research Director should preserve important evidence gaps in final synthesis.

---

# 84. Research Priority

Prioritize unresolved questions that could change the project decision.

High-priority unknown:

> Do target users already have an effective solution?

Low-priority unknown:

> Which icon style do they prefer?

Focus research effort accordingly.

---

# 85. Decision-Changing Evidence

Before additional research, ask:

> Could the answer change whether we pursue this opportunity?

If no, deprioritize it.

This prevents unnecessary research expansion.

---

# 86. Evidence Cost

Some evidence may require excessive effort to obtain.

When this occurs:

- document the gap;
    
- identify the best available proxy;
    
- reduce confidence accordingly.
    

Do not invent certainty because perfect evidence is unavailable.

---

# 87. Time-Bounded Research

This project is ultimately hackathon-oriented.

Evidence standards should remain rigorous while recognizing limited time.

Agents should seek:

> sufficient high-quality evidence for informed decision-making

rather than:

> academic completeness.

Research depth should match decision importance.

---

# 88. Red-Team Standard

The Red-Team / Skeptic Researcher should focus especially on:

- unsupported generalization;
    
- weak populations;
    
- competitor blindness;
    
- AI-for-AI's-sake;
    
- measurement weakness;
    
- religious risk;
    
- confirmation bias;
    
- implementation assumptions.
    

Red-team criticism should itself be evidence-based.

---

# 89. Research Director Standard

The Research Director must not merely count how many agents support an idea.

Instead evaluate:

- quality of evidence;
    
- independence;
    
- directness;
    
- population fit;
    
- contradictory evidence;
    
- maturity;
    
- unresolved risk.
    

Five agents repeating the same weak source do not outweigh one strong contradictory source.

---

# 90. Evidence Quality Before Agent Consensus

Agent consensus is not evidence.

A finding does not become true because:

> six agents independently thought it sounded plausible.

The agents must ultimately rely on external or directly observed evidence.

---

# 91. Source Coverage Is Not Problem Validation

A large corpus of Islamic sources does not itself demonstrate a user problem.

Likewise:

A large dataset does not establish demand.

Always connect evidence back to:

> user + task + pain + consequence.

---

# 92. Novelty Is Not Evidence

An idea being unusual or innovative does not prove it is useful.

Novelty should be considered only after:

- problem validation;
    
- user relevance;
    
- solution gap.
    

---

# 93. Technical Possibility Is Not User Value

Evidence that AI can perform a task does not establish that users need it.

Two separate questions are required:

1. Can it be done?
    
2. Is it worth doing?
    

Both need evidence.

---

# 94. User Desire Is Not Technical Feasibility

Likewise, strong user demand does not prove the solution can be safely implemented.

Separate:

- desirability;
    
- feasibility;
    
- reliability.
    

---

# 95. Evidence for Hackathon Fit

After problem validation, collect evidence relevant to challenge suitability.

Questions include:

- Does it align with a challenge track?
    
- Is AI materially useful?
    
- Can benefit be measured?
    
- Can reliability be demonstrated?
    
- Can a working solution be built?
    
- Can the workflow be shown clearly?
    

Do not use hackathon fit to fabricate problem importance.

---

# 96. Demo Evidence

A future demo should show measurable workflow improvement.

Before solution selection, research whether a potential demonstration can establish:

```text
BEFORE STATE

INTERVENTION

AFTER STATE

MEASUREMENT

TRACEABLE RESULT
```

Avoid demo concepts relying only on subjective visual impressiveness.

---

# 97. Evidence Review Before Promotion

Before promoting an opportunity, an agent should ask:

```text
Do we know who has the problem?

Do we know their real workflow?

Is there direct evidence of pain?

Is there independent corroboration?

Have current solutions been researched?

Have we searched for contradictory evidence?

Do we understand important limitations?

Can the problem be measured?

Could a simpler solution work?

Is AI plausibly useful?

Are religious risks understood?

What remains unknown?
```

If several answers are:

> No

the opportunity is not mature.

---

# 98. Evidence Quality Failure Modes

Common research failures include:

### Confirmation Bias

Only collecting supporting sources.

### Availability Bias

Assuming easily found online complaints represent everyone.

### Popularity Bias

Treating viral posts as representative.

### Authority Misuse

Using respected sources for claims outside their expertise.

### Recency Bias

Ignoring older but stronger evidence.

### Citation Laundering

Using secondary references without checking originals.

### Feature Bias

Assuming missing product features equal user problems.

### Technology Bias

Assuming AI involvement increases value.

### Consensus Bias

Assuming agent agreement equals truth.

Agents must actively guard against these.

---

# 99. Minimum Evidence for Final Opportunity Synthesis

Before an opportunity enters the final synthesis table, it should ideally have:

```text
1. Defined user

2. Defined workflow

3. Core pain

4. Direct problem evidence

5. Independent corroboration

6. Existing-solution research

7. Gap analysis

8. Disconfirming evidence

9. Islamic / trust constraints where relevant

10. Potential AI leverage

11. Non-AI baseline

12. Possible measurable outcome

13. Open questions

14. Confidence levels
```

If something is missing, mark it visibly.

---

# 100. Final Evidence Principle

The purpose of evidence is not to make an idea look convincing.

The purpose is to determine whether the idea **deserves to be convincing**.

Therefore:

**Do not reward quantity without quality.**

**Do not reward consensus without verification.**

**Do not reward novelty without need.**

**Do not reward AI capability without user value.**

**Do not hide contradictory evidence.**

**Do not convert uncertainty into confidence.**

The strongest opportunity is not the one with the most enthusiastic story.

It is the one that survives serious investigation and still demonstrates:

> **a real user, a real problem, a meaningful gap, defensible evidence, measurable value, and a responsible path toward solving it.**