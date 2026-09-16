## Islamic AI Challenge — Reference Project Research Schema

This document defines how agents must research, document, compare, and evaluate existing products, projects, systems, repositories, academic prototypes, and adjacent-domain solutions.

The purpose is not merely to build a competitor list.

The purpose is to determine:

- what already exists;
    
- which user problems are already solved;
    
- how existing systems approach the problem;
    
- what users value;
    
- where existing systems fail;
    
- whether an apparent opportunity is genuinely unresolved;
    
- which design patterns can be transferred from other domains;
    
- what technical or product lessons can be learned.
    

This document supplements:

- `AGENTS.md`
    
- `research-protocol/source-policy.md`
    
- `research-protocol/evidence-standard.md`
    
- `research-protocol/problem-card-schema.md`
    

---

# 1. Core Principle

Never assume a problem is unsolved because the team has not encountered a solution.

For every promising problem, actively search for systems that may already address it.

The required question is not:

> “Can we find competitors?”

It is:

> “What has already been attempted, how well does it solve the underlying user problem, and what remains genuinely unresolved?”

---

# 2. What Counts as a Reference Project

A Reference Project may be:

- a commercial product;
    
- a nonprofit platform;
    
- an Islamic application;
    
- an Islamic website;
    
- an AI product;
    
- an open-source repository;
    
- a research prototype;
    
- an academic project;
    
- an institutional system;
    
- a government platform;
    
- an abandoned product;
    
- a failed startup;
    
- an adjacent-domain tool;
    
- a manual service with relevant workflow design.
    

The project does not need to use AI.

Non-AI systems may provide important baselines.

---

# 3. Reference Project Categories

Every project should be classified.

Use one or more of:

```text
DIRECT COMPETITOR

PARTIAL COMPETITOR

ADJACENT ISLAMIC PROJECT

ADJACENT-DOMAIN REFERENCE

TECHNICAL REFERENCE

UX / WORKFLOW REFERENCE

RESEARCH PROTOTYPE

OPEN-SOURCE PROJECT

ABANDONED / DISCONTINUED PROJECT

MANUAL / HUMAN SERVICE

NON-AI BASELINE
```

---

# 4. Direct Competitor

A Direct Competitor:

- targets substantially the same user;
    
- addresses substantially the same job;
    
- attempts to solve substantially the same core problem.
    

Example:

If the problem is:

> Islamic researchers struggle to retrieve trustworthy passages with traceable sources.

A system designed specifically for Islamic scholarly semantic search may qualify as a direct competitor.

---

# 5. Partial Competitor

A Partial Competitor solves part of the workflow.

Example:

A general Islamic search engine might solve retrieval but not:

- provenance preservation;
    
- disagreement mapping;
    
- drafting;
    
- source comparison.
    

Partial competitors are important because several existing tools together may already solve most of the problem.

---

# 6. Adjacent Islamic Project

An Adjacent Islamic Project operates in the Islamic domain but solves a different problem whose design, source methodology, or technology is relevant.

Examples may include:

- Qur'an search tools;
    
- hadith databases;
    
- Islamic learning platforms;
    
- fatwa archives;
    
- Arabic NLP systems;
    
- Islamic content applications.
    

---

# 7. Adjacent-Domain Reference

An Adjacent-Domain Reference solves a structurally similar problem outside the Islamic domain.

Priority domains may include:

- medicine;
    
- law;
    
- scientific research;
    
- journalism;
    
- education;
    
- compliance;
    
- finance;
    
- fact checking;
    
- academic search;
    
- knowledge management;
    
- translation.
    

These references are especially valuable for high-trust problems.

---

# 8. Why Adjacent-Domain Projects Matter

Many strong product patterns may already exist elsewhere.

Examples:

```text
Islamic source verification
↔
medical evidence retrieval
```

```text
scholarly disagreement visualization
↔
legal precedent comparison
```

```text
religious claim provenance
↔
scientific citation tracing
```

```text
convert learning journeys
↔
adaptive educational systems
```

Agents should look for transferable mechanisms, not superficial similarity.

---

# 9. Reference Project IDs

Assign stable IDs.

Use:

```text
RP-001
RP-002
RP-003
```

Adjacent-domain projects may optionally use:

```text
ADJ-001
ADJ-002
```

Technical references may optionally use:

```text
TECH-001
```

Once assigned, do not reuse IDs.

---

# 10. File Naming

Use:

```text
RP-XXX-project-name.md
```

Examples:

