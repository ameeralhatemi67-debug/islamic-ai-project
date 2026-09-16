## Islamic AI Challenge — Problem Card Schema

This document defines the required structure for every validated or potentially valuable problem discovered by the research agents.

A Problem Card is not an idea pitch.

It is a structured research object used to capture:

- who experiences the problem;
    
- what they are trying to do;
    
- what currently happens;
    
- where the workflow breaks;
    
- why the problem matters;
    
- what evidence supports it;
    
- what evidence weakens it;
    
- what solutions already exist;
    
- whether an unresolved gap remains;
    
- whether AI may eventually have a justified role.
    

This document supplements:

- `AGENTS.md`
    
- `research-protocol/source-policy.md`
    
- `research-protocol/evidence-standard.md`
    

---

# 1. Core Principle

A Problem Card must describe and validate the **problem before proposing the product**.

The required reasoning sequence is:

**User → Context → Goal → Workflow → Pain → Consequence → Evidence → Existing Solutions → Remaining Gap → Constraints → Measurement → Opportunity**

Do not begin with:

> “We should build…”

Begin with:

> “This user is trying to accomplish X and repeatedly encounters Y.”

---

# 2. When to Create a Problem Card

Create a Problem Card when a research finding has progressed beyond a casual observation.

A Problem Card is appropriate when:

- a specific user can be identified;
    
- a meaningful task or goal exists;
    
- some evidence of friction has been found;
    
- the problem appears worth deeper investigation.
    

A Problem Card may still be:

- unvalidated;
    
- weak;
    
- promising;
    
- validated;
    
- rejected.
    

Creating the card does not imply endorsement.

---

# 3. Problem Card File Naming

Use:

```text
P-XXX-short-descriptive-name.md
```

Examples:

```text
P-001-convert-islamic-terminology-barrier.md

P-014-content-creator-source-verification.md

P-027-multilingual-islamic-context-loss.md
```

Do not use:

```text
idea1.md
cool-project.md
problem-final-v2.md
```

Problem IDs must remain stable once assigned.

---

# 4. Problem ID Format

Use:

```text
P-001
P-002
P-003
```

Do not reuse IDs from rejected or merged problems.

If two cards are later merged, retain both historical IDs and identify the new primary card.

Example:

```text
MERGED FROM:
P-011
P-018

PRIMARY:
P-024
```

---

# 5. Required Problem Card Template

Every Problem Card must follow the structure below.

