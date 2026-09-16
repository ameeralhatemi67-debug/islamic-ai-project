## Islamic AI Challenge — Cross-Examination Protocol

This document defines how research agents must challenge, defend, revise, escalate, and resolve important findings before those findings enter final synthesis.

Cross-examination exists to prevent:

- weak claims from surviving because nobody challenged them;
    
- premature consensus;
    
- groupthink;
    
- repeated unsupported assumptions;
    
- false market-gap claims;
    
- unjustified AI use;
    
- religious-boundary errors;
    
- evidence inflation;
    
- unresolved contradictions being hidden during synthesis.
    

This protocol supplements:

- `AGENTS.md`
    
- `research-protocol/source-policy.md`
    
- `research-protocol/evidence-standard.md`
    
- `research-protocol/problem-card-schema.md`
    
- `research-protocol/reference-project-schema.md`
    
- all specialist-agent role files;
    
- `agents/07-red-team.md`
    
- `agents/08-research-director.md`
    

If this protocol conflicts with `AGENTS.md`, follow `AGENTS.md`.

The Research Director moderates cross-examination.

---

# 1. Core Principle

Cross-examination is not a brainstorming session.

It is not a debate where agents try to win.

It is a structured attempt to answer:

> **What survives when the strongest available evidence, alternatives, objections, and failure cases are placed against a research conclusion?**

The objective is:

**challenge → test → revise → resolve → preserve uncertainty**

not:

**argue → persuade → force agreement**

---

# 2. Position in the Research Process

Cross-examination occurs only after enough independent work exists to challenge.

The intended sequence is:

```text
Independent Discovery

→

Problem Cards

→

Evidence Validation

→

Market / Reference Landscape

→

AI Opportunity Analysis

→

Red Team Review

→

CROSS-EXAMINATION

→

Director Synthesis

→

Opportunity Map
```

Cross-examination must not contaminate the initial independent-discovery phase.

---

# 3. Purpose

The protocol has six primary objectives.

### A. Test Problem Validity

Determine whether the user problem is sufficiently demonstrated.

### B. Test Gap Validity

Determine whether existing solutions actually leave the claimed gap unresolved.

### C. Test AI Necessity

Determine whether AI provides real advantage over realistic alternatives.

### D. Test Trust and Islamic Boundaries

Determine whether the opportunity preserves source integrity, uncertainty, scholarly boundaries, and appropriate human escalation.

### E. Test Feasibility and Measurability

Determine whether the proposed opportunity can realistically be implemented and evaluated.

### F. Expose Uncertainty

Identify what remains unknown rather than forcing unsupported conclusions.

---

# 4. Cross-Examination Objects

Cross-examination may target:

```text
PROBLEM CARD

MARKET-GAP CLAIM

REFERENCE-PROJECT CONCLUSION

AI OPPORTUNITY

TRUST / RELIABILITY CLAIM

MEASUREMENT CLAIM

FEASIBILITY CLAIM

CRITICAL ASSUMPTION

SYNTHESIS CLAIM
```

Do not cross-examine vague conversation fragments when a structured artifact exists.

Use the artifact.

---

# 5. Required Inputs

Before a major opportunity enters cross-examination, the Director should ideally have:

```text
Problem Card

Supporting evidence

Contradicting evidence

Relevant Reference Projects

Gap analysis

Non-AI alternative

AI Opportunity Record

Trust / safety notes

Red Team challenge

Critical assumptions
```

Missing information does not automatically stop cross-examination.

It may itself become a finding.

---

# 6. Readiness Gate

The Director should ask:

```text
Is the user defined?

Is the task defined?

Is the workflow described?

Is evidence attached?

Have current solutions been searched?

Is the claimed gap stated?

Has a non-AI alternative been considered?

If AI is proposed, is the capability specified?

Have important trust risks been identified?
```

If most answers are `NO`, the object is not ready.

Return it for research rather than conducting performative debate.

Use:

```text
[CROSS-EXAMINATION NOT READY]
```

---

# 7. Participants

Cross-examination may involve:

### Research Director — Agent 08

Moderator and resolution manager.

### Originating Agent

The agent responsible for the challenged artifact.

### Relevant Specialist Agents

Agents whose scope materially intersects with the claim.

### Agent 05 — Market Landscape Researcher

Required where novelty, competition, existing solutions, or market gaps are challenged.

### Agent 06 — AI Opportunity Researcher

Required where AI necessity, capability, feasibility, or measurement are challenged.

### Agent 07 — Red Team

Primary adversarial challenger.