```text
RP-003-islamic-search-platform.md

RP-011-evidence-retrieval-system.md

ADJ-004-medical-clinical-evidence-tool.md
```

Avoid:

```text
competitor1.md
good-app.md
reference-final.md
```

---

# 11. Required Reference Project Template

Every meaningful reference project should follow this structure.

```text
# [RP-XXX] Project Name

## 1. Classification

Category:

Direct / Partial / Adjacent / Technical / Research / Other

Related Problem Cards:

Research owner:

Review date:

Last updated:


## 2. Basic Information

Project name:

Organization / creator:

Official URL:

Repository URL:

Documentation URL:

Launch date:

Current status:

Country / region:

Primary language(s):


## 3. Target User

Primary user:

Secondary users:

User skill level:

Geography:

Language:

Relevant context:


## 4. Problem Addressed

What problem does the project claim to solve?

What user job does it support?

Which part of the workflow does it address?


## 5. Core User Workflow

Trigger:

Step 1:

Step 2:

Step 3:

...

Outcome:


## 6. Core Features

Feature 1:

Feature 2:

Feature 3:

Feature 4:


## 7. Technical Approach

AI used:
Yes / No / Unknown

Models:

Retrieval:

RAG:

Knowledge graph:

Search:

Database:

Speech:

Computer vision:

Translation:

Other:

Evidence source:


## 8. Data / Knowledge Sources

What data does the system use?

Are sources disclosed?

Are primary sources available?

Is provenance visible?

How are sources curated?

Licensing known?

Update process known?


## 9. Islamic Source Methodology

Applicable:
Yes / No

Islamic corpus:

Scholars / institutions:

Source attribution:

Handling of disagreement:

Handling of uncertainty:

Handling of personal fatwa questions:

Human review:

Source limitations:


## 10. Trust and Safety Mechanisms

Citation system:

Refusal behavior:

Uncertainty display:

Escalation:

Fact checking:

Source tracing:

Moderation:

Human oversight:

Known limitations:


## 11. User Experience

Primary interaction model:

Search:

Chat:

Voice:

Browse:

Learning journey:

Dashboard:

Other:

Key UX strengths:

Key UX weaknesses:


## 12. What It Does Well

1.

2.

3.

Evidence:


## 13. Known Limitations

1.

2.

3.

Evidence:


## 14. User Feedback

Positive themes:

Negative themes:

Recurring complaints:

Feature requests:

Platforms reviewed:

Number of relevant samples where known:

Selection method:

Limitations:


## 15. Vendor Claims

Claim:

Source:

Independent validation available:
Yes / No

Assessment:


## 16. Independent Evidence

Source:

Finding:

Strength:

What it establishes:


## 17. Project Maturity

Prototype / Beta / Production / Unknown

Active users known?

Usage scale known?

Funding known?

Institutional adoption known?

Evidence:


## 18. Project Activity

For software/open-source projects:

Last release:

Recent commits:

Open issues:

Maintenance activity:

Archived:
Yes / No

Current status:

Evidence:


## 19. Business / Access Model

Free:

Paid:

Subscription:

Institutional:

Open source:

Closed source:

Account required:

Geographic restrictions:

Other:


## 20. Strength Against Our Problem

Which parts of our Problem Card does this already solve?

Problem component:

Coverage:
Strong / Partial / Weak / None

Evidence:


## 21. Remaining Gap

What does the project NOT solve?

Is this gap meaningful to users?

Evidence:

Could the missing capability already exist elsewhere?


## 22. Does This Weaken Our Opportunity?

YES / PARTIALLY / NO / UNCLEAR

Explanation:

Affected Problem Cards:


## 23. Does This Strengthen Our Opportunity?

YES / PARTIALLY / NO / UNCLEAR

Explanation:

Example:
Existing adoption may prove users value the underlying task.


## 24. Transferable Lessons

Product lesson:

Technical lesson:

UX lesson:

Trust / safety lesson:

Source methodology lesson:

Evaluation lesson:


## 25. What Should NOT Be Copied

Pattern:

Why it should not transfer:

Evidence:


## 26. Potential Differentiation

If our project addressed the same problem, what genuinely meaningful difference could remain?

Difference:

Why users may care:

Evidence:

Is this differentiation substantive or cosmetic?


## 27. AI Necessity Comparison

Does this project use AI?

If yes:
What does AI accomplish?

If no:
How effectively is the problem solved without AI?

Lesson for our project:


## 28. Evaluation Approach

Does the project report evaluation?

Metrics:

Dataset:

Human evaluation:

User testing:

Benchmark:

Results:

Limitations:


## 29. Demo / Presentation Lessons

What does the project demonstrate well?

What makes its value understandable?

What can we learn about presenting our own workflow?


## 30. Risks

Religious:

Technical:

Privacy:

Bias:

Hallucination:

Trust:

Adoption:

Other:


## 31. Evidence Summary

Evidence supporting capabilities:

Evidence supporting limitations:

Contradictory evidence:

Confidence:


## 32. Open Questions

1.

2.

3.


## 33. Final Relevance

HIGH / MEDIUM / LOW

Why:


## 34. Research Recommendation

DEEPER REVIEW

MONITOR

USE AS REFERENCE

USE AS BASELINE

SIGNIFICANT COMPETITOR

WEAKENS PROBLEM

NO FURTHER RESEARCH


## 35. Change Log

Date:

Change:

Reason:

Agent:
```