```text
# [P-XXX] Problem Title

## 1. Status

Problem status:
UNVALIDATED / PROMISING / VALIDATED / WEAK / REJECTED

Evidence maturity:
LEVEL 0 / LEVEL 1 / LEVEL 2 / LEVEL 3 / LEVEL 4

Primary research owner:

Reviewers:

Last updated:


## 2. One-Sentence Problem Statement

[Specific user] struggles to [complete important task] because [core friction], resulting in [meaningful consequence].


## 3. Primary User

Primary user:

Role:

Knowledge level:

Language:

Geography:

Relevant characteristics:

Why this user matters:


## 4. Secondary Users / Stakeholders

Secondary users:

Experts involved:

Institutions involved:

People affected indirectly:


## 5. User Context

When does the problem occur?

Where does it occur?

What triggers the task?

What constraints exist?

What tools does the user already have?


## 6. Job to Be Done

When:

I want to:

So that:

Success looks like:


## 7. Current Workflow

Trigger:

Step 1:

Step 2:

Step 3:

Step 4:

...

Final outcome:


## 8. Workflow Evidence

How was this workflow discovered?

Evidence IDs:

What parts are directly observed?

What parts are reported by users?

What parts remain assumptions?

Workflow gaps:


## 9. Core Pain

Primary pain:

Where in the workflow does it occur?

Why does it occur?

What does the user currently do about it?


## 10. Consequences

Immediate consequence:

Long-term consequence:

Religious / trust consequence:

Time consequence:

Financial consequence:

Learning consequence:

Emotional / cognitive consequence:

Other:


## 11. Frequency

How often does the problem occur?

Evidence:

Confidence:
High / Medium / Low


## 12. Severity

How harmful or costly is the problem when it occurs?

Evidence:

Confidence:
High / Medium / Low


## 13. Existing Workarounds

Workaround 1:

Workaround 2:

Workaround 3:

Why users use them:

Cost of workaround:

Weaknesses:


## 14. Existing Solutions

Solution / Product:

URL:

Target user:

How it addresses the problem:

Evidence:

Known strengths:

Known limitations:

User complaints:

Current status:


## 15. Remaining Gap

What remains insufficiently solved?

Evidence that users care about this gap:

Why existing solutions do not fully address it:

Is this a true problem gap or merely a missing feature?


## 16. Supporting Evidence

Evidence ID:

Source:

Type:

Finding:

Strength:

What it supports:


## 17. Contradicting / Disconfirming Evidence

Evidence ID:

Source:

What it contradicts:

Strength:

Does it materially weaken the problem?


## 18. Disconfirmation Search

Hypothesis being challenged:

What would make the problem weak or irrelevant?

Searches performed:

Evidence found against the problem:

Evidence found supporting the problem:

Current assessment:


## 19. Islamic Knowledge / Reliability Considerations

Does the problem involve Islamic rulings?

Does it involve Qur'an or hadith?

Does it involve scholarly disagreement?

Does it involve personal fatwa requests?

Could incorrect output create religious harm?

Does it require source attribution?

Does it require qualified human review?

Relevant source-policy notes:

Markers:
[REQUIRES ISLAMIC SCHOLAR REVIEW]
[REQUIRES SOURCE-BOUNDARY REVIEW]
[PERSONAL SCHOLARLY JUDGMENT MAY BE REQUIRED]


## 20. Trust and Safety Risks

Hallucination risk:

Misquotation risk:

Context loss:

Overgeneralization:

False consensus:

Privacy risk:

Bias risk:

Misuse risk:

Other:


## 21. Potential AI Leverage

What part of the problem could AI plausibly improve?

Why might AI be useful?

Possible AI capability:

What evidence supports this?

Confidence:
High / Medium / Low


## 22. Non-AI Baseline

How could the problem be addressed without AI?

Current non-AI approach:

Possible improved non-AI solution:

Would AI still provide meaningful additional value?

Why?


## 23. Why AI Might Be the Wrong Choice

Could deterministic software solve it?

Could better search solve it?

Could better information architecture solve it?

Could a database solve it?

Could human support solve it more safely?

What new risks would AI introduce?


## 24. Intervention Point

Where in the current workflow would an improved solution intervene?

Before:

Intervention:

After:

Why this point matters:


## 25. Measurable Outcome

Primary success metric:

Baseline:

Possible improved state:

How could it be measured?

Secondary metrics:

Potential proxy metrics:


## 26. Before / After Model

BEFORE:

User currently:

Time:

Steps:

Errors:

Trust / verification burden:


AFTER — hypothetical only:

User could:

Time:

Steps:

Errors:

Trust / verification burden:


Important:
Do not invent improvement values before testing.


## 27. Demo Potential

Can the problem be demonstrated clearly?

What would a judge see in the "before" state?

What would a judge see in the improved state?

Can value be understood in under 60 seconds?

What could be quantitatively compared?


## 28. Hackathon Relevance

Possible challenge track:

Why it fits:

Target audience fit:

Potential measurable benefit:

Reliability relevance:

Technical relevance:

Do not use this section to justify an otherwise weak problem.


## 29. Technical Feasibility Questions

Required data:

Available data:

Potential models:

Retrieval requirements:

APIs:

Language requirements:

Latency concerns:

Cost concerns:

Evaluation requirements:

Unknowns:


## 30. Adoption Considerations

Would the target user realistically use a new tool?

Current habits:

Switching cost:

Trust barrier:

Device / platform requirements:

Language expectations:

Institutional dependencies:

Evidence:


## 31. Comparable / Adjacent Projects

Project:

Domain:

URL:

Why it is relevant:

What we can learn:

What does not transfer:


## 32. Assumptions

[ASSUMPTION]

[ASSUMPTION]

[ASSUMPTION]


## 33. Unknowns

[UNKNOWN]

[UNKNOWN]

[UNKNOWN]


## 34. Evidence Gaps

[EVIDENCE GAP]

Question:

Why it matters:

What evidence currently exists:

What would resolve it:


## 35. Decision-Changing Questions

Question 1:

If answer is YES:

If answer is NO:


Question 2:

If answer is YES:

If answer is NO:


## 36. Confidence Assessment

Problem existence:
High / Medium / Low

Problem frequency:
High / Medium / Low

Problem severity:
High / Medium / Low

Workflow understanding:
High / Medium / Low

Current-solution gap:
High / Medium / Low

Islamic/reliability understanding:
High / Medium / Low

AI opportunity:
High / Medium / Low

Measurability:
High / Medium / Low

Technical feasibility:
High / Medium / Low

Overall evidence maturity:
High / Medium / Low


## 37. Current Recommendation

PROCEED TO MORE RESEARCH

or

PROCEED TO SOLUTION EXPLORATION

or

HOLD

or

MERGE WITH P-XXX

or

REJECT


## 38. Reason for Recommendation

Evidence-based explanation only.


## 39. Required Next Actions

1.

2.

3.


## 40. Change Log

Date:

Change:

Reason:

Agent:
```