Not every agent must participate in every examination.

Use only agents whose expertise materially contributes.

---

# 8. Research Director Role

The Research Director must:

- choose what is examined;
    
- define the disputed claims;
    
- distribute only necessary context;
    
- preserve structured turn-taking;
    
- prevent pile-ons;
    
- request evidence;
    
- distinguish resolved from unresolved issues;
    
- assign research returns;
    
- update challenge status;
    
- preserve disagreements;
    
- determine whether the object may proceed to synthesis.
    

The Director must not decide issues through personal preference.

---

# 9. Originating Agent Role

The originating agent must:

- explain the claim;
    
- cite its evidence;
    
- identify limitations;
    
- respond directly to challenges;
    
- concede when evidence fails;
    
- revise claims when justified;
    
- avoid defending wording merely because it authored it.
    

The originating agent is defending:

> the accuracy of the research,

not:

> its reputation.

---

# 10. Red Team Role

Agent 07 should focus on high-impact failure modes.

Its priority is:

```text
P0 assumptions

→

problem invalidation

→

hidden competitors

→

AI necessity

→

safety / trust

→

feasibility

→

measurement
```

The Red Team should not generate dozens of low-value objections.

Prefer one fatal challenge over twenty cosmetic criticisms.

---

# 11. Specialist Reviewer Role

Other specialist agents should challenge only within areas where they bring useful evidence or perspective.

Examples:

Agent 01:

> Is this actually a problem for general Muslim users?

Agent 02:

> Does this accurately represent new-Muslim needs?

Agent 03:

> Does this match real educator/content workflows?

Agent 04:

> Are trust, provenance, uncertainty, and source boundaries represented correctly?

Agent 05:

> Is the gap actually unsolved?

Agent 06:

> Is AI actually necessary?

Do not manufacture objections merely to participate.

---

# 12. Independence Before Discussion

Whenever feasible, agents should submit their initial critiques independently before seeing other critiques.

The sequence should be:

```text
Artifact distributed

→

Independent review

→

Challenges recorded

→

Challenges revealed

→

Discussion
```

This reduces:

- anchoring;
    
- imitation;
    
- social convergence;
    
- repeated objections.
    

---

# 13. No Raw Reasoning Transfer

Agents should exchange structured conclusions and evidence, not unrestricted internal reasoning.

Cross-examination inputs should primarily contain:

- claims;
    
- evidence;
    
- citations;
    
- assumptions;
    
- challenge records;
    
- structured responses.
    

This keeps the process auditable and reduces context contamination.

---

# 14. Claim Freezing

Before examination begins, freeze the exact claim being challenged.

Example:

```text
CLAIM ID:
CL-014

CLAIM:
English-speaking new Muslims frequently struggle to determine whether conflicting online Islamic answers represent legitimate scholarly disagreement.

SOURCE ARTIFACT:
P-008

CONFIDENCE:
Medium
```

Do not allow the claim to shift silently during debate.

If revised, record both versions.

---

# 15. Challenge IDs

Every substantive challenge should receive an ID.

Use:

```text
CX-001
CX-002
CX-003
```

Where examination sessions are numerous, optionally include the target:

```text
CX-P008-01

CX-AIOP003-02
```

Once assigned, do not reuse an ID.

---

# 16. Standard Challenge Record

Use:

```text
CHALLENGE ID:

TARGET:

CHALLENGER:

CLAIM BEING CHALLENGED:

CHALLENGE:

WHY IT MATTERS:

EVIDENCE:

COUNTEREVIDENCE:

MISSING EVIDENCE:

SEVERITY:
P0 / P1 / P2 / P3

RECOMMENDED VALIDATION:

STATUS:
Open / Answered / Resolved / Disconfirmed / Accepted Limitation
```

Challenges must be specific.

---

# 17. Severity Levels

Use:

### P0 — Potentially Fatal

If correct, this could invalidate the problem, gap, AI opportunity, safety, or feasibility.

Examples:

- problem does not exist;
    
- strong competitor already solves it;
    
- required data cannot be used;
    
- uncontrolled high-severity religious risk.
    

### P1 — Major

Could materially weaken or reframe the opportunity.

### P2 — Important

Useful issue that should be addressed but does not threaten the core claim.

### P3 — Minor

Low-impact concern.

Cross-examination should focus primarily on P0 and P1.

---

# 18. Evidence Burden

The burden of evidence belongs to the party making the positive claim.

Examples:

Claim:

> Users frequently experience this problem.

The originating agent must support frequency.

Claim:

> No current system provides this capability.