---

# 12. Research Required for Each Promising Problem

For each serious Problem Card, agents should attempt to identify:

- at least several direct or partial competitors where they exist;
    
- Islamic-domain references;
    
- adjacent-domain references;
    
- technical references where relevant;
    
- non-AI alternatives.
    

Do not invent projects merely to satisfy a quota.

Quality takes precedence over count.

---

# 13. Recommended Search Coverage

For a strong opportunity, aim where practical to investigate:

```text
3+ direct or partial solutions

2+ adjacent-domain systems

1+ relevant open-source or technical implementation

1+ research or academic prototype where applicable

1+ non-AI baseline
```

This is guidance, not a rigid requirement.

If only one meaningful project exists, document that honestly.

---

# 14. Existing Products Must Be Tested Against the Problem

Do not ask:

> Does Product X have AI?

Ask:

> Does Product X already allow the user to successfully complete the job described in P-XXX?

Feature lists are secondary.

User problem coverage is primary.

---

# 15. Workflow Comparison

Compare workflows rather than only features.

Example:

```text
CURRENT USER WORKFLOW

Search Google
→ Open 8 pages
→ Compare
→ Save sources
→ Draft
```

```text
REFERENCE PROJECT WORKFLOW

Ask query
→ Receive passages
→ Inspect citations
→ Export notes
```

This reveals true value better than:

| Feature | Product A | Product B |

Feature tables may still be used later.

---

# 16. Capability Claims Must Be Verified

If a website states:

> “Provides reliable Islamic answers”

record this as:

> `[VENDOR CLAIM]`

Then investigate:

- actual citations;
    
- source transparency;
    
- test queries;
    
- documentation;
    
- independent reviews;
    
- user complaints.
    

Do not promote marketing language into research fact.

---

# 17. Inspect the Actual Product Where Possible

When access permits, investigate the real product rather than relying entirely on descriptions.

Record:

```text
TEST DATE:

TEST SCENARIO:

INPUT:

OBSERVED OUTPUT:

SOURCE BEHAVIOR:

FAILURE:

NOTES:
```

Do not claim first-hand testing when the product was not actually accessed.

---

# 18. Use Realistic Test Scenarios

Test scenarios should reflect the Problem Card.

Bad:

> “What is Islam?”

Better:

> A content creator needs three source-backed passages related to a specific topic while preserving attribution.

Test the actual workflow.

---

# 19. Islamic Project Testing

For Islamic AI products, useful test categories may include:

- straightforward source retrieval;
    
- ambiguous wording;
    
- requests for evidence;
    
- scholarly disagreement;
    
- unsupported premise;
    
- personal fatwa question;
    
- multilingual query;
    
- Arabic source retrieval;
    
- out-of-scope request.
    

Do not attempt high-risk testing merely for spectacle.

The objective is to understand system boundaries.

---

# 20. User Reviews

When analyzing reviews, separate:

### Product Satisfaction

General praise or dissatisfaction.

### Workflow Evidence

Specific descriptions of how the user uses the product.

### Problem Evidence

Specific pain points.

### Feature Requests

Requested capabilities.

### Reliability Evidence

Claims about incorrect answers, citations, trust, or safety.

Specific feedback is more useful than star ratings alone.

---

# 21. Review Sampling

Where possible, record:

```text
Platform:

Date range:

Number reviewed:

Search method:

Relevant reviews:

Positive themes:

Negative themes:

Reliability themes:

Limitations:
```

Avoid selecting only complaints supporting our hypothesis.

---

# 22. App Store Ratings

Ratings may provide useful high-level information but should not be overinterpreted.

A 4.8 rating does not establish:

> the system solves our specific problem.