---

# 6. Problem Title Standard

Titles must describe the problem rather than the imagined product.

Bad:

> AI Islamic Research Copilot

Better:

> Islamic Content Creators Lose Time Verifying and Reconnecting Claims to Primary Sources

Bad:

> Smart Convert Assistant

Better:

> New Muslims Struggle to Understand Unfamiliar Islamic Terminology During Early Learning

---

# 7. One-Sentence Problem Statement

Use this formula:

```text
[Specific user] struggles to [complete important task]
because [core friction],
resulting in [meaningful consequence].
```

Example:

> English-speaking new Muslims struggle to follow introductory Islamic educational material because common Arabic terminology is introduced inconsistently or without context, resulting in confusion and repeated external searching.

The problem statement must not contain the solution.

Bad:

> New Muslims need an AI assistant that translates Islamic terminology.

This already assumes a solution.

---

# 8. Primary User

Avoid broad categories.

Bad:

> Muslims

Better:

> English-speaking Muslims who converted within the past two years and are independently learning foundational Islamic concepts online.

Another good example:

> Arabic-speaking Islamic content creators preparing short educational social-media content several times per week.

Specific users allow better evidence and better product decisions.

---

# 9. Secondary Users

Some problems involve multiple stakeholders.

Examples:

- student;
    
- teacher;
    
- scholar;
    
- editor;
    
- mosque;
    
- translator;
    
- content creator;
    
- reviewer;
    
- institution.
    

The card should identify:

> Who directly experiences the problem?

and:

> Who experiences consequences from the problem?

Do not combine different users into one persona if their workflows differ.

---

# 10. Job to Be Done

Use a behavioral formulation.

```text
When [situation],
I want to [motivation/task],
so that [desired outcome].
```

Example:

> When preparing a short educational post about a religious topic, I want to quickly verify each major claim against trustworthy original sources so that I can publish confidently without misrepresenting Islamic material.

---

# 11. Current Workflow

The workflow is one of the most important parts of the card.

Do not write vague descriptions such as:

> User searches online and researches.

Reconstruct actual steps.

Example:

```text
Topic assigned
↓
Search Google
↓
Search trusted Islamic websites
↓
Open several results
↓
Read Arabic material
↓
Compare explanations
↓
Verify hadith
↓
Copy useful passages
↓
Write draft
↓
Return to browser to recover lost citation
↓
Check wording
↓
Publish
```

This reveals intervention points.

---

# 12. Workflow Evidence

Every reconstructed workflow should identify how much of it is actually known.

Use:

```text
DIRECTLY OBSERVED

USER REPORTED

INFERRED

UNKNOWN
```

Example:

```text
Step 1 — USER REPORTED
Step 2 — USER REPORTED
Step 3 — DIRECTLY OBSERVED
Step 4 — INFERRED
Step 5 — UNKNOWN
```

Do not present inferred workflows as fully validated.

---

# 13. Core Pain

The pain must describe what is difficult.

Avoid generic phrases:

> Research is hard.

Prefer:

> The creator repeatedly leaves the drafting environment to rediscover the primary source behind copied notes, creating additional search steps and increasing the possibility of publishing a claim without traceable provenance.

Specific pain is actionable.

---

# 14. Root Cause vs Symptom

Distinguish:

### Symptom

> Users repeatedly ask the same questions.

### Possible root cause

> Existing educational material assumes terminology that beginners do not understand.

Do not assume the first explanation is the root cause.

Record alternative hypotheses where relevant.

---

# 15. Consequences

A painful workflow step may not be important unless it creates meaningful consequences.

Potential consequences include:

- wasted time;
    
- abandonment;
    
- religious misinformation;
    
- incorrect citations;
    
- misunderstanding;
    
- need for repeated expert intervention;
    
- low confidence;
    
- inaccessible learning;
    
- duplicated effort.
    

Document evidence where possible.

---

# 16. Frequency and Severity Must Remain Separate

Example:

Problem A:

> Happens every day but costs 30 seconds.

Problem B:

> Happens twice per year but could result in serious religious misinformation.

These are different opportunity profiles.

Do not collapse them into one vague rating.

---

# 17. Existing Workarounds

Workarounds reveal unmet need.

Examples:

- manually opening several websites;
    
- asking a knowledgeable friend;
    
- keeping spreadsheets;
    
- copying links into notes;
    
- avoiding the topic;
    
- using generic AI and verifying afterward;
    
- paying a translator;
    
- searching Arabic terms manually.
    

Workarounds are often strong evidence that the underlying job matters.

---

# 18. Existing Solutions

Research competitors before claiming a gap.

Do not merely list names.

Understand:

- what they solve;
    
- who they serve;
    
- how they work;
    
- what users like;
    
- what remains difficult.
    

If another solution already solves the problem well, say so.

---

# 19. Problem Gap vs Product Gap

The card must explicitly answer:

> Is this a meaningful unsolved user problem, or merely a feature missing from one product?

Example:

Feature gap:

> App X has no voice mode.

Problem gap:

> visually impaired users cannot effectively complete the workflow because all available tools rely on inaccessible text interaction.

Only the second demonstrates a user problem.

---

# 20. Evidence Section

Do not paste an unstructured citation list.

Each evidence item should say what it proves.

Example:

```text
EVID-021

Source:
App-store reviews for Product X.

Finding:
Multiple reviewers report difficulty identifying sources behind answers.

Strength:
Moderate

Supports:
Source-transparency pain.

Does NOT establish:
How widespread the issue is across the wider Muslim population.
```

---

# 21. Contradicting Evidence

Every serious Problem Card should preserve evidence that weakens it.

Example:

```text
EVID-033

Finding:
Product Y already provides sentence-level citations.

Impact:
Weakens the hypothesis that claim-level provenance is entirely unavailable.

Remaining question:
Whether users find Product Y's implementation sufficient.
```

Do not hide this.

---

# 22. Disconfirmation Search

Each Problem Card should attempt to answer:

> What evidence would cause us to stop pursuing this problem?

Possible answers:

- users rarely experience it;
    
- existing products solve it;
    
- users do not care;
    
- AI makes the task less trustworthy;
    
- the solution requires unavailable data;
    
- the target population is too small for the challenge.
    

Agents should intentionally search for those conditions.

---

# 23. Islamic Reliability Section

This section is mandatory when religious information is involved.

The card should identify whether the problem touches:

- Qur'anic interpretation;
    
- hadith;
    
- fiqh;
    
- fatwa;
    