The landscape research must support search coverage.

Claim:

> AI will substantially reduce research time.

Agent 06 must provide a plausible basis and evaluation method.

A challenger does not need to prove the opposite before requesting evidence.

---

# 19. Absence Claims Require Special Care

Claims such as:

> “No product exists.”

or:

> “Nobody has solved this.”

are difficult to establish.

Prefer:

> “No reviewed system was found meeting conditions A, B, and C after searches across X, Y, and Z.”

Cross-examination should downgrade unsupported universal absence claims.

---

# 20. Cross-Examination Sequence

A standard examination should proceed through:

```text
ROUND 0 — Preflight

ROUND 1 — Problem & User

ROUND 2 — Evidence

ROUND 3 — Existing Solutions & Gap

ROUND 4 — AI Necessity

ROUND 5 — Trust & Islamic Boundaries

ROUND 6 — Feasibility & Measurement

ROUND 7 — Red Team Critical Attack

ROUND 8 — Originating Agent Response

ROUND 9 — Targeted Rebuttal

ROUND 10 — Director Resolution
```

Not every round is necessary for every artifact.

---

# 21. Round 0 — Preflight

The Director establishes:

```text
TARGET ARTIFACT:

OWNER:

CLAIMS UNDER EXAMINATION:

KNOWN EVIDENCE:

KNOWN COUNTEREVIDENCE:

KNOWN CRITICAL ASSUMPTIONS:

PARTICIPATING AGENTS:

QUESTIONS TO RESOLVE:
```

Do not begin with an unrestricted prompt such as:

> “Discuss this idea.”

---

# 22. Round 1 — Problem & User Examination

Questions may include:

- Who exactly experiences this?
    
- What are they trying to accomplish?
    
- Where in the workflow does failure occur?
    
- Is the pain demonstrated?
    
- How often does it happen?
    
- What consequence results?
    
- Is the user segment too broad?
    
- Is this actually a symptom of a deeper problem?
    
- Does the user currently attempt to solve it?
    

Useful output:

```text
PROBLEM VALIDITY:
Supported / Weak / Requires Reframe / Disconfirmed
```

---

# 23. Round 2 — Evidence Examination

Review:

- directness;
    
- authority;
    
- independence;
    
- recency;
    
- representativeness;
    
- corroboration;
    
- contradicting evidence.
    

Ask:

> Does the evidence actually support the stated claim?

Not merely:

> Is there a citation?

---

# 24. Citation Audit

For important claims verify:

```text
SOURCE EXISTS?

SOURCE SAYS WHAT IS CLAIMED?

CONTEXT PRESERVED?

DATE RELEVANT?

POPULATION MATCHES?

PRIMARY OR SECONDARY?

INDEPENDENT CORROBORATION?
```

Citation presence alone does not establish evidence quality.

---

# 25. Behavioral Evidence Test

When a problem claim relies heavily on stated preferences, ask whether behavioral evidence exists.

Useful behavioral signals include:

- switching tools;
    
- repeated searching;
    
- manual workarounds;
    
- asking humans;
    
- abandoning workflows;
    
- repeated complaints;
    
- maintaining personal systems.
    

Behavior often provides stronger problem evidence than general opinion.

---

# 26. Round 3 — Existing Solutions & Gap

Agent 05 should address:

- direct competitors;
    
- partial competitors;
    
- adjacent Islamic systems;
    
- non-AI alternatives;
    
- manual alternatives;
    
- adjacent-domain patterns.
    

Core question:

> What remains unsolved after we consider the strongest realistic alternatives?

---

# 27. Gap Attack Questions

Ask:

- Is this gap genuinely missing?
    
- Is it only missing from one product?
    
- Can several existing products solve the workflow together?
    
- Is fragmentation itself sufficiently painful?
    
- Is the claimed differentiator actually important?
    
- Was Arabic-language search conducted where relevant?
    
- Were academic and GitHub projects searched?
    
- Is a human service the real competitor?
    

---

# 28. Gap Outcome

Use:

```text
GAP STATUS:

Strongly Supported

Partially Supported

Fragmented-Solution Gap

Weak

Already Solved

Disconfirmed

Unknown
```

Do not let an opportunity proceed with:

> “No competitors found”

when the search methodology was weak.

---

# 29. Round 4 — AI Necessity

Agent 06 should defend AI only after the gap survives.

Required questions:

```text
What exact task needs improvement?

What is the strongest non-AI baseline?

Why is that baseline insufficient?

What specific AI capability helps?

What measurable change should result?

What new failure modes does AI create?
```