Likewise, a 2.5 rating may reflect unrelated technical issues.

Inspect detailed reviews.

---

# 23. GitHub Research

For open-source repositories inspect, where relevant:

- README;
    
- license;
    
- architecture;
    
- issues;
    
- releases;
    
- contribution history;
    
- latest commits;
    
- stars/forks as secondary indicators;
    
- dependencies;
    
- model usage;
    
- data sources.
    

Do not use GitHub stars as the main measure of project quality.

---

# 24. Repository Activity

Classify:

```text
ACTIVE

LOW ACTIVITY

DORMANT

ARCHIVED

ABANDONED

UNKNOWN
```

Base the classification on observable activity.

Do not infer abandonment from one quiet month.

---

# 25. Abandoned Projects Are Valuable

Actively investigate abandoned or discontinued projects where identifiable.

Ask:

- Why did they stop?
    
- Was adoption weak?
    
- Was maintenance expensive?
    
- Did data access fail?
    
- Were users uninterested?
    
- Did technology fail?
    
- Was funding lost?
    

Failure patterns can prevent repeating mistakes.

---

# 26. Do Not Invent Failure Reasons

A dead repository does not prove:

> users did not want the product.

Possible reasons include:

- developer moved on;
    
- private continuation;
    
- lack of funding;
    
- technical difficulty.
    

Record only supported explanations.

Use:

> `[CAUSE OF DISCONTINUATION UNKNOWN]`

where necessary.

---

# 27. Academic Prototypes

Academic systems may be technically sophisticated but not production-ready.

Research:

- purpose;
    
- dataset;
    
- methodology;
    
- evaluation;
    
- user testing;
    
- source code;
    
- limitations.
    

Do not assume successful benchmark results imply product-market success.

---

# 28. Research Prototypes Can Reveal Technical Feasibility

An academic project may demonstrate that:

- multilingual retrieval is possible;
    
- Arabic embeddings work;
    
- citation verification can be automated;
    
- knowledge graphs improve retrieval.
    

This can materially strengthen technical feasibility even if the prototype itself has no users.

---

# 29. Adjacent-Domain Reference Criteria

Choose adjacent systems based on structural similarity.

Good adjacent comparison:

> Islamic ruling research ↔ legal research platform

because both involve:

- authoritative corpora;
    
- source hierarchy;
    
- contextual interpretation;
    
- conflicting authorities;
    
- citation provenance.
    

Weak adjacent comparison:

> Islamic research app ↔ food delivery app

unless a specific workflow pattern genuinely transfers.

---

# 30. Transferability Analysis

For every adjacent project, explicitly classify lessons as:

```text
DIRECTLY TRANSFERABLE

TRANSFERABLE WITH ADAPTATION

CONTEXT-SPECIFIC

NOT TRANSFERABLE
```

Explain why.

---

# 31. Domain Differences Matter

A medical solution cannot automatically be transferred into an Islamic context.

Differences may include:

- authority structures;
    
- source interpretation;
    
- terminology;
    
- accountability;
    
- user expectations;
    
- privacy;
    
- consequences of errors.
    

Document both similarity and difference.

---

# 32. Feature Matrices Are Secondary

Feature comparison may be useful later.

Example:

|Capability|Product A|Product B|Product C|
|---|---|---|---|
|Source citations|Yes|Partial|No|
|Arabic|Yes|Yes|No|
|Disagreement handling|No|Partial|No|

However, a feature matrix does not answer:

> whether users successfully complete the task.

Use workflow and outcome analysis alongside it.

---

# 33. Problem Coverage Matrix

A more useful comparison is:

|Problem Component|Product A|Product B|Product C|
|---|---|---|---|
|Discover source|Strong|Strong|Partial|
|Verify attribution|Weak|Strong|None|
|Compare positions|None|Partial|None|
|Preserve provenance during drafting|None|None|Partial|

This helps expose remaining gaps.

---

# 34. User Segment Coverage

A product may solve the problem for one user but not another.

Example:

A scholarly Arabic search platform may work well for:

> Arabic-speaking advanced students

but poorly for:

> English-speaking converts.

Do not label the entire problem solved without checking user fit.

---

# 35. Language Coverage

For Islamic projects, inspect:

- Arabic quality;
    
- English quality;
    
- multilingual support;
    
- terminology handling;
    
- transliteration;
    
- cross-language retrieval.
    

Marketing claims such as:

> “supports 50 languages”

do not establish equal quality across all languages.

---

# 36. Source Transparency

For knowledge systems, investigate:

- Are sources shown?
    