- scholarly disagreement;
    
- personal circumstances;
    
- Islamic terminology;
    
- religious education;
    
- source attribution.
    

Do not defer Islamic reliability until after the product is designed.

It may fundamentally shape whether the opportunity is viable.

---

# 24. AI Leverage Is a Hypothesis

At the Problem Card stage, AI is not yet the assumed solution.

Write:

> Potential AI leverage

rather than:

> AI solution.

Potential leverage may include:

- semantic retrieval;
    
- cross-language retrieval;
    
- source matching;
    
- classification;
    
- summarization;
    
- contextual explanation;
    
- natural-language navigation;
    
- document extraction;
    
- speech processing.
    

These remain hypotheses until validated.

---

# 25. Non-AI Baseline Is Mandatory

Every card with an AI opportunity must answer:

> Could this be solved better without AI?

Possible baselines:

- improved search;
    
- curated database;
    
- deterministic filters;
    
- taxonomy;
    
- static glossary;
    
- structured forms;
    
- human service;
    
- ordinary software.
    

A problem is not automatically an AI problem.

---

# 26. Intervention Point

The eventual solution should ideally improve a specific point in the workflow.

Example:

```text
Current workflow:

Research
↓
Draft
↓
Lose source connection
↓
Search again
↓
Verify
```

Possible intervention:

```text
Research
↓
CAPTURE CLAIM + SOURCE CONNECTION AUTOMATICALLY
↓
Draft
↓
Verify directly
```

The card should identify this point without fully designing the product.

---

# 27. Measurement

The Problem Card must identify what measurable outcome might improve.

Examples:

- research time;
    
- number of manual searches;
    
- source verification accuracy;
    
- task completion;
    
- number of unsupported claims;
    
- comprehension score;
    
- translation fidelity;
    
- expert review time.
    

Do not invent expected performance.

---

# 28. Before / After Must Remain Hypothetical

At this stage, the "after" state is an opportunity hypothesis.

Do not write:

> Research time will decrease by 80%.

unless actual testing exists.

Write:

> Research time could potentially be reduced; baseline and improvement require testing.

---

# 29. Demo Potential

Hackathon projects benefit from problems whose improvement can be shown clearly.

However:

Do not reject an important problem merely because the demo is less visually dramatic.

Demo potential is one factor.

Problem quality comes first.

---

# 30. Technical Questions

Technical feasibility should be explored enough to identify major blockers.

Do not fully architect the solution yet.

Useful questions include:

- Does necessary data exist?
    
- Can it legally be used?
    
- Is Arabic processing adequate?
    
- Is retrieval possible?
    
- Could the required system run within hackathon constraints?
    
- Is evaluation possible?
    

Mark unknowns.

---

# 31. Adoption

A solution no one will use is weak.

The card should identify possible barriers such as:

- distrust of AI;
    
- workflow switching;
    
- account creation;
    
- source preferences;
    
- institutional policies;
    
- cost;
    
- connectivity;
    
- language.
    

Use evidence where available.

---

# 32. Assumptions

Any material assumption must be explicit.

Example:

```text
[ASSUMPTION]
Content creators would prefer integrated provenance over manually maintaining their current note-taking system.
```

This assumption can later become a validation question.

---

# 33. Unknowns

Unknowns should not be hidden.

Example:

```text
[UNKNOWN]
How much time Islamic content creators currently spend on source verification per published item.
```

Unknowns help define the next research round.

---

# 34. Evidence Gaps

Not every unknown deserves immediate research.

Evidence gaps should identify unknowns that materially affect the decision.

Example:

> We do not know whether creators actually consider this one of their top three workflow frustrations.

This is decision-changing.

---

# 35. Decision-Changing Questions

Every promising card should identify questions that could change its status.

Example:

```text
QUESTION:
Do existing Islamic research tools already provide sufficiently reliable cross-source retrieval?

YES:
The opportunity may become weak or need substantial reframing.

NO:
The gap remains credible.
```

These questions help the research team spend time efficiently.

---