---

# 30. Strongest Non-AI Baseline Rule

Do not compare the AI proposal against an intentionally weak workflow.

For example:

Weak comparison:

> AI versus manually reading thousands of pages.

Better comparison:

> AI semantic retrieval versus current specialist search + filters.

Cross-examination should require the strongest realistic alternative.

---

# 31. AI Necessity Outcomes

Use:

```text
AI LEVERAGE:

Strong

Moderate

Weak

Unnecessary

Unknown
```

If AI is unnecessary, the research result is still valuable.

Do not preserve AI simply to fit the competition theme.

---

# 32. Generative AI Challenge

If text generation is proposed, ask:

- Why generation instead of retrieval?
    
- Why generation instead of extraction?
    
- Can the user inspect evidence?
    
- How is unsupported synthesis detected?
    
- Can the system refuse?
    
- Is human review needed?
    

Generation requires stronger justification than retrieval-only systems in high-trust contexts.

---

# 33. Agentic Architecture Challenge

If a proposed capability involves multiple autonomous agents:

- What tasks truly require separation?
    
- What measurable advantage results?
    
- Could a simpler pipeline work?
    
- How are conflicting agents resolved?
    
- Does complexity increase hallucination or latency?
    

Do not confuse architecture complexity with innovation.

---

# 34. Round 5 — Trust & Islamic Boundaries

Agent 04 should examine:

```text
SOURCE TRUST

ATTRIBUTION

CITATION

CONTEXT

TRANSLATION

SCOPE

UNCERTAINTY

SCHOLARLY DISAGREEMENT

BOUNDARY

REFUSAL

ESCALATION

CORRECTION
```

The key question is:

> Could this system cause a user to mistake generated or scoped information for authoritative universal religious judgment?

---

# 35. Religious Claim Discipline

Cross-examination must preserve distinctions among:

- Qur'anic text;
    
- hadith;
    
- scholarly explanation;
    
- individual fatwa;
    
- institutional ruling;
    
- scholarly disagreement;
    
- agent synthesis.
    

Do not resolve religious disagreements through agent voting.

---

# 36. Scholar-Review Trigger

If the examination requires determining:

- whether consensus exists;
    
- which disputed opinion is correct;
    
- a personalized ruling;
    
- authenticity beyond verified sources;
    
- complex jurisprudential interpretation;
    

mark:

```text
[REQUIRES ISLAMIC SCHOLAR REVIEW]
```

The Director must not improvise a resolution.

---

# 37. Bin Baz Source Handling

When Bin Baz material is involved, verify:

- official source;
    
- exact attribution;
    
- context;
    
- question circumstances;
    
- whether the statement is being generalized beyond its scope.
    

Do not convert:

> “Shaykh Ibn Baz ruled…”

into:

> “All Islamic scholarship holds…”

without independent evidence.

---

# 38. Safety Outcome

Use:

```text
TRUST RISK:

Low

Moderate

High

Requires Scholar / Human Oversight

Unacceptable Under Current Design
```

High risk does not automatically kill an opportunity if the scope can be safely changed.

---

# 39. Round 6 — Feasibility & Measurement

Ask:

- Is required data accessible?
    
- Is licensing compatible?
    
- Is the AI capability currently feasible?
    
- Can evaluation cases be created?
    
- Is expert review available?
    
- Can the workflow be demonstrated?
    
- Can the improvement be measured?
    
- Is the prototype scope realistic?
    

---

# 40. Measurement Challenge

Every important opportunity should answer:

```text
BASELINE:

TASK:

METRIC:

TEST SET:

EXPECTED DIRECTION OF IMPROVEMENT:

WHO VALIDATES RESULTS:
```

Do not require an arbitrary success threshold before experimentation.

Do require a credible measurement method.

---

# 41. Measurement Outcome

Use:

```text
MEASURABILITY:

Clear

Plausible

Difficult

Unclear

Not Credibly Measurable
```

A project with no credible measurement may perform poorly against evidence-focused judging.

---

# 42. Feasibility Outcome

Use:

```text
FEASIBILITY:

High

Medium

Low

Blocked by Dependency

Unknown
```

Record the blocking dependency.

---

# 43. Round 7 — Red Team Critical Attack

Agent 07 should now present only the strongest unresolved attacks.

Recommended maximum:

```text
3 P0 challenges

5 P1 challenges
```

unless exceptional circumstances justify more.

The purpose is focus.

Do not flood the examination with low-value objections.

---

# 44. Critical Assumption Question

For every opportunity, require:

> **What single assumption, if false, most threatens this opportunity?**

Record:

```text
CRITICAL ASSUMPTION:

WHY IT MATTERS:

CURRENT EVIDENCE:

VALIDATION STATUS:
```

---

# 45. Round 8 — Originating Agent Response

The artifact owner must respond to each P0/P1 challenge using one of:

```text
ACCEPT

REJECT WITH EVIDENCE

PARTIALLY ACCEPT

REVISE CLAIM

REQUEST ADDITIONAL RESEARCH

CONCEDE
```

Responses such as:

> “I disagree.”

are insufficient.

---

# 46. Response Template

Use:

```text
CHALLENGE ID:

RESPONSE:

POSITION:
Accept / Reject / Partial / Revise / Research Needed / Concede

EVIDENCE:

REVISED CLAIM:
If applicable

REMAINING UNCERTAINTY:
```

---

# 47. Concession Is Valuable

Agents should not be penalized for conceding a failed claim.

A good response may be:

> “The available evidence does not justify the original frequency claim. Revise from ‘frequent’ to ‘documented among the sampled users; wider prevalence unknown.’”

This improves research quality.

---

# 48. Silent Goalpost Movement Is Forbidden

If the original claim changes materially, record:

```text
ORIGINAL CLAIM:

REVISED CLAIM:

REASON FOR REVISION:
```

Do not allow an agent to defend a weaker claim while pretending the original survived.

---

# 49. Round 9 — Targeted Rebuttal

After the response, the challenger may issue one focused rebuttal where necessary.

Do not restart the full debate.

The rebuttal should answer:

> Does the response actually resolve the original challenge?

Use:

```text
RESOLVED

PARTIALLY RESOLVED

NOT RESOLVED
```

with evidence.

---

# 50. Debate Depth Limit

As a default:

```text
Initial challenge

→

Owner response

→

One rebuttal

→

Director decision
```

Do not allow endless back-and-forth.

Additional rounds require Director approval because new evidence materially changed the question.

---

# 51. New Evidence Rule

If genuinely new evidence appears during rebuttal, the Director may reopen the challenge.

Use:

```text
[REOPENED — NEW EVIDENCE]
```

Do not reopen because participants simply repeat prior arguments.

---

# 52. Director Resolution

The Director evaluates:

- original claim;
    
- challenge;
    
- response;
    
- rebuttal;
    
- evidence.
    

Resolution must be evidence-based.

Possible outcomes:

```text
ORIGINAL CLAIM SUPPORTED

CLAIM SUPPORTED WITH NARROWER SCOPE

CLAIM REQUIRES REVISION

CLAIM REMAINS UNCERTAIN

CLAIM DISCONFIRMED

ADDITIONAL RESEARCH REQUIRED
```

---

# 53. Challenge Status

Final challenge status should use:

```text
OPEN

RESOLVED — CLAIM SUPPORTED

RESOLVED — CLAIM REVISED

RESOLVED — CLAIM DISCONFIRMED

ACCEPTED LIMITATION

RESEARCH RETURN REQUIRED
```

---

# 54. P0 Gate

An unresolved P0 challenge normally blocks promotion into final opportunity synthesis.

Exceptions require the Director to record why the uncertainty can be carried forward.

Example:

```text
P0 STATUS:
Open

DIRECTOR DECISION:
Carry forward as exploratory only.

REASON:
Problem is important but market evidence remains incomplete.
```

Do not present such an opportunity as validated.

---

# 55. P1 Gate

Unresolved P1 challenges may allow progression when:

- the limitation is explicit;
    
- the claim is narrowed;
    
- the uncertainty does not invalidate the opportunity.
    

Record them visibly.

---

# 56. P2 / P3 Treatment

P2 and P3 items should not consume excessive cross-examination time.

Record them for later design work unless they combine into a larger concern.

---

# 57. Research Return Request

When evidence is insufficient, the Director should issue:

```text
[RESEARCH RETURN REQUEST]

REQUEST ID:

TARGET AGENT:

QUESTION:

WHY IT MATTERS:

TARGET CLAIM:

REQUIRED EVIDENCE:

PRIORITY:
P0 / P1 / P2

RETURN FORMAT:
```

Requests must be narrow and answerable.

---

# 58. Good Research Return

Example:

```text
TARGET:
Agent 05

QUESTION:
Find whether Arabic or English Islamic research tools currently provide sentence-level or claim-level citation provenance.

WHY:
GAP-004 depends on this being insufficiently solved.

REQUIRED:
Direct products, screenshots/documentation where possible, current capability evidence.

PRIORITY:
P0
```