- Are citations specific?
    
- Can users open original material?
    
- Are citations claim-level or answer-level?
    
- Can the user distinguish quoted source from generated explanation?
    
- Are sources authoritative?
    
- Can provenance be exported?
    

These may be important differentiators.

---

# 37. Scholarly Disagreement Handling

For relevant Islamic systems inspect:

- Does the system acknowledge disagreement?
    
- Does it present one view as universal?
    
- Does it identify scholars?
    
- Does it preserve context?
    
- Does it escalate unclear cases?
    

This may materially affect trustworthiness.

---

# 38. Refusal and Escalation

Investigate whether the system can:

- refuse unsupported questions;
    
- admit insufficient evidence;
    
- redirect to qualified scholars;
    
- request additional context;
    
- identify high-risk topics.
    

Absence of these mechanisms may be a meaningful limitation.

---

# 39. Citation Accuracy

A system showing citations is not automatically trustworthy.

Where practical test:

- Does cited source exist?
    
- Does it support the claim?
    
- Is context preserved?
    
- Is the quoted text accurate?
    

Distinguish:

> citation presence

from:

> citation correctness.

---

# 40. Source Coverage

A reference project may rely on a narrow corpus.

Record:

- sources included;
    
- sources excluded;
    
- denomination/methodological scope where relevant;
    
- update process.
    

Corpus scope strongly affects what problems the system can solve.

---

# 41. User Trust

Research trust indicators such as:

- source transparency;
    
- institutional backing;
    
- scholar involvement;
    
- community reputation;
    
- user reviews;
    
- correction mechanisms.
    

Do not infer trust solely from brand recognition.

---

# 42. Correction Mechanisms

Strong reference systems may provide:

- feedback;
    
- report-error controls;
    
- expert review;
    
- version history;
    
- correction notices;
    
- audit trail.
    

These mechanisms may offer important design lessons.

---

# 43. Personalization

If a system personalizes content, inspect:

- what information it uses;
    
- whether sensitive religious attributes are inferred;
    
- whether users control personalization;
    
- privacy implications.
    

Do not assume personalization is automatically beneficial.

---

# 44. Privacy

Record whether the system appears to collect:

- account information;
    
- religious questions;
    
- personal circumstances;
    
- voice recordings;
    
- location;
    
- behavioral history.
    

Privacy may materially affect adoption.

---

# 45. Technical Architecture

Do not attempt reverse engineering without authorization.

Use:

- public documentation;
    
- repositories;
    
- papers;
    
- developer statements;
    
- observable product behavior.
    

If architecture is unknown, write:

> `UNKNOWN`

Do not invent likely stacks.

---

# 46. AI Model Identification

If a project uses AI, record models only when evidence exists.

Use:

```text
Model:
Verified / Claimed / Unknown
```

Do not infer a model based only on writing style.

---

# 47. RAG Claims

If a system claims RAG or source-grounding, investigate:

- corpus;
    
- retrieval method where documented;
    
- citation behavior;
    
- source fidelity;
    
- known hallucination behavior.
    

Do not treat “RAG-powered” as evidence of reliability.

---

# 48. Knowledge Graphs

If a project uses a knowledge graph, investigate:

- what entities/relationships are represented;
    
- source provenance;
    
- update process;
    
- how the graph affects user workflow.
    

Technology names alone are not meaningful differentiation.

---

# 49. Evaluation Quality

Projects may report strong metrics.

Assess:

- benchmark relevance;
    
- sample size;
    
- test set;
    
- human evaluators;
    
- baseline;
    
- methodology;
    
- reproducibility.
    

Vendor-created evaluations should be labeled accordingly.

---

# 50. Benchmark Relevance

A system scoring well on generic question-answering may still perform poorly on:

- Arabic Islamic texts;
    
- citation fidelity;
    
- disagreement;
    
- contextual fatwa boundaries.
    

Only relevant evaluation should support relevant claims.

---

# 51. Product Maturity

Classify maturity:

```text
CONCEPT

ACADEMIC PROTOTYPE

EARLY PROTOTYPE

BETA

PRODUCTION

MATURE PRODUCTION

DISCONTINUED

UNKNOWN
```

A concept competitor should not be treated as equal to a widely used production system.

---

# 52. Adoption Evidence

Possible adoption indicators include:

- published user numbers;
    
- institutional deployments;
    
- active communities;
    
- app downloads;
    
- review volume;
    
- repository usage;
    
- references by organizations.
    

Treat each indicator cautiously.

Downloads do not equal active users.

---

# 53. Business Model