# 36. Confidence Must Be Multi-Dimensional

Avoid:

> Overall confidence: High

when only part of the problem is understood.

Example:

```text
Problem existence:
High

Frequency:
Low

Severity:
Medium

Gap:
Medium

AI relevance:
Low
```

This tells the Research Director what still requires investigation.

---

# 37. Evidence Maturity

Use:

## Level 0 — Speculation

Problem imagined but not evidenced.

## Level 1 — Signal

Initial evidence exists.

## Level 2 — Pattern

Multiple independent signals suggest recurrence.

## Level 3 — Validated Problem

Problem, user, workflow, consequence, and solution gap have credible support.

## Level 4 — Solution-Ready

Problem is sufficiently understood to begin serious solution design and evaluation planning.

---

# 38. Status Definitions

## UNVALIDATED

Interesting but insufficient evidence.

## PROMISING

Evidence is encouraging but meaningful uncertainty remains.

## VALIDATED

Evidence strongly supports continued solution exploration.

## WEAK

Available evidence suggests low importance, weak gap, or poor fit.

## REJECTED

Evidence indicates the opportunity should not currently proceed.

---

# 39. Rejected Cards Must Be Preserved

Never delete rejected Problem Cards.

Add:

```text
STATUS:
REJECTED

REJECTION REASON:

DATE:

EVIDENCE:
```

Rejected problems prevent future agents from repeating the same research.

---

# 40. Merging Duplicate Problems

Agents may discover similar problems.

Do not immediately merge them.

First determine whether:

- users differ;
    
- workflow differs;
    
- root causes differ;
    
- consequences differ.
    

Example:

> Convert terminology confusion

may be different from:

> Multilingual translation loss for experienced students.

Similar technology does not mean identical problems.

---

# 41. Splitting Overly Broad Problems

Broad cards should be split.

Too broad:

> Muslims cannot find trustworthy information online.

Possible specific problems:

- converts cannot evaluate conflicting search results;
    
- creators lose provenance during research;
    
- users cannot identify scholarly disagreement;
    
- non-Arabic users misunderstand untranslated technical terms.
    

Each may require different evidence and solutions.

---

# 42. One Problem Card Should Represent One Core Problem

A card should not become:

> everything wrong with Islamic technology.

If the card contains several different jobs or workflows, split it.

---

# 43. User Group Separation

Do not combine:

- new Muslims;
    
- scholars;
    
- general public;
    
- content creators;
    
- researchers;
    

merely because all need Islamic knowledge.

Their tasks are substantially different.

---

# 44. Problem Cards Are Living Documents

Cards may change as evidence improves.

Updates may:

- narrow the user;
    
- revise the workflow;
    
- downgrade confidence;
    
- add competitors;
    
- split the problem;
    
- reject the problem;
    
- promote it.
    

Use the change log.

---

# 45. Do Not Rewrite History

When an important assumption is disproved, record it.

Example:

```text
CHANGE:

Previous assumption:
No existing product provides sentence-level citations.

New evidence:
Product X introduced sentence-level citations in June 2026.

Impact:
Gap narrowed; Problem Card downgraded from VALIDATED to PROMISING.
```

This improves research integrity.

---

# 46. Research Director Review

Before a Problem Card enters final synthesis, the Research Director should check:

```text
Is the user specific?

Is the task real?

Is the workflow evidenced?

Is the pain precise?

Is the consequence meaningful?

Are competitors researched?

Is the gap real?

Is contradictory evidence included?

Are religious risks understood?

Is AI optional rather than assumed?

Is a non-AI baseline present?

Can improvement be measured?

Are uncertainties visible?
```

---

# 47. Red-Team Review

Promising cards should eventually be reviewed by the Red-Team agent.

The Red-Team should ask:

- Is this problem exaggerated?
    
- Is the evidence cherry-picked?
    
- Are users representative?
    
- Is this already solved?
    
- Is AI unnecessary?
    
- Could the proposed direction cause religious harm?
    
- Would people actually use it?
    