---

# 59. Bad Research Return

Avoid:

> “Research competitors more.”

or:

> “Find more evidence.”

These cause wasteful research loops.

---

# 60. Re-Examination After Research Return

When new research arrives:

1. attach it to the relevant challenge;
    
2. allow a concise owner response;
    
3. allow one challenger review;
    
4. Director resolves.
    

Do not repeat the entire cross-examination session.

---

# 61. Disagreement Preservation

If two evidence-backed positions remain unresolved, do not force agreement.

Record the issue in:

```text
/synthesis/disagreements.md
```

using:

```text
DISAGREEMENT ID:

QUESTION:

POSITION A:

EVIDENCE A:

POSITION B:

EVIDENCE B:

ROOT CAUSE:

WHAT WOULD RESOLVE IT:

IMPACT ON OPPORTUNITY:

STATUS:
```

---

# 62. Open Questions

Questions that require future evidence should go to:

```text
/synthesis/open-questions.md
```

Do not bury them inside debate transcripts.

---

# 63. Cross-Agent Convergence

When multiple independent agents reach similar findings, record:

```text
[CROSS-AGENT CONVERGENCE]
```

But verify that their evidence is truly independent.

Repeated use of the same underlying article is not independent convergence.

---

# 64. Cross-Agent Divergence

When agents differ, investigate why.

Possible causes:

```text
DIFFERENT USER SEGMENTS

DIFFERENT GEOGRAPHIES

DIFFERENT SOURCE QUALITY

DIFFERENT TIME PERIODS

DIFFERENT DEFINITIONS

DIFFERENT WORKFLOW STAGES

TRUE EVIDENCE CONFLICT
```

Divergence can reveal useful segmentation.

---

# 65. Majority Vote Is Not Resolution

Do not resolve:

> 5 agents versus 2 agents.

Resolve:

> evidence versus evidence.

A minority position supported by stronger evidence may prevail.

---

# 66. Prevent Pile-On Behavior

Once a challenge has been clearly stated, other agents should not repeat it.

They may add:

- new evidence;
    
- materially different reasoning;
    
- different user implications.
    

Otherwise mark:

```text
DUPLICATE CHALLENGE
```

and merge it.

---

# 67. Prevent Agreement Echoes

Agents do not need to post:

> “I agree.”

unless they provide independent evidence or a meaningful qualification.

Cross-examination values information gain, not social consensus.

---

# 68. Prevent Agent Role Drift

During cross-examination:

Agent 05 should not independently decide religious rulings.

Agent 04 should not claim market absence without market research.

Agent 06 should not invent user demand.

Agent 07 should not override evidence through skepticism alone.

Agent 08 should not invent conclusions unsupported by specialists.

Stay within role boundaries.

---

# 69. Prevent Premature Solution Ideation

Cross-examination may reveal a safer or narrower direction.

Record it as:

```text
[POTENTIAL REFRAME]
```

Do not turn the session into solution brainstorming.

Solution design occurs later.

---

# 70. Reframe Protocol

When a challenge suggests the problem itself should change:

```text
ORIGINAL PROBLEM:

CHALLENGE:

PROPOSED REFRAME:

EVIDENCE FOR REFRAME:

OWNER:

DIRECTOR DECISION:
```

The revised Problem Card should return through validation.

---

# 71. Problem Merge Protocol

If two Problem Cards appear to represent one underlying issue:

```text
CARD A:

CARD B:

SHARED ROOT:

IMPORTANT DIFFERENCES:

MERGE?
Yes / No / Hierarchical

DIRECTOR DECISION:
```

Preserve user-specific manifestations where useful.

---

# 72. Problem Split Protocol

If one Problem Card contains multiple distinct jobs or users:

```text
ORIGINAL CARD:

DISTINCT PROBLEM A:

DISTINCT PROBLEM B:

WHY SPLIT:

DIRECTOR DECISION:
```

Broad cards often hide weak evidence.

---

# 73. Market Gap Reframe

A claim may move from:

> “No solution exists.”

to:

> “Solutions exist, but the workflow remains fragmented.”

This is a valid outcome.

Record the revision rather than treating it as defeat.

---

# 74. AI Reframe

A claim may move from:

> “AI should answer Islamic questions.”

to:

> “AI may assist semantic retrieval while leaving religious judgment to sourced material and human review.”

Cross-examination should reward safer and better-supported narrowing.

---

# 75. Trust Reframe

If religious risk is high, test whether the opportunity survives with:

- retrieval-only behavior;
    