Understand whether sustainability depends on:

- advertising;
    
- subscription;
    
- donations;
    
- institutional contracts;
    
- grants;
    
- open-source contribution.
    

Business model may explain design decisions and adoption barriers.

---

# 54. Accessibility

Inspect accessibility where relevant:

- screen-reader compatibility;
    
- voice input/output;
    
- mobile support;
    
- font readability;
    
- language;
    
- bandwidth;
    
- account requirements.
    

Accessibility gaps may expose meaningful opportunities.

---

# 55. Integration

Some workflows may require:

- browser extensions;
    
- CMS integration;
    
- note-taking tools;
    
- classroom systems;
    
- mobile apps;
    
- APIs.
    

A standalone product may fail even if its core feature is strong.

Study how reference projects fit existing workflows.

---

# 56. Switching Cost

Ask:

> Why would a user switch from their current tool?

Possible barriers:

- established habits;
    
- saved data;
    
- trust;
    
- institutional approval;
    
- learning curve;
    
- cost.
    

Differentiation must overcome switching cost.

---

# 57. Cosmetic vs Meaningful Differentiation

Cosmetic:

- different color scheme;
    
- another chatbot interface;
    
- slightly different branding.
    

Meaningful:

- substantially better provenance;
    
- dramatically faster workflow;
    
- access for an underserved language group;
    
- reliable disagreement mapping;
    
- measurable reduction in errors.
    

Agents must distinguish them.

---

# 58. Reference Projects May Eliminate an Opportunity

If an existing project solves the problem well, record that clearly.

Possible outcome:

```text
IMPACT ON P-012:
Strongly weakens opportunity.

Reason:
Existing tool already provides the required workflow with high user satisfaction.
```

This is successful research.

---

# 59. Existing Competition Can Also Validate Demand

A competitor may strengthen the case that:

- users care about the problem;
    
- users already pay for a solution;
    
- institutions adopt such tools.
    

Competition does not automatically invalidate an opportunity.

The question is whether a meaningful gap remains.

---

# 60. Saturated Market

If many strong products already serve the exact need, mark:

> `[SATURATED SOLUTION LANDSCAPE]`

Then identify whether:

- a specific underserved user remains;
    
- existing quality is inadequate;
    
- a new technical capability changes what is possible.
    

Do not force differentiation where none exists.

---

# 61. Empty Market

If few products exist, do not immediately assume opportunity.

Possible explanations:

- problem is ignored;
    
- problem is technically difficult;
    
- regulations prevent solutions;
    
- users do not care;
    
- willingness to pay is low;
    
- human service already suffices.
    

Investigate why the market is empty.

---

# 62. Failed Project Search

For promising opportunities, actively search:

```text
"[problem] startup discontinued"

"[product] shut down"

"[project] archived"

"[project] GitHub abandoned"

"[problem] failed product"

"[product] user complaints"
```

Failure analysis can be highly informative.

---

# 63. Failed Projects Should Have a Failure Card

When a failed project is highly relevant, add:

```text
## Failure Analysis

Observed failure:

Evidence:

Known cause:

Hypothesized cause:

What is verified?

What remains unknown?

Lesson:
```

Do not confuse correlation with cause.

---

# 64. Technical Reference Projects

Some projects matter only because they demonstrate a capability.

Example:

> Arabic semantic retrieval model.

Their card may focus more heavily on:

- dataset;
    
- benchmark;
    
- model;
    
- licensing;
    
- performance;
    
- limitations.
    

They do not need full product-market analysis if irrelevant.

---

# 65. UX Reference Projects

Some projects matter because of interaction design.

Examples:

- evidence visualization;
    
- source comparison;
    
- learning journeys;
    
- uncertainty interfaces.
    

Capture:

- information architecture;
    
- navigation;
    
- user decision support;
    
- trust signals.
    

Do not assume underlying technology must also be copied.

---

# 66. Evaluation Reference Projects

Some projects matter because they provide strong evaluation methods.

Capture:

- benchmark construction;
    
- human review process;
    
- metrics;
    
- test categories;
    
- error taxonomy.
    

These may be more valuable than their product features.

---

# 67. Islamic Source Reference Projects

For Islamic data systems, pay particular attention to:

- corpus provenance;
    
- authenticity metadata;
    
- Arabic text normalization;
    
- scholar attribution;
    
- cross-reference structure;
    
- licensing;
    
- update policies.
    

These may influence our eventual architecture.

---

# 68. Bin Baz Reference Use

If a project uses or indexes material from:

[https://binbaz.org.sa/](https://binbaz.org.sa/)

record:

- whether content is directly linked;
    
- whether source attribution is preserved;
    
- whether text is reproduced;
    
- whether licensing/usage terms are known;
    
- whether generated interpretations are distinguished from original material.
    

Do not assume use rights without verification.

---

# 69. Licensing

Record licenses where relevant.

For:

- code;
    
- datasets;
    
- text corpora;
    
- models;
    
- APIs.
    

Use:

```text
LICENSE:

COMMERCIAL USE:

MODIFICATION:

REDISTRIBUTION:

ATTRIBUTION REQUIRED:

UNKNOWN TERMS:
```

Licensing may eliminate otherwise attractive implementation strategies.

---

# 70. Data Availability

If a project depends on a proprietary corpus or API, record this.

Ask:

- can we access equivalent data?
    
- is scraping permitted?
    
- is an API available?
    
- are rate limits restrictive?
    

A reference project may not be reproducible.

---

# 71. Cost

Where relevant, note:

- subscription price;
    
- API cost;
    
- compute requirements;
    
- human review cost.
    

A technically strong approach may not be viable within hackathon constraints.

---

# 72. Performance

Do not state:

> Product X is fast.

Where possible, observe or document:

- latency;
    
- response time;
    
- retrieval speed.
    

If subjective, label it:

> `[OBSERVATION]`

---

# 73. Product Quality vs Research Value

A poorly designed product can still provide a valuable lesson.

A successful product can also contain patterns we should avoid.

Do not classify projects only as:

> good / bad.

Extract specific lessons.

---

# 74. Reference Project Evidence Strength

Each important conclusion should be supported.

Example:

```text
CLAIM:
Product X does not display claim-level citations.

EVIDENCE:
Direct product testing, 16 September 2026.

STRENGTH:
Strong.
```

Another:

```text
CLAIM:
Users dislike Product X citations.

EVIDENCE:
Three Reddit comments.

STRENGTH:
Weak to Moderate.
```

---

# 75. Unknown Capabilities

If documentation is unclear:

> `UNKNOWN`

Do not assume absence.

Example:

Bad:

> Product X does not support export.

Better:

> Export functionality was not identified in reviewed documentation or testing.

---

# 76. Search Failure Language

Use:

> “No evidence of feature X was found during this review.”

Do not automatically write:

> “Feature X does not exist.”

unless directly verified.

---

# 77. Date Every Product Review

Products change quickly.

Every card should contain:

```text
REVIEW DATE:
YYYY-MM-DD
```

Major capability observations should be understood as time-specific.

---

# 78. Version Awareness

Where available record:

- app version;
    
- API version;
    
- model version;
    
- repository commit/release.
    

This is particularly important for AI systems.

---

# 79. Screenshots and Artifacts

If permitted, agents may preserve:

- screenshots;
    
- demo links;
    
- architecture diagrams;
    
- benchmark tables.
    

Store them with clear attribution.

Do not use screenshots as a substitute for written analysis.

---

# 80. Reference Project Research Output

A high-quality reference analysis should allow another researcher to answer:

> What does this project actually do?

> Who uses it?

> Which problem does it solve?

> How does its workflow compare to ours?

> What evidence supports its strengths?

> What evidence supports its weaknesses?

> Does it weaken our opportunity?

> Does it validate demand?

> What can we learn?

> What should we avoid?

---

# 81. Minimal Reference Project Card

For early landscape research, use:

```text
# [RP-XXX] Project Name

URL:

CATEGORY:

TARGET USER:

PROBLEM:

CORE WORKFLOW:

CORE FEATURES:

AI USED:

SOURCE / DATA APPROACH:

WHAT IT DOES WELL:

KEY LIMITATIONS:

USER FEEDBACK:

RELATED PROBLEM CARD:

DOES IT WEAKEN OUR OPPORTUNITY?

KEY LESSON:

RELEVANCE:
High / Medium / Low
```

Only expand high-relevance references into full cards.

---

# 82. Promotion to Full Reference Card

Expand when:

- it directly competes;
    
- it materially changes our understanding;
    
- it provides an important technical pattern;
    
- it exposes major risks;
    
- it provides highly transferable design lessons.
    

Do not spend equal effort on every discovered product.

---

# 83. Comparison Set

Once several reference projects are researched, create a comparison set containing:

```text
PRIMARY PROBLEM:

TARGET USER:

REFERENCE PROJECTS:

DIRECT COMPETITORS:

ADJACENT REFERENCES:

NON-AI BASELINES:

KEY DIFFERENCES:

COMMON LIMITATIONS:

UNSOLVED REQUIREMENTS:

TRANSFERABLE PATTERNS:

MAJOR THREATS TO OUR OPPORTUNITY:
```

---

# 84. Common Limitation Analysis

Repeated limitations across products may indicate a difficult but valuable gap.

Example:

```text
Product A:
Poor provenance

Product B:
Poor provenance

Product C:
Poor provenance
```

Possible interpretation:

> Source provenance may be a persistent unresolved challenge.

But also investigate:

> Is it technically difficult?

> Do users care?

Repeated absence alone does not prove demand.

---

# 85. Convergent Design

If many successful projects independently adopt the same pattern, treat that as meaningful.

Examples:

- citation preview;
    
- confidence labels;
    
- progressive disclosure;
    
- human escalation.
    

Ask why the pattern appears repeatedly.

---

# 86. Divergent Design

If successful projects solve the same task differently, investigate:

- user differences;
    
- domain differences;
    
- technical trade-offs;
    
- trust models.
    

Do not prematurely choose one pattern.

---

# 87. Reference Project Bias

Research agents may become attached to impressive products.

Avoid:

> “We should copy Product X.”

Instead ask:

> “Which specific mechanism succeeds, under what conditions, and would those conditions apply to our user?”

---

# 88. Innovation Through Combination

Innovation may sometimes come from combining proven patterns.

Example:

```text
legal citation tracing
+
adaptive education
+
Islamic trusted corpus
```

This may create something new without requiring an entirely novel technical primitive.

But combination must still solve a validated problem.

---

# 89. Do Not Overfit to Competitors

Competitor research should inform the solution space.

It should not constrain imagination entirely.

A current market may reflect:

- old technology;
    
- poor incentives;
    
- inherited interface conventions.
    

After understanding existing approaches, remain open to fundamentally different workflows.

---

# 90. Reference Project Red-Team Questions

For each highly relevant project ask:

```text
Could users simply use this instead of anything we build?

What does it already do better than our hypothetical project?

What resources does it possess that we do not?

Why would someone switch?

Are we underestimating its capabilities?

Are we relying on outdated reviews?

Is our supposed differentiation actually meaningful?
```

---

# 91. Opportunity-Killing Test

A direct competitor may kill an opportunity if:

- it solves the same problem;
    
- for the same user;
    
- with strong quality;
    
- with accessible pricing;
    
- with high trust;
    
- with little remaining friction.
    

If so, record it.

Do not invent novelty to save the idea.

---

# 92. Opportunity-Pivot Test

A competitor may reveal that the true opportunity is narrower.

Example:

Original problem:

> Find Islamic answers.

Competitor finding:

> Many systems already answer questions.

Remaining gap:

> Users cannot understand why conflicting sources disagree.

This may produce a stronger Problem Card.

---

# 93. New Problems Discovered Through Competitors

Reference research may generate new problem hypotheses.

Record them separately.

Do not rewrite competitor observations directly into conclusions.

Use:

```text
[NEW PROBLEM HYPOTHESIS]

Observation:

Possible problem:

Evidence needed:
```

---

# 94. Research Director Synthesis

The Research Director should use reference-project research to identify:

- crowded areas;
    
- underserved user groups;
    
- repeated product weaknesses;
    
- proven UX patterns;
    
- technical feasibility;
    
- failed approaches;
    
- meaningful differentiation opportunities.
    

Reference projects should materially influence opportunity evaluation.

---

# 95. Reference Project Map

The Research Director may create:

|Project|User|Problem Coverage|Trust|AI|Major Gap|Relevance|
|---|---|---|---|---|---|---|

This is a synthesis layer.

Do not replace detailed cards with the table.

---

# 96. Reference Landscape Status

A solution landscape may be classified as:

```text
EMPTY / UNDEREXPLORED

EMERGING

FRAGMENTED

MATURE

SATURATED

UNCLEAR
```

Each classification requires evidence.

---

# 97. Final Reference Project Principle

Reference-project research is not about proving our idea is unique.

It is about discovering reality before we invest in the wrong direction.

The strongest research asks:

> **Who already solves this?**

> **How do they solve it?**

> **How well does it work?**

> **What do users still struggle with?**

> **What have others already learned?**

> **What has already failed?**

> **What could we transfer from more mature domains?**

> **Is there still a meaningful reason for our project to exist?**

If the answer to the last question is no, that is a valuable result.

If the answer is yes, the remaining gap should be supported by evidence rather than novelty claims.