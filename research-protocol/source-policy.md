## Islamic AI Challenge — Research Source Policy

This document defines how all research agents must discover, evaluate, use, cite, compare, and interpret sources throughout the project.

It applies to:

- Islamic religious sources;
    
- scholarly material;
    
- academic research;
    
- user/community evidence;
    
- product information;
    
- technical documentation;
    
- competitor/reference projects;
    
- statistics;
    
- news and media;
    
- social platforms;
    
- any external information used to support a research conclusion.
    

This policy supplements `AGENTS.md`.

If a source-related instruction conflicts with `AGENTS.md`, follow `AGENTS.md` unless the Research Director explicitly documents an approved exception.

---

# 1. Core Principle

A source is not valuable merely because it supports an idea.

A source is valuable when it helps establish what is true, uncertain, disputed, experienced, or currently available.

Agents must optimize for:

**Authority → Relevance → Traceability → Context → Corroboration**

not:

**Agreement with our preferred conclusion**

---

# 2. Source Categories Must Remain Separate

Agents must distinguish between different kinds of evidence.

Do not treat all sources as interchangeable.

The primary categories are:

1. Islamic primary texts
    
2. Islamic scholarly sources
    
3. Islamic institutional sources
    
4. Academic and scientific research
    
5. Official product/project sources
    
6. User and behavioral evidence
    
7. Journalism and media
    
8. Informal commentary
    
9. Agent inference
    

Each category answers different questions.

For example:

- a fatwa may establish what a scholar ruled;
    
- an app review may establish what a user disliked;
    
- a research paper may establish measured behavior;
    
- product documentation may establish what a system claims to support.
    

One category must not automatically substitute for another.

---

# 3. Islamic Primary Texts

Islamic primary textual sources include:

- the Qur'an;
    
- hadith reports.
    

These sources must be handled with particular care.

Agents must not:

- fabricate verses;
    
- fabricate hadith;
    
- alter wording;
    
- remove context in a misleading way;
    
- invent grading information;
    
- attribute a text to the wrong source;
    
- derive a new ruling independently.
    

Where exact wording matters, use a reliable published source and preserve traceability.

---

# 4. Qur'anic Citations

When citing the Qur'an, include at minimum:

```text
Surah:
Ayah:
Translation source, if translation is quoted:
URL or corpus reference:
```

If the agent provides its own English paraphrase rather than a published translation, label it explicitly:

> `[AGENT PARAPHRASE — NOT A QUOTED TRANSLATION]`

Do not present an agent-generated paraphrase as the canonical wording of the Qur'an.

Where interpretation is involved, distinguish the verse itself from tafsir or scholarly explanation.

---

# 5. Hadith Citations

When a hadith materially supports a conclusion, agents should attempt to record:

```text
Collection:
Book / chapter where available:
Hadith identifier where available:
Arabic or translated text source:
Authenticity / grading source where relevant:
URL:
```

Never invent hadith numbers or grades.

If authenticity cannot be verified, write:

> `[HADITH AUTHENTICITY NOT VERIFIED]`

Do not assume that a widely shared quotation is an authentic hadith.

---

# 6. Islamic Scholarly Sources

Islamic scholarly material may include:

- published fatwas;
    
- scholarly explanations;
    
- books;
    
- lectures;
    
- institutional rulings;
    
- official scholar websites;
    
- recognized collections of scholarly material.
    

Agents must identify whose view is being presented.

Prefer:

> “Shaykh X states…”

over:

> “Islam says…”

unless the broader claim is independently justified.

The more contested the subject, the more important attribution becomes.

---

# 7. Bin Baz Official Website

For this project, the official website of Shaykh Abdul Aziz ibn Baz:

[https://binbaz.org.sa/](https://binbaz.org.sa/)

is an approved **trusted primary scholarly reference corpus within the scope of material actually published on the website**.

Agents using Bin Baz must:

1. use the official website where reasonably possible;
    
2. link directly to the relevant page;
    
3. identify the title of the source;
    
4. preserve important context;
    
5. distinguish direct quotation from paraphrase;
    
6. avoid expanding the ruling beyond what the source establishes;
    
7. identify specific circumstances mentioned in the source;
    
8. preserve qualifications and exceptions;
    
9. distinguish the scholar's position from broader claims of consensus.
    

Agents must never transform:

> “According to Shaykh Ibn Baz…”

into:

> “All scholars agree…”

unless reliable independent evidence establishes such agreement.

---

# 8. Bin Baz Is Not an Exhaustive Corpus

The Bin Baz corpus is highly valuable for this research, but agents must not assume that it:

- contains every Islamic ruling;
    
- represents every school of jurisprudence;
    
- documents every legitimate scholarly disagreement;
    
- resolves every contemporary issue;
    
- eliminates the need for additional scholarly review.
    

When a research question concerns disagreement, comparative jurisprudence, consensus, minority positions, or a matter not adequately covered by the corpus, additional evidence may be necessary.

Use:

> `[ADDITIONAL SCHOLARLY REVIEW REQUIRED]`

when appropriate.

---

# 9. Islamic Source Hierarchy

When answering a religious-source research question, agents should generally prefer evidence in this order where applicable:

### Tier I — Primary Islamic Text

- Qur'an;
    
- authenticated hadith.
    

### Tier II — Direct Scholarly Primary Material

- official scholar websites;
    
- original fatwa collections;
    
- published scholarly works;
    
- direct institutional rulings.
    

### Tier III — Reliable Scholarly Repositories

- recognized databases;
    
- verified collections;
    
- institutional archives reproducing original material.
    

### Tier IV — Secondary Explanations

- educational articles;
    
- scholarly summaries;
    
- reputable explanatory websites.
    

### Tier V — Informal Discussion

- forums;
    
- Reddit;
    
- social posts;
    
- unsourced videos;
    
- personal blogs.
    

Tier V may reveal user confusion or public perception.

It should normally **not establish Islamic rulings**.

---

# 10. Do Not Confuse Religious Evidence with User Evidence

A Reddit comment may be excellent evidence that:

> users find a concept confusing.

It is poor evidence that:

> a particular ruling is correct.

Similarly, a fatwa may be excellent evidence for:

> what a scholar ruled.

It may not establish:

> how frequently users experience a particular product problem.

Agents must always ask:

> What question does this source actually answer?

---

# 11. Scholarly Disagreement

Where meaningful scholarly disagreement exists, agents must preserve it.

Do not artificially manufacture consensus.

Do not exaggerate disagreement either.

When disagreement appears relevant, attempt to determine:

```text
ISSUE:

POSITION A:

SOURCE(S):

POSITION B:

SOURCE(S):

KNOWN BASIS OF DISAGREEMENT:

IS CONSENSUS CLAIMED?

CAN CONSENSUS BE VERIFIED?

DOES CONTEXT ALTER THE RULING?

REQUIRES SCHOLAR REVIEW:
Yes / No
```

If the agent cannot responsibly characterize the disagreement, use:

> `[SCHOLARLY STATUS UNRESOLVED]`

---

# 12. Consensus Claims

Claims of ijma' or scholarly consensus require particularly strong evidence.

Agents must not infer consensus because:

- several websites repeat the same ruling;
    
- one scholar describes a matter as obvious;
    
- the agent cannot find an opposing position;
    
- a position is popular online.
    

Where consensus materially affects the research, find an appropriate scholarly source explicitly establishing it.

Otherwise use narrower language.

---

# 13. Schools of Jurisprudence

Where madhhab differences materially affect a problem, agents should preserve those distinctions rather than flattening them.

Relevant research may record:

- Hanafi;
    
- Maliki;
    
- Shafi'i;
    
- Hanbali;
    
- other recognized scholarly positions where relevant.
    

Agents are not required to perform comparative fiqh unless it matters to the research question.

Do not introduce disagreement merely for completeness when it has no bearing on the problem being investigated.

---

# 14. Context-Dependent Rulings

Agents must be alert to religious material whose application depends on:

- intention;
    
- location;
    
- custom;
    
- contractual details;
    
- family circumstances;
    
- financial structure;
    
- timing;
    
- medical condition;
    
- legal context;
    
- jurisdiction;
    
- individual facts.
    

A source answering one factual scenario must not automatically be generalized to another.

Record relevant contextual conditions.

---

# 15. Fatwa vs General Knowledge

Agents must distinguish between:

### General educational Islamic information

and

### Personalized religious judgment or fatwa

Questions that materially depend on an individual's specific circumstances may require qualified scholarly review.

Research agents must not independently issue personal fatwas.

If such cases arise, document them as product/safety requirements.

Use:

> `[PERSONAL SCHOLARLY JUDGMENT MAY BE REQUIRED]`

---

# 16. High-Risk Religious Topics

Use heightened caution around topics including:

- takfir;
    
- divorce;
    
- marriage validity;
    
- inheritance;
    
- major financial transactions;
    
- accusations of disbelief;
    
- criminal punishment;
    
- medical-religious decisions;
    
- rights between individuals;
    
- religious vows;
    
- complex contemporary financial instruments.
    

Agents should focus on researching the information problem, workflow, sourcing, or escalation need.

Do not independently adjudicate sensitive individual cases.

---

# 17. Direct Quotations

Use direct quotations only where wording materially matters.

When quoting:

- preserve exact meaning;
    
- avoid deceptive truncation;
    
- identify the speaker/source;
    
- link to the original where possible;
    
- keep quotations reasonably short.
    

Never create quotation marks around an agent-generated paraphrase.

Use:

> `[PARAPHRASE]`

where appropriate.

---

# 18. Translation

Translations can introduce meaning changes.

Whenever translation affects a religious conclusion:

- preserve the source language where practical;
    
- identify the translation source;
    
- avoid silently modifying technical terminology;
    
- flag ambiguous terms;
    
- compare translations when necessary.
    

Important Arabic terms may be retained alongside translation.

Example:

```text
Tawakkul (توكل)
```

Do not assume one English word perfectly captures every Islamic technical concept.

---

# 19. Arabic Search Is Required Where Relevant

Research about Islamic scholarship should not rely exclusively on English-language search.

Agents capable of doing so should search Arabic sources where they materially improve evidence quality.

This is especially important when researching:

- original fatwas;
    
- scholarly terminology;
    
- Arabic Islamic platforms;
    
- Arabic user workflows;
    
- original quotations;
    
- local products and services.
    

English-language results may still be useful, but translation layers should not unnecessarily replace original sources.

---

# 20. Search Beyond the First Result

Search ranking does not equal authority.

Agents must not automatically trust:

- the first Google result;
    
- AI-generated search summaries;
    
- snippets;
    
- featured answers;
    
- social-media popularity.
    

Open and inspect the underlying source.

Where the claim matters, verify it.

---

# 21. Search Snippets Are Not Evidence

Search-engine snippets may be:

- truncated;
    
- outdated;
    
- generated;
    
- missing context.
    

A snippet may guide research.

It should not normally serve as the final evidence for an important claim.

Open the original page.

---

# 22. AI-Generated Content Is Not a Primary Source

Outputs from:

- ChatGPT;
    
- Gemini;
    
- Claude;
    
- Perplexity;
    
- Copilot;
    
- other AI systems
    

must not be treated as authoritative evidence.

AI systems may assist with:

- discovering sources;
    
- generating search terms;
    
- summarizing already verified material;
    
- comparing evidence;
    
- organizing findings.
    

But their outputs are not evidence by themselves.

Always trace substantive claims back to the underlying source.

---

# 23. Academic Sources

Academic research is preferred when investigating:

- user behavior;
    
- misinformation;
    
- learning outcomes;
    
- human-computer interaction;
    
- NLP performance;
    
- translation quality;
    
- trust;
    
- retrieval systems;
    
- AI safety;
    
- information-seeking behavior;
    
- digital religion;
    
- educational technology.
    

Prefer, where possible:

1. peer-reviewed research;
    
2. systematic reviews;
    
3. reputable conference papers;
    
4. university or institutional publications;
    
5. credible preprints where appropriate.
    

Record methodological limitations.

---

# 24. Academic Evidence Must Match the Claim

Do not cite a paper merely because its title sounds relevant.

Inspect:

- research question;
    
- population;
    
- methodology;
    
- sample size;
    
- findings;
    
- limitations;
    
- date.
    

For example:

A study of 30 university students should not automatically be generalized to all Muslims worldwide.

Use language proportional to the evidence.

---

# 25. Preprints

Preprints can be useful, especially for recent AI research.

However, identify them as preprints when relevant.

Do not represent an unreviewed preprint as equivalent to established peer-reviewed evidence.

Where the finding is important, seek corroboration.

---

# 26. Statistics

Statistics must include enough information to understand what they measure.

Capture where available:

```text
VALUE:

METRIC:

POPULATION:

GEOGRAPHY:

DATE:

SOURCE:

METHODOLOGY:

LIMITATION:
```

Avoid orphan statistics such as:

> “70% of Muslims experience X”

without a traceable source and population definition.

---

# 27. User and Behavioral Evidence

User evidence may include:

- app-store reviews;
    
- public support threads;
    
- Reddit;
    
- forums;
    
- social media;
    
- YouTube comments;
    
- public Q&A discussions;
    
- public product feedback;
    
- interviews;
    
- survey responses;
    
- recurring search behavior where observable.
    

These sources are especially valuable for discovering:

- pain;
    
- confusion;
    
- workarounds;
    
- unmet expectations;
    
- repeated failures;
    
- language barriers;
    
- usability problems.
    

They should be treated as **behavioral evidence**, not automatically as factual authority.

---

# 28. User Evidence Quality

Strength increases when:

- multiple users independently report the same issue;
    
- reports span multiple platforms;
    
- complaints are detailed;
    
- the workflow can be reconstructed;
    
- the issue persists over time;
    
- product reviews corroborate community discussion.
    

Strength decreases when:

- one anonymous user makes an unsupported claim;
    
- comments appear copied;
    
- context is missing;
    
- the statement is obviously speculative;
    
- the complaint concerns an outdated version.
    

---

# 29. Do Not Manufacture User Consensus

Avoid statements like:

> “Users want…”

unless evidence supports the generalization.

Prefer:

> “Several users reviewed…”

or:

> “A recurring theme across the sampled discussions was…”

Record sample limitations.

---

# 30. Community Platforms

Community platforms should be approached as field research.

Agents should look for:

- recurring questions;
    
- repeated misunderstandings;
    
- workflows;
    
- complaints;
    
- emotional friction;
    
- product failures;
    
- workarounds;
    
- terminology barriers.
    

Do not treat popularity or upvotes as proof of religious or factual correctness.

---

# 31. Direct Interviews and Surveys

If the project later conducts interviews or surveys, those findings should be clearly separated from online observational research.

Store:

```text
METHOD:

PARTICIPANT TYPE:

NUMBER OF PARTICIPANTS:

RECRUITMENT METHOD:

QUESTIONS:

RAW RESPONSES:

SYNTHESIS:

LIMITATIONS:
```

Do not alter participant responses to strengthen an argument.

---

# 32. Product Sources

For competitor and reference-project research, prioritize:

### Primary Product Sources

- official website;
    
- official documentation;
    
- public repository;
    
- developer documentation;
    
- release notes;
    
- published demos.
    

Use these to establish what the product claims to support.

---

# 33. Product Claims Are Not Independent Proof

If a product website states:

> “99% accurate”

that establishes that the company makes the claim.

It does **not** independently establish that the system is 99% accurate.

Label appropriately:

> `[VENDOR CLAIM]`

Seek external validation where the claim matters.

---

# 34. Product User Evidence

Use:

- app-store reviews;
    
- GitHub issues;
    
- public support threads;
    
- Reddit discussions;
    
- community forums;
    
- independent reviews
    

to understand real-world experience.

Separate:

> what the vendor says

from:

> what users report.

---

# 35. GitHub and Open-Source Projects

When referencing GitHub projects, inspect where relevant:

- repository;
    
- README;
    
- commit activity;
    
- releases;
    
- issues;
    
- license;
    
- architecture;
    
- documentation;
    
- project status.
    

Do not assume a repository is active merely because it exists.

Record whether it appears:

- active;
    
- maintained;
    
- experimental;
    
- abandoned;
    
- archived;
    
- unclear.
    

---

# 36. Reference Projects from Adjacent Domains

Agents should actively look outside Islamic technology where analogous trust problems exist.

Priority domains may include:

- medicine;
    
- law;
    
- scientific research;
    
- journalism;
    
- education;
    
- compliance;
    
- financial services;
    
- fact checking;
    
- knowledge management;
    
- academic search.
    

These references are used for **design learning**, not Islamic authority.

Clearly label them:

> `[ADJACENT-DOMAIN REFERENCE]`

---

# 37. Journalism

Journalism may be useful for:

- recent events;
    
- company announcements;
    
- controversies;
    
- product developments;
    
- interviews;
    
- public incidents.
    

Prefer:

- original reporting;
    
- reputable outlets;
    
- clearly attributed reporting;
    
- primary documents where available.
    

For important claims, seek primary evidence rather than relying entirely on media summaries.

---

# 38. Blogs and Commentary

Blogs may be useful for:

- practitioner experience;
    
- technical explanation;
    
- product commentary;
    
- discovering leads.
    

They are generally weaker for establishing important factual claims unless the author is directly involved or provides verifiable evidence.

Evaluate authorship and incentives.

---

# 39. Social Media

Social media is useful for:

- discovering pain points;
    
- observing reactions;
    
- identifying terminology;
    
- finding emerging products;
    
- locating primary announcements.
    

It is weak for:

- establishing scholarly authority;
    
- proving broad prevalence;
    
- verifying complex claims without corroboration.
    

Treat posts proportionally.

---

# 40. Primary Sources Are Preferred

Whenever possible, prefer:

**original document**

over:

**article describing the document**

and:

**original product documentation**

over:

**blog describing the product**

and:

**original fatwa**

over:

**forum user paraphrasing the fatwa**

Secondary sources remain useful for discovery and context.

---

# 41. Triangulation

Important research conclusions should ideally use multiple independent sources.

For example:

```text
Academic research
+
user reports
+
competitor limitation
=
stronger problem evidence
```

Triangulation reduces dependence on one potentially biased source.

---

# 42. Independence of Sources

Ten websites copying the same original article do not represent ten independent sources.

Agents must distinguish:

- independent corroboration;
    
- duplicated content;
    
- syndicated content;
    
- copied quotations;
    
- common upstream sources.
    

Prefer diverse evidence chains.

---

# 43. Source Freshness

Freshness matters differently depending on the claim.

Old sources may remain excellent for:

- classical scholarship;
    
- foundational theory;
    
- historical facts.
    

Fresh sources are preferable for:

- current product capabilities;
    
- pricing;
    
- market availability;
    
- active repositories;
    
- recent AI performance;
    
- current user complaints;
    
- platform features.
    

Always consider whether the claim may have changed.

---

# 44. Archive Historical States When Relevant

When comparing products over time, record dates.

Do not criticize a current system solely for a limitation reported several years earlier unless the limitation is confirmed to remain.

---

# 45. Contradictory Sources

When credible sources disagree:

1. do not silently choose one;
    
2. identify the contradiction;
    
3. inspect whether they address the same question;
    
4. check dates and context;
    
5. inspect source authority;
    
6. determine whether disagreement can be resolved;
    
7. preserve uncertainty when it cannot.
    

Use:

```text
[CONTRADICTION]

Source A:
Claim:

Source B:
Claim:

Possible explanation:

Current conclusion:

Confidence:
```

---

# 46. Absence of Evidence

Failure to find evidence is not automatically evidence that something does not exist.

Avoid:

> “No solution exists.”

Prefer:

> “No relevant solution was identified within the research performed.”

unless exhaustive evidence justifies a stronger claim.

---

# 47. Negative Evidence

Negative evidence is important.

Record credible evidence that:

- users are satisfied;
    
- existing products solve the problem;
    
- the problem is uncommon;
    
- the workflow is simpler than expected;
    
- AI is unnecessary;
    
- adoption barriers are severe.
    

Do not suppress evidence because it weakens an opportunity.

---

# 48. Disconfirmation Requirement

For every major hypothesis, agents must deliberately search for contrary evidence.

Example:

```text
HYPOTHESIS:
Users struggle to verify AI-generated Islamic answers.

DISCONFIRMATION SEARCH:
Search for products already providing strong claim-level citations.
Search for user reports indicating citations are sufficient.
Search for studies showing users do not value provenance.

RESULT:
...
```

A hypothesis surviving serious disconfirmation becomes more credible.

---

# 49. Source Capture Format

Important sources should be recorded using the following structure where practical:

```text
SOURCE ID:

CATEGORY:
Islamic / Academic / Product / User / Technical / Media / Other

TITLE:

AUTHOR / ORGANIZATION:

URL:

PUBLICATION DATE:

ACCESS DATE:

LANGUAGE:

PRIMARY OR SECONDARY:

KEY FINDING:

RELEVANT EXCERPT:

WHAT THIS SOURCE SUPPORTS:

WHAT THIS SOURCE DOES NOT SUPPORT:

LIMITATIONS:

CONFIDENCE:
High / Medium / Low
```

---

# 50. Evidence IDs

Where the research becomes large, assign evidence identifiers.

Example:

```text
EVID-001
EVID-002
EVID-003
```

Problem Cards can then reference:

```text
Supporting evidence:
EVID-003
EVID-017
EVID-025
```

This improves traceability and cross-agent synthesis.

---

# 51. Direct Evidence vs Interpretation

Record both separately.

Example:

```text
[EVIDENCE]
12 of 40 sampled reviews mention difficulty identifying the source of generated answers.

[OBSERVATION]
Source transparency appears to be a recurring usability concern.

[HYPOTHESIS]
Better claim-level provenance may increase trust.
```

Never collapse all three into:

> “Users need claim-level citations.”

---

# 52. Evidence Strength

Agents may use the following working labels.

### Strong

The source is directly relevant, authoritative or methodologically sound, and materially supports the claim.

### Moderate

The source is useful but has limitations in authority, sample, applicability, or methodology.

### Weak

The source is anecdotal, indirect, poorly documented, or only partially relevant.

Weak evidence can inspire investigation.

Weak evidence should not independently support major conclusions.

---

# 53. Confidence Is Not Source Quantity

Five weak sources do not necessarily outweigh one highly authoritative direct source.

Evaluate:

- quality;
    
- independence;
    
- relevance;
    
- context.
    

Do not count URLs as votes.

---

# 54. Source Diversity

For important user problems, aim where possible for evidence across several layers:

```text
USER SIGNAL
What people report.

WORKFLOW SIGNAL
What they currently have to do.

EXPERT SIGNAL
What specialists identify as difficult or risky.

PRODUCT SIGNAL
What existing systems fail to provide.

RESEARCH SIGNAL
What academic evidence establishes.
```

Not every problem will have all five.

The combination increases confidence.

---

# 55. Islamic Reliability Review

Any finding that could materially affect Islamic correctness should eventually pass through the Islamic Knowledge & Trust Researcher or another designated reviewer.

Agents outside that role may discover Islamic issues.

They should not assume final authority over them.

Use:

> `[REQUIRES ISLAMIC RELIABILITY REVIEW]`

---

# 56. Source-Boundary Review

When research concerns:

- disagreement;
    
- missing evidence;
    
- ambiguity;
    
- personal fatwa boundaries;
    
- escalation requirements;
    
- inability to answer reliably;
    

route the issue to the Source Boundary & Disagreement Researcher when available.

---

# 57. Technical Claims

Technical claims should use appropriate sources such as:

- official documentation;
    
- model documentation;
    
- benchmarks;
    
- repositories;
    
- papers;
    
- reproducible experiments.
    

Marketing pages may describe capabilities but should not be treated as independent performance verification.

---

# 58. AI Benchmark Claims

When comparing models or AI systems, record:

- model version;
    
- test date;
    
- benchmark;
    
- dataset;
    
- evaluation method;
    
- relevant configuration.
    

Do not compare results produced under incompatible conditions without acknowledging the limitation.

---

# 59. Do Not Cite Aggregators When Originals Are Available

If an aggregator republishes:

- a fatwa;
    
- a paper;
    
- a product announcement;
    
- a statistic;
    

prefer the original source where practical.

Aggregators may remain useful for discovering material.

---

# 60. Broken or Inaccessible Sources

If a useful source is inaccessible:

- record the citation if reliably known;
    
- mark access limitations;
    
- seek an archived or alternative primary version;
    
- do not claim to have inspected content you could not access.
    

Use:

> `[SOURCE NOT DIRECTLY VERIFIED]`

when necessary.

---

# 61. Paywalled Research

A paywalled paper may still be cited if enough reliable metadata or accessible abstract information supports a limited claim.

Do not pretend to have read inaccessible full text.

Clearly distinguish:

> abstract-level evidence

from:

> full-text review.

---

# 62. Citation Chains

Avoid long citation chains such as:

Blog C → citing Article B → summarizing Study A.

Whenever possible, retrieve Study A.

Research should move toward the origin of important claims.

---

# 63. Evidence Saturation

Stop collecting additional sources when:

- multiple strong independent sources establish the point;
    
- new searches mostly repeat existing evidence;
    
- the marginal value of additional sources becomes low.
    

Do not collect sources for appearance.

Time should move to unresolved questions.

---

# 64. Minimum Standard for a Major Problem Claim

A major claim that a problem is worth further investigation should ideally include:

- at least one direct user or workflow signal;
    
- at least one independent corroborating source;
    
- research into existing solutions;
    
- disconfirming evidence search;
    
- limitations;
    
- confidence level.
    

This is a guideline rather than an artificial quota.

Quality overrides quantity.

---

# 65. Source Bias

Agents should consider possible incentives.

Examples:

- vendors want to promote their product;
    
- users posting complaints may disproportionately represent negative experiences;
    
- scholars may address questions from particular methodological traditions;
    
- academic studies may use narrow populations;
    
- media articles may emphasize unusual cases.
    

Bias does not invalidate a source.

It affects interpretation.

---

# 66. Geographic Context

The Muslim population is globally diverse.

Do not assume findings from:

- Saudi Arabia;
    
- the Gulf;
    
- the United States;
    
- Europe;
    
- South Asia;
    
- Southeast Asia;
    

automatically generalize worldwide.

Record geographic context where relevant.

---

# 67. Language Context

Problems may differ materially across:

- Arabic;
    
- English;
    
- French;
    
- Urdu;
    
- Indonesian;
    
- Malay;
    
- Turkish;
    
- other languages.
    

Record which language population the evidence actually concerns.

Do not convert an English-language problem into a global Islamic problem without validation.

---

# 68. Convert and New-Muslim Research

When researching converts or people learning about Islam:

- prioritize direct reports;
    
- avoid assuming all converts follow the same learning path;
    
- identify geography and language where possible;
    
- distinguish religious confusion from cultural confusion;
    
- distinguish lack of information from difficulty evaluating information.
    

Do not reduce users to stereotypes.

---

# 69. Da'wah and Educator Research

When studying scholars, educators, da'wah workers, creators, or researchers, distinguish roles.

Their workflows may differ substantially.

For example:

```text
Islamic scholar
Da'wah volunteer
YouTube creator
Mosque educator
Academic researcher
Translator
Content editor
```

Do not combine them into a single generic persona without evidence.

---

# 70. Do Not Search Only for Complaints

Research must include positive evidence where relevant.

Determine:

- what currently works well;
    
- what users trust;
    
- which workflows users prefer;
    
- what successful products get right.
    

Understanding successful behavior is as valuable as identifying failure.

---

# 71. Preserve Useful Quotes Carefully

For behavioral evidence, short user quotations may be retained when they strongly express a pain point.

Remove unnecessary personal identifiers.

Record:

- platform;
    
- date where available;
    
- URL;
    
- surrounding context.
    

Do not present one vivid quotation as representative of everyone.

---

# 72. Ethical User Research

Publicly available information may be studied, but agents should avoid unnecessary collection of:

- names;
    
- usernames;
    
- contact details;
    
- identifiable personal histories;
    
- private religious circumstances.
    

Extract the problem signal rather than building dossiers on individuals.

---

# 73. Source Storage

Validated sources should be stored or referenced under:

```text
/research/evidence/
```

Competitor and project evidence should additionally be organized under:

```text
/research/reference-projects/
```

Where useful, organize by:

```text
/islamic/
/academic/
/users/
/products/
/technical/
```

Do not duplicate large amounts of content unnecessarily.

---

# 74. Source Naming

Use descriptive filenames.

Example:

```text
EVID-014-app-reviews-source-transparency.md
```

rather than:

```text
source14.md
```

---

# 75. Research Director Responsibility

The Research Director must not treat all submitted evidence as equally valid.

During synthesis, the director must evaluate:

- source quality;
    
- independence;
    
- contradiction;
    
- relevance;
    
- freshness;
    
- methodological limitations;
    
- Islamic source boundaries.
    

Weak evidence should not become strong merely because many agents repeat it.

---

# 76. Correcting Source Errors

If an agent discovers that previously recorded evidence is:

- wrong;
    
- fabricated;
    
- outdated;
    
- misquoted;
    
- incorrectly attributed;
    
- misunderstood;
    

the correction must be explicit.

Do not silently preserve the old claim.

Use:

```text
[CORRECTION]

Previous claim:

Problem:

Corrected interpretation:

Affected files:
```

---

# 77. Uncertainty Is Acceptable

Agents are not required to resolve every question.

Use clear markers:

```text
[UNVERIFIED]

[UNCERTAIN]

[CONFLICTING EVIDENCE]

[SOURCE LIMITATION]

[REQUIRES USER VALIDATION]

[REQUIRES SCHOLAR REVIEW]

[REQUIRES TECHNICAL REVIEW]
```

Explicit uncertainty is better than false confidence.

---

# 78. Prohibited Source Behavior

Agents must never:

- fabricate citations;
    
- invent religious rulings;
    
- invent scholars' positions;
    
- invent statistics;
    
- invent user complaints;
    
- invent competitor features;
    
- cite a page not inspected as though it were inspected;
    
- treat an AI answer as primary evidence;
    
- use search snippets as authoritative proof;
    
- hide contradictory evidence;
    
- exaggerate source strength;
    
- claim consensus without appropriate evidence;
    
- remove context that changes meaning;
    
- convert correlation into causation;
    
- treat repeated copied sources as independent corroboration.
    

---

# 79. Source Decision Checklist

Before relying on a source, ask:

```text
What exact claim am I using this source to support?

Is this source qualified to support that claim?

Is it primary or secondary?

Can I access and verify the original?

Is the source current enough?

Is important context missing?

Could the author have an incentive affecting interpretation?

Does another independent source corroborate it?

Is there credible contradictory evidence?

Am I describing the strength of the evidence accurately?
```

---

# 80. Islamic Source Decision Checklist

For religious claims, additionally ask:

```text
Is this Qur'an, hadith, scholarly interpretation, fatwa, or commentary?

Who is speaking?

Is the attribution verified?

Is the context preserved?

Does the ruling depend on specific circumstances?

Is there known scholarly disagreement?

Am I accidentally generalizing one scholar's view?

Is this question appropriate for automated treatment?

Does this require qualified scholarly review?
```

---

# 81. User Evidence Decision Checklist

For community evidence, ask:

```text
Is this an actual user report?

What user group does it represent?

Is the complaint detailed enough to understand?

Does the same issue appear elsewhere?

Could this be an isolated case?

Is the product/version current?

Am I treating experience as experience rather than universal fact?
```

---

# 82. Product Evidence Decision Checklist

For competitor research, ask:

```text
What does the product officially claim?

What does it actually demonstrate?

What do users report?

What version am I examining?

Is the project active?

What is genuinely missing?

Have I tested whether the supposed gap has already been solved?
```

---

# 83. Final Source Principle

The purpose of sourcing is not to decorate conclusions with citations.

The purpose is to make every important conclusion:

**traceable, challengeable, reproducible, and correctable.**

For Islamic knowledge:

**attribute carefully.**

For user problems:

**observe carefully.**

For academic claims:

**interpret carefully.**

For products:

**verify carefully.**

For uncertainty:

**state it openly.**

Never use evidence merely to defend an idea.

Use evidence to determine whether the idea deserves to exist.