- extractive output;
    
- stronger source display;
    
- human escalation;
    
- narrower user scope;
    
- explicit refusal.
    

If not, record the risk as structural.

---

# 76. Test Cases During Cross-Examination

Where relevant, agents may create future evaluation cases.

Examples:

```text
AMBIGUOUS QUERY

FALSE PREMISE

CONFLICTING SOURCES

MISSING CONTEXT

FABRICATED HADITH

WRONG CITATION

PERSONAL FATWA REQUEST

MULTILINGUAL QUERY

ARABIC TERMINOLOGY

UNSUPPORTED CLAIM
```

These should be preserved for later prototype evaluation.

---

# 77. Islamic Knowledge Test Cases

High-risk opportunities should eventually include scenarios where the system must:

- refuse;
    
- request clarification;
    
- distinguish viewpoints;
    
- show sources;
    
- identify insufficient evidence;
    
- escalate.
    

The ability to abstain may be part of successful performance.

---

# 78. Evidence Changes Confidence

Cross-examination must update confidence when warranted.

Example:

```text
BEFORE:
High

AFTER:
Medium

REASON:
Major competitor found; gap narrower than initially believed.
```

or:

```text
BEFORE:
Medium

AFTER:
High

REASON:
Independent behavioral evidence confirmed the workflow problem and disconfirmation search found no adequate solution.
```

Confidence changes require reasons.

---

# 79. Confidence Is Component-Specific

Do not assign one confidence label to the entire opportunity.

Use:

```text
PROBLEM EXISTENCE:

USER IMPORTANCE:

MARKET GAP:

AI LEVERAGE:

MEASURABILITY:

FEASIBILITY:

TRUST MITIGATION:
```

Each may differ.

---

# 80. Cross-Examination Result Record

Each examined object should produce:

```text
# Cross-Examination Result

TARGET:

DATE / CYCLE:

DIRECTOR:

PARTICIPANTS:

CLAIMS EXAMINED:

P0 CHALLENGES:

P1 CHALLENGES:

REVISIONS:

DISCONFIRMED CLAIMS:

ACCEPTED LIMITATIONS:

OPEN QUESTIONS:

RESEARCH RETURNS:

SURVIVING CLAIMS:

CONFIDENCE CHANGES:

DIRECTOR STATUS:
Proceed / Proceed with Limitations / Rework / Hold / Discontinue
```

---

# 81. Director Status Definitions

### Proceed

Critical claims survived.

### Proceed with Limitations

Opportunity remains useful but material uncertainty must remain visible.

### Rework

Core framing needs revision before synthesis.

### Hold

Important missing research prevents a decision.

### Discontinue

Evidence no longer supports further consideration.

---

# 82. Survived Challenge Label

Use:

```text
[SURVIVED CROSS-EXAMINATION]
```

only when:

- meaningful challenges were raised;
    
- P0 issues were resolved;
    
- P1 issues are resolved or explicitly accepted;
    
- evidence remains sufficient.
    

Do not use it merely because discussion occurred.

---

# 83. Disconfirmed Label

Use:

```text
[DISCONFIRMED BY CROSS-EXAMINATION]
```

when evidence shows the central claim should no longer be treated as viable.

Preserve why it failed.

---

# 84. Accepted Limitation

Some weaknesses may remain without invalidating the opportunity.

Use:

```text
[ACCEPTED LIMITATION]
```

Example:

> Strong evidence exists in English-speaking communities, but Arabic-user prevalence remains unknown.

This limitation should appear in synthesis.

---

# 85. Research Efficiency

Cross-examination must not become an unlimited research process.

Prioritize questions that could materially change:

- problem validity;
    
- gap validity;
    
- AI necessity;
    
- safety;
    
- feasibility;
    
- measurement.
    

Do not spend substantial effort resolving cosmetic differences.

---

# 86. Information-Gain Rule

Before requesting new research ask:

> If we answer this question, could it change whether we pursue or reframe the opportunity?

If `NO`, defer it.

---

# 87. Stop Conditions

Cross-examination should stop when:

- all P0 challenges are resolved or explicitly carried as blocking uncertainty;
    
- major P1 challenges are resolved or accepted;
    
- new arguments repeat earlier points;
    
- additional research has low decision value;
    
- the Director has enough information to set a status.
    

Perfect certainty is not required.

---

# 88. Anti-Loop Rule

Do not repeat:

```text
challenge
→ search
→ slightly revised challenge
→ search
→ same challenge
```

If two research returns fail to materially change an issue, the Director should classify it as:

```text
UNRESOLVED WITH AVAILABLE EVIDENCE
```

and move forward accordingly.

---

# 89. Token / Context Efficiency

Prefer structured records over entire raw research histories.

For each examination, provide participants only:

- target artifact;
    
- key evidence;
    
- relevant reference projects;
    
- existing challenges;
    
- role-specific context.
    

Do not load unrelated research.

---

# 90. Batch Similar Challenges

If several Problem Cards depend on the same assumption, examine the shared assumption once.

Example:

```text
ASSUMPTION:
Users value visible source provenance.

AFFECTED:
P-004
P-008
AI-OP-002
AI-OP-005
```

Reuse the result.

---

# 91. Conflict With Source Policy

If a cross-examination conclusion conflicts with Islamic source-handling requirements, the source policy takes precedence.

Do not vote around source-integrity rules.

---

# 92. Conflict With Evidence Standard

If participants want to promote a claim despite evidence below the required standard:

- lower confidence;
    
- narrow the claim;
    
- request validation;
    
- or reject promotion.
    

Do not weaken the evidence standard for attractive ideas.

---

# 93. Conflict With Hackathon Appeal

A highly impressive demo does not override weak problem evidence.

If:

```text
DEMO:
Strong

PROBLEM:
Weak
```

the Director should record the weakness.

Do not manufacture validation to preserve an attractive concept.

---

# 94. Cross-Examination Does Not Choose the Winner

The protocol determines:

- what is supported;
    
- what is weak;
    
- what survives;
    
- what remains uncertain.
    

It does not automatically choose the final hackathon concept.

Selection occurs after the opportunity landscape is synthesized.

---

# 95. Minimum Cross-Examination Gate for Major Opportunities

Before a major opportunity reaches final synthesis it should answer:

```text
Who has the problem?

What evidence proves it?

What is the user's current workflow?

What existing solution is strongest?

What remains unresolved?

Why is AI needed?

What is the strongest non-AI alternative?

How would improvement be measured?

What are the main Islamic trust risks?

What critical assumption threatens the opportunity?

What did the Red Team find?

What remains uncertain?
```

---

# 96. Required Final Outputs

At the end of the cross-examination phase, the Director should have:

### A. Resolved Challenge Records

### B. Open P0/P1 Challenges

### C. Revised Problem Cards

Where necessary.

### D. Revised Gap Claims

Where necessary.

### E. Revised AI Opportunity Records

Where necessary.

### F. Disagreement Register

### G. Open Questions Register

### H. Research Return Results

### I. List of Disconfirmed Opportunities

### J. List of Opportunities That Survived

These become inputs to synthesis.

---

# 97. Cross-Examination Summary Template

```text
# Cross-Examination Cycle Summary

## Scope

Artifacts examined:
...

## P0 Challenges

...

## P1 Challenges

...

## Claims Revised

...

## Claims Disconfirmed

...

## Problems Reframed

...

## Market Gaps Revised

...

## AI Opportunities Revised

...

## Trust / Islamic Boundary Findings

...

## Research Returns

...

## Unresolved Disagreements

...

## Open Questions

...

## Opportunities Discontinued

...

## Opportunities Proceeding

...

## Accepted Limitations

...

## Confidence Changes

...
```

---

# 98. Definition of Done

Cross-examination is complete when the Research Director can answer:

**What exact claims were tested?**

**What were the strongest objections?**

**What evidence supported those objections?**

**How did the originating agent respond?**

**Which claims survived unchanged?**

**Which claims were narrowed?**

**Which claims were disproved?**

**Which problems were reframed?**

**Which market gaps remain credible?**

**Where is AI still justified?**

**Where was AI found unnecessary?**

**Which trust or Islamic boundaries remain important?**

**What assumptions remain unresolved?**

**What additional research is still necessary?**

**Which opportunities are defensible enough to enter synthesis?**

If these questions cannot be answered, cross-examination is incomplete.

---

# 99. Final Principle

Cross-examination exists to create productive friction between evidence and enthusiasm.

Its objective is not:

> “Make every idea survive.”

Its objective is:

> **Expose each important research claim to the strongest relevant challenge and preserve only what the evidence can still support.**

Challenge claims precisely.

Require evidence.

Use the strongest alternative.

Do not reward complexity.

Do not hide contradiction.

Do not force consensus.

Allow agents to concede.

Narrow claims when necessary.

Escalate religious uncertainty.

Stop when additional debate stops producing information.

And treat a disproved idea as progress, because every weak idea eliminated increases the quality of the opportunities that remain.