- Is the measurement weak?
    
- Is the card hiding contradictions?
    

Record the review.

---

# 48. Source-Boundary Review

Cards involving Islamic information should be reviewed for:

- source scope;
    
- scholarly disagreement;
    
- attribution;
    
- escalation;
    
- unsafe generalization.
    

Use the designated Source Boundary & Disagreement Researcher where available.

---

# 49. Problem Card Quality Standard

A high-quality Problem Card allows a new researcher to understand:

> who the user is;

> what the user is trying to do;

> what they currently do;

> exactly where the difficulty occurs;

> what consequences result;

> what evidence proves it;

> what evidence weakens it;

> how current tools address it;

> what remains unresolved;

> whether AI may be justified;

> what still needs validation.

If this cannot be understood from the card, it is incomplete.

---

# 50. Minimal Problem Card

During early discovery, agents may use this shortened version before expanding the card:

```text
# [P-XXX] Title

USER:

JOB TO BE DONE:

CURRENT WORKFLOW:

CORE PAIN:

CONSEQUENCE:

SUPPORTING EVIDENCE:

CURRENT SOLUTIONS:

REMAINING GAP:

DISCONFIRMING EVIDENCE:

POTENTIAL AI LEVERAGE:

NON-AI ALTERNATIVE:

MEASUREMENT:

KEY UNKNOWN:

STATUS:

CONFIDENCE:
```

Only promising findings need to be expanded into the complete schema.

---

# 51. Promotion from Minimal to Full Card

Expand a minimal card when:

- evidence begins converging;
    
- the problem survives initial disconfirmation;
    
- a meaningful solution gap appears;
    
- another agent needs to evaluate it;
    
- it may enter cross-examination.
    

Do not spend large amounts of time fully documenting clearly weak findings.

---

# 52. Problem Cards Are Not Pitch Decks

Avoid:

- marketing slogans;
    
- exaggerated market claims;
    
- product names;
    
- flashy features;
    
- unsupported impact claims.
    

A Problem Card should read like research.

Not sales material.

---

# 53. Strong Problem Card Example Structure

A strong card may ultimately establish:

```text
USER:
English-speaking new Muslim.

TASK:
Understand an introductory lesson containing Arabic religious terminology.

WORKFLOW:
Watch lesson → encounter unfamiliar word → pause → search Google →
open several explanations → compare terminology → return to lesson.

PAIN:
Learning repeatedly fragments into external searches.

EVIDENCE:
Recurring convert reports + educational research + product observations.

CURRENT SOLUTIONS:
Glossaries, search engines, Islamic Q&A websites.

GAP:
Explanations are disconnected from the immediate learning context.

AI LEVERAGE:
Potential contextual explanation and retrieval.

NON-AI BASELINE:
Interactive glossary linked to structured curriculum.

MEASUREMENT:
Time to correctly understand term + comprehension accuracy.

UNKNOWN:
Whether users prefer inline explanations over existing search behavior.
```

This is sufficiently concrete to investigate further without prematurely deciding what to build.

---

# 54. Weak Problem Card Example

```text
USER:
Muslims.

PROBLEM:
Islamic knowledge is difficult.

SOLUTION:
AI chatbot.

EVIDENCE:
People use ChatGPT.

IMPACT:
Huge.

STATUS:
Validated.
```

This card should be rejected.

It lacks:

- user specificity;
    
- workflow;
    
- pain precision;
    
- evidence;
    
- competitor analysis;
    
- gap;
    
- disconfirmation;
    
- measurement.
    

---

# 55. Final Problem Card Principle

A good Problem Card does not try to make the problem sound impressive.

It makes the problem **understandable and testable**.

The card should survive the questions:

> Is this real?

> Who experiences it?

> Where exactly does it happen?

> Why does it matter?

> What proves that?

> What already solves it?

> What remains unresolved?

> Could something simpler solve it?

> Would AI genuinely help?

> How would we know if we improved it?

Only after those questions can be answered should the team move from:

**problem discovery**

to:

**solution design**.