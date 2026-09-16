# Islamic AI Challenge — Research Council Orchestration Protocol

This document defines how the Islamic AI Challenge Problem Discovery Research Lab is executed.

It specifies:

- agent spawn order;
    
- phase sequencing;
    
- agent isolation;
    
- context permissions;
    
- read/write responsibilities;
    
- research handoffs;
    
- file ownership;
    
- identifier allocation;
    
- retry behavior;
    
- stopping rules;
    
- cross-examination flow;
    
- synthesis gates;
    
- context and token discipline;
    
- failure recovery;
    
- final completion conditions.
    

This file controls **how the research system operates**.

It does not replace:

- `AGENTS.md`;
    
- specialist agent profiles;
    
- research protocols;
    
- source policy;
    
- evidence standards.
    

All agents remain bound by those documents.

---

# 1. Instruction Authority Hierarchy

When instructions conflict, agents and the Root Orchestrator must resolve them using this strict priority order:

```text
1. AGENTS.md
   Supreme global constitution for all agents and sub-agents.

2. research-protocol/source-policy.md
   Authoritative rules for Islamic knowledge, canonical texts, attribution, and fatwa boundaries.

3. research-protocol/evidence-standard.md
   Authoritative rules for evidence classification, verification, confidence, and disconfirmation.

4. ORCHESTRATION.md
   Council lifecycle, phase execution, access permissions, isolation, file ownership, and gates.

5. Current Task Packet
   Phase-specific operational assignment, assigned research questions, allowed context, outputs, and stop conditions.

6. Agent Role Profile
   Persistent specialist scope, domain expertise, and role-specific research methodology.

7. Relevant Output Schema (e.g., problem-card-schema.md, reference-project-schema.md)
   Artifact structure, sections, and formatting standards.
```

### Critical Precedence Rules:
- **Task Packets Scope the Phase:** A Task Packet may narrow an agent's focus, context, or specific questions for the active phase, but it can **never** override `AGENTS.md`, theological source integrity (`source-policy.md`), evidence verification standards (`evidence-standard.md`), or orchestration isolation rules.
- **Schemas Govern Formatting, Not Mission:** An output schema defines how artifacts are structured. It must **never** be interpreted as permission to broaden an agent's assigned mission, skip phases, bypass context isolation, or prematurely attempt later-stage analysis (such as solution design during Level 1 problem discovery).
- **Director Adjudication Scope:** The Research Director (Agent 08) may resolve ambiguous research questions or procedural edge cases within a phase, but may not override higher-level constitutional, source-integrity, or evidence-standard requirements.

---

# 2. Purpose

The purpose of orchestration is to prevent the research process from becoming:

> multiple agents generating overlapping ideas and agreeing with each other.

The intended system is:

```text
Independent investigation

→

structured evidence

→

validated problems

→

existing-solution research

→

AI-leverage analysis

→

adversarial attack

→

cross-examination

→

evidence-grounded synthesis
```

---

# 3. Core Orchestration Principle

Agents must receive **only the context necessary for their current role and phase**.

Too little context produces duplicated work.

Too much context produces:

- anchoring;
    
- imitation;
    
- confirmation bias;
    
- context dilution;
    
- unnecessary token consumption.
    

The Orchestrator must actively control information flow.

---

# 4. Two Coordination Roles

The system contains two different coordination responsibilities.

## A. Root Orchestrator

The Root Orchestrator is the parent execution process that:

- reads this file;
    
- spawns agents;
    
- prepares task packets;
    
- controls phase transitions;
    
- controls file access;
    
- tracks completion;
    
- manages retries;
    
- enforces isolation.
    

The Root Orchestrator should **not conduct substantive research**.

## B. Agent 08 — Research Director

The Research Director:

- audits research quality;
    
- resolves research-process questions;
    
- requests targeted follow-up;
    
- moderates cross-examination;
    
- synthesizes evidence;
    
- produces the Opportunity Map.
    

The Root Orchestrator manages execution.

Agent 08 manages research judgment.

Do not collapse these roles.

---

# 5. Research Council

The active council consists of:

```text
Agent 01
Muslim User Researcher

Agent 02
New Muslim Researcher

Agent 03
Educator / Da'wah Researcher

Agent 04
Islamic Knowledge & Trust Researcher

Agent 05
Market & Reference Landscape Researcher

Agent 06
AI Product Opportunity Researcher

Agent 07
Red Team & Skeptical Researcher

Agent 08
Research Director
```

---

# 6. Recursive Agent Spawning

Specialist agents must not freely create additional research swarms.

Default rule:

> Only the Root Orchestrator creates council-level agents.

A specialist agent may use a bounded helper sub-agent only when:

- explicitly permitted in its task packet;
    
- the helper performs a narrow research task;
    
- the helper does not create further agents;
    
- the parent agent verifies the helper's evidence;
    
- the helper does not directly modify shared synthesis artifacts.
    

Avoid uncontrolled recursive agent spawning.

---

# 7. Workspace Structure

The expected workspace is:

```text
/
├── AGENTS.md
├── ORCHESTRATION.md
│
├── agents/
│   ├── 01-muslim-user-researcher.md
│   ├── 02-new-muslim-researcher.md
│   ├── 03-educator-dawah-researcher.md
│   ├── 04-islamic-trust-researcher.md
│   ├── 05-market-landscape-researcher.md
│   ├── 06-ai-opportunity-researcher.md
│   ├── 07-red-team.md
│   └── 08-research-director.md
│
├── research-protocol/
│   ├── source-policy.md
│   ├── evidence-standard.md
│   ├── problem-card-schema.md
│   ├── reference-project-schema.md
│   ├── cross-examination-protocol.md
│   └── opportunity-map-schema.md
│
├── research/
│   ├── raw/
│   ├── evidence/
│   ├── problem-cards/
│   └── reference-projects/
│
└── synthesis/
    ├── opportunity-map.md
    ├── disagreements.md
    └── open-questions.md
```

Do not create additional permanent directories unless orchestration explicitly requires them.

---

# 8. Canonical Filenames

The following are canonical:

```text
research-protocol/cross-examination-protocol.md

research-protocol/opportunity-map-schema.md
```

Do not use:

```text
cross-examination-protocol.md.md

opportunity-map-schema.md.md
```

---

# 9. Repository Hygiene

Agents may modify research artifacts assigned to them.

Agents must not:

- rename unrelated files;
    
- delete another agent's work;
    
- alter global protocols;
    
- alter another agent's profile;
    
- commit or push repository history unless explicitly instructed;
    
- reorganize the workspace independently.
    

Research first.

Repository restructuring is not part of normal agent duties.

---

# 10. Research Cycle

Every complete execution is a Research Cycle.

Assign:

```text
CYCLE-001
CYCLE-002
CYCLE-003
```

or another monotonically increasing identifier.

The cycle identifier must appear in major run-level artifacts.

---

# 11. Run Manifest

At the beginning of each cycle, create:

```text
research/raw/CYCLE-XXX-run-manifest.md
```

Recommended contents:

```text
# Research Cycle Manifest

CYCLE ID:

STARTED:

RESEARCH OBJECTIVE:

AGENT MODEL / CONFIGURATION:

ROOT ORCHESTRATOR:

ACTIVE AGENTS:

PROTOCOL VERSION / COMMIT:
If available

CURRENT PHASE:

PHASE STATUS:

KNOWN LIMITATIONS:

NOTES:
```

Update the manifest when phases complete.

---

# 12. Do Not Mix Research Cycles Silently

Previous research may be reused only when:

- it is still relevant;
    
- its provenance is clear;
    
- its date is known;
    
- current agents understand that it originated in an earlier cycle.
    

Mark:

```text
[PRIOR-CYCLE EVIDENCE]
```

when appropriate.

Do not silently treat stale research as newly verified.

---

# 13. Research State Machine

The research cycle uses these states:

```text
PHASE 0 — BOOTSTRAP

PHASE 1 — INDEPENDENT DISCOVERY

PHASE 2 — PROBLEM VALIDATION

PHASE 3 — MARKET LANDSCAPE

PHASE 4 — AI OPPORTUNITY ANALYSIS

PHASE 5 — RED TEAM

PHASE 6 — CROSS-EXAMINATION

PHASE 7 — SYNTHESIS

PHASE 8 — SYNTHESIS AUDIT

PHASE 9 — COMPLETE
```

Do not skip phases without a documented reason.

---

# 14. Phase 0 — Bootstrap

Before spawning research agents, the Root Orchestrator must verify the workspace.

Required files:

```text
AGENTS.md

ORCHESTRATION.md

research-protocol/source-policy.md

research-protocol/evidence-standard.md

research-protocol/problem-card-schema.md

research-protocol/reference-project-schema.md

research-protocol/cross-examination-protocol.md

research-protocol/opportunity-map-schema.md

agents/01-muslim-user-researcher.md

agents/02-new-muslim-researcher.md

agents/03-educator-dawah-researcher.md

agents/04-islamic-trust-researcher.md

agents/05-market-landscape-researcher.md

agents/06-ai-opportunity-researcher.md

agents/07-red-team.md

agents/08-research-director.md
```

---

# 15. Bootstrap Failure

If a required file is:

- missing;
    
- empty;
    
- obviously corrupted;
    

do not silently continue.

Record:

```text
[BOOTSTRAP BLOCKER]
```

and identify the missing dependency.

If the missing artifact is not required until a later phase, earlier phases may proceed only when doing so does not alter research validity.

---

# 16. Task Packet

Every spawned agent receives a Task Packet.

The packet must contain:

```text
CYCLE ID

CURRENT PHASE

AGENT ROLE

MISSION

FILES TO READ

FILES ALLOWED TO READ

FILES NOT TO READ YET

FILES TO WRITE

QUESTIONS TO ANSWER

REQUIRED OUTPUTS

STOP CONDITIONS

HANDOFF RULES

SPECIAL LIMITATIONS
```

Never launch an agent with only:

> “Research this topic.”

---

# 17. Canonical Documentation vs Runtime Context

To prevent context dilution, instruction repetition, and token exhaustion, the orchestration strictly distinguishes:

```text
CANONICAL REFERENCE DOCUMENTATION
Authoritative, detailed reference standards stored in /research-protocol/.
Kept intact in the repository. Consulted on-demand when an agent's specific task requires it.

RUNTIME REQUIRED CONTEXT
The minimal set of instructions, schemas, and target artifacts loaded for a specific agent and phase.
Follows the principle: Give each agent the minimum context required to perform its current task correctly.
```

Specialist protocols (`source-policy.md`, `evidence-standard.md`, `problem-card-schema.md`, `reference-project-schema.md`, `cross-examination-protocol.md`, `opportunity-map-schema.md`) are **not** preloaded into every agent at startup. They are loaded selectively or consulted on demand.

---

# 17.1 Reference Candidate vs Canonical Reference Project

To protect discovery researchers from context overload and premature competitor analysis:

```text
REFERENCE CANDIDATE (Phase 1: Discovered by Agents 01–04)
A lightweight record of an existing tool, app, website, or service noticed while researching user workflows.
Recorded inline within Section 11 of the Level 1 Problem Card or raw discovery notes:
- Name
- URL
- Related Problem ID
- Target User (if known)
- What It Appears to Solve
- Why Relevant
- Observed Limitation / User Complaint (if found)
Discovery agents do NOT assign RP-* IDs and do NOT read the full reference-project schema.

CANONICAL REFERENCE PROJECT (Phase 3: Owned by Agent 05)
A formal, deeply investigated reference or competitor project assigned a canonical RP-*, ADJ-*, or TECH-* ID.
Agent 05 owns canonical reference-project research, reads the full reference-project-schema.md, and creates
individual evaluation files in /research/reference-projects/.
```

---

# 18. Runtime Context Loading Matrix

The Root Orchestrator must enforce the following context-loading rules for every phase and agent:

| **Phase 1: Agents 01–03**<br>(User, New Muslim, Educator Discovery) | • `AGENTS.md`<br>• Own Agent Profile<br>• Current Task Packet<br>• `problem-card-schema.md` (Level 1 only) | • `source-policy.md`<br>• `evidence-standard.md` | • `reference-project-schema.md` (full schema)<br>• Other discovery agents' raw outputs/cards<br>• Phase 4–8 schemas & synthesis files |
| **Phase 1: Agent 04**<br>(Islamic Knowledge & Trust Discovery) | • `AGENTS.md`<br>• Agent 04 Profile<br>• Current Task Packet<br>• `problem-card-schema.md` (Level 1 only)<br>• `source-policy.md` (MUST READ) | • `evidence-standard.md` | • `reference-project-schema.md` (full schema)<br>• Other discovery agents' raw outputs/cards<br>• Phase 4–8 schemas & synthesis files |
| **Phase 2: Agent 08**<br>(Validation) | • `AGENTS.md`<br>• Agent 08 Profile<br>• Task Packet<br>• `problem-card-schema.md` (Level 2 audit section)<br>• Newly created Level 1 Problem Cards<br>• Agents 01–04 raw discovery reports | • `source-policy.md`<br>• `evidence-standard.md` | • Phase 4–8 schemas (`cross-examination-protocol.md`, `opportunity-map-schema.md`)<br>• Premature solution ideation |
| **Phase 3: Agent 05**<br>(Market Landscape) | • `AGENTS.md`<br>• Agent 05 Profile<br>• Task Packet<br>• `reference-project-schema.md` (Full schema)<br>• `problem-card-schema.md` (Level 3 section)<br>• Validated Problem Cards (Level 2)<br>• Problem Registry (`CYCLE-XXX-problem-registry.md`) | • `evidence-standard.md`<br>• `source-policy.md`<br>• Specific discovery evidence if cited | • Complete raw discovery conversations across all agents (reduces anchoring)<br>• Phase 4–8 opportunity/synthesis files |
| **Phase 4: Agent 06**<br>(AI Opportunity) | • `AGENTS.md`<br>• Agent 06 Profile<br>• Task Packet<br>• `problem-card-schema.md` (Level 4 Part A)<br>• Validated Problem Cards (Level 2 & 3)<br>• Problem Registry & Gap Register<br>• Agent 05 Landscape Summary & relevant `RP-*` files | • Relevant Agent 04 trust findings<br>• Specific technical benchmarks | • Unrelated Phase 1 raw discovery material<br>• Phase 6–8 cross-examination & synthesis |
| **Phase 5: Agent 07**<br>(Red Team) | • `AGENTS.md`<br>• Agent 07 Profile<br>• Task Packet<br>• `problem-card-schema.md` (Level 4 Part B)<br>• Target Opportunity Package (Problem Cards Levels 1–4, Agent 05 Landscape, Agent 06 AI Opportunity Register) | • Canonical protocols on demand (`source-policy.md`, etc.) | • Unrelated raw discovery files<br>• Director synthesis preferences / ranking |
| **Phase 6: Participants**<br>(Cross-Examination) | • `cross-examination-protocol.md` (relevant rules)<br>• Target Examination Packet (Target Problem Card, specific P0/P1 challenge, counterevidence) | • Relevant Reference Projects or Evidence notes cited in the challenge | • Entire repository history<br>• Unrelated problem cards |
| **Phase 7: Agent 08**<br>(Synthesis) | • `AGENTS.md`<br>• Agent 08 Profile<br>• `opportunity-map-schema.md`<br>• Structured Artifacts (Level 4 Problem Cards, `RP-*`, `AI-OP-*`, `RT-*`, CX Summary, `disagreements.md`, `open-questions.md`) | • Raw discovery files (only if structured artifact is ambiguous) | • Non-evidenced hackathon pitch ideas |

---

# 19. Context Isolation

During Phase 1, Agents 01–04 must not read:

```text
other specialist-agent raw outputs

other specialist-agent Problem Cards

future synthesis files

Agent 06 analysis

Agent 07 analysis
```

This preserves independent discovery.

---

# 20. Phase 1 — Independent Discovery

Spawn in parallel:

```text
Agent 01

Agent 02

Agent 03

Agent 04
```

Parallel execution is preferred because it reduces cross-agent influence.

---

# 21. Phase 1 Input

In accordance with the Runtime Context Loading Matrix, Phase 1 inputs are strictly calibrated by role:

### For Agents 01–03 (User, New Muslim, Educator Discovery):
- **MUST READ:**
  - `AGENTS.md` (Global Constitution);
  - Own specialist role profile;
  - Current Phase 1 Task Packet;
  - Level 1 of `research-protocol/problem-card-schema.md`;
  - Challenge research objective and approved domain references where relevant.
- **MAY CONSULT IF NEEDED:** `research-protocol/source-policy.md` and `research-protocol/evidence-standard.md` on demand when handling sacred texts, complex rulings, or ambiguous evidence.

### For Agent 04 (Islamic Knowledge & Trust Researcher):
- **MUST READ:**
  - `AGENTS.md` (Global Constitution);
  - Agent 04 specialist role profile;
  - Current Phase 1 Task Packet;
  - Level 1 of `research-protocol/problem-card-schema.md`;
  - **`research-protocol/source-policy.md`** (*mandatory startup context* — Agent 04's core role governs Islamic source integrity, attribution, and scholarly boundaries);
  - Challenge research objective and verified domain references where relevant.
- **MAY CONSULT IF NEEDED:** `research-protocol/evidence-standard.md` on demand.

**Strict Phase 1 Isolation (All Agents 01–04):**
- Do **NOT** provide the full `reference-project-schema.md` (discovery agents record lightweight Reference Candidates in Level 1 Problem Cards);
- Do **NOT** provide outputs or Problem Cards from other Phase 1 specialist agents (preserves independent discovery);
- Do **NOT** provide downstream synthesis, cross-examination, or opportunity schemas.

---

# 22. Phase 1 Goal

Each agent must discover:

```text
Users

Jobs to be done

Current workflows

Pain points

Consequences

Workarounds

Evidence

Existing solutions encountered

Contradicting evidence

Candidate Problem Cards
```

They are not asked to select projects.

---

# 23. Phase 1 Raw Output

Each agent writes one primary raw report:

```text
research/raw/CYCLE-XXX-agent-01-discovery.md

research/raw/CYCLE-XXX-agent-02-discovery.md

research/raw/CYCLE-XXX-agent-03-discovery.md

research/raw/CYCLE-XXX-agent-04-discovery.md
```

---

# 24. Problem Card Ownership

Agents 01–04 create Problem Cards in:

```text
research/problem-cards/
```

Problem Cards are owned by the originating agent until synthesis.

Other agents may challenge them.

They should not silently overwrite them.

---

# 25. Problem ID Allocation

To prevent parallel ID collisions, reserve ranges.

```text
Agent 01:
P-001 through P-099

Agent 02:
P-100 through P-199

Agent 03:
P-200 through P-299

Agent 04:
P-300 through P-399
```

Reserved future ranges:

```text
P-400 through P-799:
Future expansion

P-800 through P-899:
Director-created cross-cutting or merged problems if absolutely necessary

P-900 through P-999:
Reserved
```

Do not reuse retired IDs.

---

# 26. Problem Card Filenames

Use:

```text
P-001-short-description.md

P-103-short-description.md

P-218-short-description.md
```

Follow `problem-card-schema.md`.

---

# 27. Evidence IDs

Where internal evidence records are created, namespace them by agent:

```text
E01-001
E01-002
E02-001
E03-001
E04-001
```

If later agents create evidence records, continue the same pattern:

```text
E05-001
E06-001
E07-001
E08-001
```

This prevents parallel collisions. Do not add cycle numbers to Evidence IDs; cycle provenance is captured by the artifact and run manifest.

Evidence files belong under:

```text
research/evidence/
```

---

# 28. Phase 1 Stop Condition

An Agent 01–04 discovery pass stops when:

- required research questions have been addressed;
    
- meaningful problem candidates have been documented;
    
- major evidence has been collected;
    
- new sources mostly repeat known findings;
    
- two consecutive searches produce no materially new findings.
    

Do not research indefinitely.

---

# 29. Phase 1 Quality Rule

Do not require each agent to produce a fixed number of problems.

Accept:

```text
2 strong problems
```

over:

```text
10 speculative problems
```

Artificial quantity is prohibited.

---

# 30. Phase 1 Completion Gate

Phase 1 completes when all active Agents 01–04 have either:

```text
COMPLETED
```

or:

```text
COMPLETED WITH LIMITATIONS
```

If an agent fails completely, record the coverage gap before proceeding.

---

# 31. Phase 2 — Problem Validation

Spawn Agent 08.

At this stage, Agent 08 is acting as:

> intake auditor,

not full synthesizer.

---

# 32. Agent 08 Phase 2 Input

In accordance with the Runtime Context Loading Matrix, Agent 08 receives:

```text
AGENTS.md (Global Constitution)

Agent 08 profile & Phase 2 Task Packet

research-protocol/problem-card-schema.md (Level 2 audit section)

Level 1 Problem Cards created by Agents 01–04

Agents 01–04 raw discovery reports
```

Agent 08 may consult `source-policy.md` and `evidence-standard.md` on demand to evaluate theological compliance and citation rigor.

Agent 08 must **not** load later schemas (`cross-examination-protocol.md`, `opportunity-map-schema.md`) or attempt to choose solution directions during intake validation.

---

# 33. Phase 2 Responsibilities

Agent 08 checks:

- Problem Card completeness;
    
- evidence traceability;
    
- duplicated problems;
    
- user specificity;
    
- workflow clarity;
    
- unsupported prevalence claims;
    
- contradictory evidence;
    
- source-policy compliance.
    

---

# 34. Problem Validation States

Agent 08 assigns:

```text
DISCOVERED

UNDER VALIDATION

SUPPORTED

WEAKLY SUPPORTED

REQUIRES REFRAME

DUPLICATE / MERGED

DISCONFIRMED

OUT OF SCOPE
```

---

# 35. Research Return During Phase 2

If a Problem Card lacks essential evidence, Agent 08 sends a targeted return request to its owner.

Each agent receives at most:

```text
1 normal targeted return pass
```

per Problem Card.

A second return requires a P0/P1 reason.

Avoid endless refinement loops.

---

# 36. Phase 2 Output

Agent 08 produces:

```text
research/raw/CYCLE-XXX-problem-registry.md
```

Recommended fields:

```text
Problem ID

Owner

User

Short problem

Validation status

Evidence confidence

Major gaps

Duplicate links

Ready for landscape research?
Yes / No
```

---

# 37. Phase 2 Gate

Only problems marked:

```text
SUPPORTED

WEAKLY SUPPORTED

REQUIRES REFRAME
```

where the remaining uncertainty is explicit may proceed into landscape investigation.

Clearly disconfirmed problems should not consume Agent 05 research time unless needed as a negative reference.

---

# 38. Phase 3 — Market Landscape

Spawn Agent 05.

Agent 05 begins only after receiving the validated Problem Registry.

---

# 39. Agent 05 Context

In accordance with the Runtime Context Loading Matrix, Agent 05 receives:

```text
AGENTS.md (Global Constitution)

Agent 05 profile & Phase 3 Task Packet

research-protocol/reference-project-schema.md (Full canonical schema)

research-protocol/problem-card-schema.md (Level 3 section)

Validated Problem Cards (Level 2) including candidate reference mentions

Problem Registry (research/raw/CYCLE-XXX-problem-registry.md)
```

Agent 05 may consult `evidence-standard.md` and `source-policy.md` on demand when evaluating claims.

**Agent 05 must NOT receive:**
- Complete raw discovery conversations across all agents (preserves objectivity and prevents context anchoring);
- Phase 4–8 opportunity, cross-examination, and synthesis files.

---

# 40. Agent 05 Goal

Agent 05 determines:

```text
What already exists?

Which products solve the same jobs?

Which solve part of the workflow?

Which non-AI alternatives exist?

Which manual alternatives exist?

What adjacent-domain systems are relevant?

What appears genuinely unresolved?
```

---

# 41. Reference Project Ownership

Agent 05 owns canonical Reference Project files.

Store under:

```text
research/reference-projects/
```

Other agents may suggest projects but must not overwrite Agent 05's records.

---

# 42. Reference Project IDs

Use:

```text
RP-001
RP-002
RP-003
```

for direct/partial/reference projects.

Use where appropriate:

```text
ADJ-001

TECH-001
```

according to `reference-project-schema.md`.

---

# 43. Gap IDs

Agent 05 owns preliminary Gap IDs.

Use:

```text
GAP-001

GAP-002

GAP-003
```

Never reuse a Gap ID.

---

# 44. Phase 3 Outputs

Required Agent 05 outputs:

```text
Reference Project records

market / reference landscape summary

capability comparison where useful

workflow coverage analysis where useful

gap register

disconfirmation findings
```

Primary summary:

```text
research/raw/CYCLE-XXX-agent-05-landscape.md
```

---

# 45. Phase 3 Gate

Before proceeding, Agent 08 performs a light audit.

It checks:

- important problems received landscape coverage;
    
- major direct competitors were searched;
    
- absence claims are scoped;
    
- Arabic/non-English searches were used where relevant;
    
- non-AI alternatives were considered.
    

This is not full synthesis.

---

# 46. Phase 3 Return Limit

Agent 08 may return Agent 05 for:

```text
one targeted market follow-up pass
```

for unresolved P0/P1 market questions.

Do not rerun the entire market scan.

---

# 47. Phase 4 — AI Opportunity Analysis

Spawn Agent 06.

Agent 06 begins after Phase 3.

---

# 48. Agent 06 Context

In accordance with the Runtime Context Loading Matrix, Agent 06 receives:

```text
AGENTS.md (Global Constitution)

Agent 06 profile & Phase 4 Task Packet

research-protocol/problem-card-schema.md (Level 4 Part A: AI Opportunity Evaluation)

Validated Problem Cards (Levels 1–3)

Problem Registry & Gap Register (GAP-XXX)

Agent 05 Landscape Summary & relevant canonical RP-* records
```

Agent 06 may consult relevant Agent 04 trust findings and technical benchmarks on demand.

**Agent 06 must NOT receive:**
- Unrelated Phase 1 raw discovery files;
- Phase 6–8 cross-examination and synthesis artifacts.

---

# 49. Agent 06 Goal

For each meaningful validated gap:

```text
identify exact task

identify strongest non-AI baseline

determine whether AI is justified

identify specific AI capability

define expected measurable value

identify data / feasibility constraints

identify new risks
```

---

# 50. AI Opportunity IDs

Agent 06 owns:

```text
AI-OP-001

AI-OP-002

AI-OP-003
```

Never reuse IDs.

---

# 51. Agent 06 Output

Primary output:

```text
research/raw/CYCLE-XXX-agent-06-ai-opportunities.md
```

It should include:

- AI Opportunity Register;
    
- non-AI counterfactuals;
    
- capability mapping;
    
- measurement approaches;
    
- risk analysis;
    
- disconfirmed AI opportunities.
    

---

# 52. AI Rejection Is Valid

Agent 06 must explicitly preserve cases where:

```text
AI UNNECESSARY
```

or:

```text
NON-AI SOLUTION PREFERRED
```

The Root Orchestrator must not suppress these outcomes because the hackathon involves AI.

---

# 53. Phase 4 Gate

Agent 08 performs a targeted audit.

It checks that each serious AI opportunity has:

```text
Problem ID

Gap ID

Workflow step

Non-AI baseline

AI capability

Measurement approach

Trust considerations

Feasibility notes
```

Incomplete opportunities return once for targeted revision.

---

# 54. Phase 5 — Red Team

Spawn Agent 07.

Agent 07 must enter **after** problem, market, and AI claims have been structured.

---

# 55. Agent 07 Context

In accordance with the Runtime Context Loading Matrix, Agent 07 receives:

```text
AGENTS.md (Global Constitution)

Agent 07 profile & Phase 5 Task Packet

research-protocol/problem-card-schema.md (Level 4 Part B: Adversarial Review)

Target Opportunity Package:
- Validated Problem Cards (Levels 1–3)
- Agent 05 Market Landscape & relevant RP-* records
- Agent 06 AI Opportunity Register & preliminary Section 24 drafts
- Relevant Agent 04 trust audits
```

Agent 07 may consult canonical protocols (`source-policy.md`, `evidence-standard.md`) on demand when verifying attack claims.

**Agent 07 must NOT receive:**
- Unrelated raw discovery notes;
- Director synthesis preferences, rankings, or anticipated defenses (preserves adversarial independence).

---

# 56. Agent 07 Independence

Agent 07 should initially review the artifacts independently.

It must not first receive:

- other agents' anticipated defenses;
    
- Director preferences;
    
- favored ideas.
    

Its first task is falsification.

---

# 57. Red Team IDs

Use:

```text
A-001
A-002
```

for critical assumptions.

Use where needed:

```text
RT-001
RT-002
```

for Red Team challenge reports.

Cross-examination later uses separate `CX-` IDs.

---

# 58. Red Team Output

Primary output:

```text
research/raw/CYCLE-XXX-agent-07-red-team.md
```

It should include:

- critical assumptions;
    
- P0/P1 challenges;
    
- missed competitors;
    
- AI-necessity challenges;
    
- safety risks;
    
- feasibility risks;
    
- measurement weaknesses;
    
- disconfirmed opportunities;
    
- opportunities that survived initial challenge.
    

---

# 59. Red Team Focus Limit

Per major opportunity, Agent 07 should prioritize approximately:

```text
maximum 3 P0 challenges

maximum 5 P1 challenges
```

unless exceptional evidence justifies more.

This prevents low-value adversarial noise.

---

# 60. Phase 5 Gate

Agent 08 reads the Red Team report.

It maps challenges to:

- Problem IDs;
    
- Gap IDs;
    
- AI Opportunity IDs;
    
- critical assumptions.
    

Unmapped generic criticism should not enter cross-examination until made specific.

---

# 61. Phase 6 — Cross-Examination

Phase 6 follows:

```text
research-protocol/cross-examination-protocol.md
```

Agent 08 moderates.

---

# 62. Cross-Examination Units

Do not cross-examine the entire project in one giant session.

Create separate examination units around:

```text
one major Problem

one major Gap

one AI Opportunity

or one shared critical assumption
```

This reduces context load.

---

# 63. Cross-Examination Participant Selection

The Root Orchestrator and Agent 08 select only relevant participants.

Example:

Problem involving new Muslims:

```text
Agent 02

Agent 04 if trust-sensitive

Agent 05 if market-sensitive

Agent 06 if AI proposed

Agent 07

Agent 08
```

Do not automatically summon every agent.

---

# 64. Cross-Examination Context Packet

Each participant receives:

```text
target artifact

supporting evidence

relevant counterevidence

relevant Reference Projects

existing challenge IDs

specific questions to resolve
```

Do not provide unrelated workspace history.

---

# 65. Independent Challenge Round

Before discussion, relevant reviewers submit independent structured critiques.

They should not see one another's critiques first.

Agent 08 then merges duplicates.

---

# 66. Cross-Examination Turn Limit

Default:

```text
Challenge

→

Owner response

→

One rebuttal

→

Director resolution
```

Additional turns require materially new evidence.

Do not permit infinite argument.

---

# 67. Cross-Examination IDs

Use:

```text
CX-001

CX-002
```

or target-specific IDs such as:

```text
CX-P103-01

CX-AIOP004-01
```

Do not reuse.

---

# 68. Research Returns From Cross-Examination

If additional evidence is required, Agent 08 sends a narrow research return to the most appropriate agent.

Example:

```text
Agent 05:
find whether competitor X already supports claim-level provenance.

Agent 02:
find stronger evidence about new-Muslim terminology barriers.
```

Do not restart whole agents.

---

# 69. Cross-Examination Return Limit

Normally:

```text
one targeted research return
```

per P0/P1 question.

If the question remains unresolved after meaningful search, record:

```text
UNRESOLVED WITH AVAILABLE EVIDENCE
```

Do not burn unlimited research effort.

---

# 70. Cross-Examination Output

Produce:

```text
research/raw/CYCLE-XXX-cross-examination-summary.md
```

and update:

```text
synthesis/disagreements.md

synthesis/open-questions.md
```

as needed.

---

# 71. Phase 6 Gate

An opportunity may proceed to synthesis when:

```text
P0 challenges:
resolved, disconfirmed, or explicitly blocking

P1 challenges:
resolved or recorded as accepted limitations

problem:
sufficiently supported

gap:
sufficiently investigated

AI:
appropriately justified or rejected

trust:
explicitly documented
```

---

# 72. Blocking P0

An unresolved P0 normally prevents an opportunity from being treated as validated.

Agent 08 may still carry it into synthesis as:

```text
EXPLORATORY
```

or:

```text
HOLD
```

but not as selection-ready.

---

# 73. Phase 7 — Synthesis

Only now may Agent 08 perform full synthesis.

---

# 74. Agent 08 Full Context

Agent 08 may now read:

```text
all Problem Cards

all relevant evidence

all Reference Projects

Agent 05 landscape

Agent 06 AI opportunities

Agent 07 Red Team

cross-examination results

disagreements

open questions
```

Raw discovery notes should be consulted only where structured artifacts are insufficient.

---

# 75. Synthesis Goal

Agent 08 determines:

```text
what is supported

what is weak

what overlaps

what was disproved

what gaps remain

where AI helps

where AI does not help

what trust boundaries apply

what opportunities survived
```

Agent 08 must not yet select a final hackathon winner.

---

# 76. Opportunity IDs

Agent 08 owns:

```text
OPP-001

OPP-002

OPP-003
```

Use `opportunity-map-schema.md`.

---

# 77. Opportunity Map

Agent 08 writes:

```text
synthesis/opportunity-map.md
```

This file is the canonical synthesis artifact.

---

# 78. Synthesis Companion Files

Agent 08 also maintains:

```text
synthesis/disagreements.md

synthesis/open-questions.md
```

Do not hide unresolved material inside the Opportunity Map only.

---

# 79. No Composite Ranking

During Phase 7:

Do not assign:

```text
#1

Winner

Best Idea

92/100
```

The objective is an evidence-grounded opportunity landscape.

Selection occurs later.

---

# 80. Phase 8 — Synthesis Audit

After Agent 08 completes the first Opportunity Map, conduct one final audit.

Spawn Agent 07 again in a **new review invocation**.

Do not rely only on its previous conversational state.

---

# 81. Final Red Team Audit Context

Agent 07 receives:

```text
synthesis/opportunity-map.md

synthesis/disagreements.md

synthesis/open-questions.md

cross-examination summary

selected supporting artifacts as needed
```

Its task is not to restart research.

It audits the synthesis.

---

# 82. Final Audit Questions

Agent 07 checks:

- Were negative findings preserved?
    
- Were confidence levels inflated?
    
- Were unresolved P0 issues hidden?
    
- Did the Director overgeneralize?
    
- Were strong competitors omitted?
    
- Was unnecessary AI restored during synthesis?
    
- Were Islamic trust limitations softened?
    
- Did presentation bias favor one opportunity?
    

---

# 83. Final Audit Output

Write:

```text
research/raw/CYCLE-XXX-synthesis-audit.md
```

Limit the audit to high-impact findings.

---

# 84. Final Director Revision

Agent 08 receives the synthesis audit.

It may:

```text
ACCEPT

REJECT WITH EVIDENCE

REVISE

ADD LIMITATION
```

for each material audit point.

Then it produces the final version of:

```text
synthesis/opportunity-map.md
```

---

# 85. No Infinite Audit Cycle

Only one normal final audit round is allowed.

A second audit occurs only if:

- new external evidence appears;
    
- a P0 error was discovered;
    
- a material source-integrity issue was found.
    

---

# 86. Phase 9 — Complete

The Research Cycle is complete when:

```text
Opportunity Map exists

Problem Cards are traceable

Reference Projects are traceable

AI opportunities are traceable

Red Team findings are traceable

Cross-examination is documented

Disagreements are documented

Open questions are documented

Final synthesis audit completed
```

---

# 87. Completion State

Update the Run Manifest:

```text
CURRENT PHASE:
PHASE 9 — COMPLETE

STATUS:
COMPLETE
```

or:

```text
COMPLETE WITH LIMITATIONS
```

---

# 88. Final Research Package

The completed cycle should contain enough information to move later into:

```text
solution brainstorming

concept selection

hackathon strategy

prototype architecture
```

without repeating problem discovery from scratch.

---

# 89. Agent Read Permissions by Phase (Runtime Matrix Enforcement)

The Orchestrator must enforce strict read permissions to protect agent attention and token budgets:

## Phase 1 (Discovery: Agents 01–03)
- **MUST READ:** `AGENTS.md`, own agent profile, Task Packet, `problem-card-schema.md` (Level 1 only).
- **MAY CONSULT IF NEEDED:** `source-policy.md`, `evidence-standard.md`.
- **MUST NOT READ YET:** `reference-project-schema.md` (full schema), other discovery agents' raw outputs/cards, synthesis files.

## Phase 1 (Trust Discovery: Agent 04)
- **MUST READ:** `AGENTS.md`, Agent 04 profile, Task Packet, `problem-card-schema.md` (Level 1 only), `source-policy.md` (mandatory startup context).
- **MAY CONSULT IF NEEDED:** `evidence-standard.md`.
- **MUST NOT READ YET:** `reference-project-schema.md` (full schema), other discovery agents' raw outputs/cards, synthesis files.

## Phase 2 (Validation: Agent 08)
- **MUST READ:** `AGENTS.md`, Agent 08 profile, Task Packet, `problem-card-schema.md` (Level 2 audit section), newly created Level 1 Problem Cards, Agents 01–04 raw discovery reports.
- **MAY CONSULT IF NEEDED:** `source-policy.md`, `evidence-standard.md`.
- **MUST NOT READ YET:** Future phase schemas (`cross-examination-protocol.md`, `opportunity-map-schema.md`).

## Phase 3 (Market Landscape: Agent 05)
- **MUST READ:** `AGENTS.md`, Agent 05 profile, Task Packet, `reference-project-schema.md` (full canonical schema), `problem-card-schema.md` (Level 3 section), validated Level 2 Problem Cards, Problem Registry.
- **MAY CONSULT IF NEEDED:** `evidence-standard.md`, `source-policy.md`, specific discovery notes if cited.
- **MUST NOT READ YET:** Full raw discovery conversations across all agents (preserves objectivity), Phase 4–8 synthesis files.

## Phase 4 (AI Opportunity: Agent 06)
- **MUST READ:** `AGENTS.md`, Agent 06 profile, Task Packet, `problem-card-schema.md` (Level 4 Part A), validated Problem Cards (Levels 1–3), Problem Registry, Gap Register, Agent 05 Landscape Summary & relevant `RP-*` files.
- **MAY CONSULT IF NEEDED:** Relevant Agent 04 trust findings, specific technical benchmarks.
- **MUST NOT READ YET:** Unrelated Phase 1 raw discovery notes, Phase 6–8 cross-examination and synthesis files.

## Phase 5 (Red Team: Agent 07)
- **MUST READ:** `AGENTS.md`, Agent 07 profile, Task Packet, `problem-card-schema.md` (Level 4 Part B), Target Opportunity Package (Problem Cards Levels 1–4, Agent 05 Landscape, Agent 06 AI Opportunity Register).
- **MAY CONSULT IF NEEDED:** Canonical protocols (`source-policy.md`, `evidence-standard.md`) on demand.
- **MUST NOT READ YET:** Unrelated raw discovery notes, Director synthesis preferences or rankings.

## Phase 6 (Cross-Examination Participants)
- **MUST READ:** `cross-examination-protocol.md` (relevant rules), specific CX target packet (target Problem Card, specific P0/P1 challenge, counterevidence).
- **MAY CONSULT IF NEEDED:** Specific referenced `RP-*` or evidence notes.
- **MUST NOT READ YET:** Entire repository history, unrelated problem cards.

## Phase 7+ (Synthesis & Final Audit: Agent 08 & Agent 07)
- **MUST READ:** `AGENTS.md`, own profile, `opportunity-map-schema.md`, structured artifacts (Level 4 Problem Cards, `RP-*`, `AI-OP-*`, `RT-*`, CX Summary, `disagreements.md`, `open-questions.md`).
- **MAY CONSULT IF NEEDED:** Raw discovery files (strictly to resolve factual ambiguities in structured cards).
- **MUST NOT READ:** Speculative, non-evidenced hackathon pitch ideas.

---

# 90. File Ownership

Canonical ownership:

```text
AGENTS.md
Human / project owner

ORCHESTRATION.md
Human / project owner

research protocols
Human / project owner

Agent profiles
Human / project owner

Problem Cards
Originating Agent 01–04

Evidence
Originating research agent

Reference Projects
Agent 05

AI Opportunity Register
Agent 06

Red Team report
Agent 07

Opportunity Map
Agent 08

Disagreements
Agent 08

Open Questions
Agent 08
```

---

# 91. Shared File Write Rule

No two concurrently running agents may modify the same file.

If parallel agents need to contribute to a shared topic:

- each writes its own file;
    
- Agent 08 later merges structured findings.
    

This avoids race conditions and accidental overwrites.

---

# 92. Revision Rule

When another agent challenges a source artifact:

- it writes a challenge;
    
- it does not overwrite the artifact.
    

The owner revises the artifact after review if warranted.

---

# 93. Change History

Important revisions should preserve:

```text
PREVIOUS CLAIM

NEW CLAIM

WHY CHANGED

EVIDENCE
```

Research evolution should remain visible.

---

# 94. Handoff Format

Use:

```text
[HANDOFF]

FROM:

TO:

RELATED ID:

FINDING:

WHY IT MATTERS:

EVIDENCE:

ACTION REQUESTED:

PRIORITY:
P0 / P1 / P2 / P3
```

---

# 95. Handoff Rule

A handoff is not a command to repeat another agent's research.

It should request something specifically belonging to the receiving agent's expertise.

---

# 96. Handoff Tracking

Agent 08 should track important handoffs in the cycle manifest or problem registry.

Critical handoffs must not disappear.

---

# 97. Research Return Format

Use:

```text
[RESEARCH RETURN REQUEST]

TO:

QUESTION:

RELATED ID:

WHY THIS COULD CHANGE THE DECISION:

EVIDENCE NEEDED:

PRIORITY:

RETURN FORMAT:
```

Avoid:

> research more.

---

# 98. Source Retrieval Discipline

Agents should prefer:

```text
primary sources

official product documentation

original research

direct user evidence
```

where appropriate.

Community sources remain useful for behavioral evidence.

Follow `source-policy.md`.

---

# 99. Search Breadth

Agents should search beyond obvious English-language terms when the problem warrants it.

For Islamic digital products, Arabic search may be essential.

Do not declare absence based solely on English search.

---

# 100. Search Saturation

Stop searching a line of inquiry when:

- strong evidence exists;
    
- new results are repetitive;
    
- two consecutive search attempts yield no materially new result;
    
- additional search has low decision value.
    

---

# 101. Context Budget Discipline

Do not load the entire repository into every agent.

Prefer:

```text
role profile

relevant protocol

target artifact

key evidence

specific task
```

Context quality is more important than context quantity.

---

# 102. Summary Before Transfer

When one phase hands information to the next, transfer structured artifacts rather than entire conversations.

Example:

Agent 06 should receive:

```text
P-103

GAP-004

RP-011

RP-018
```

not:

> 40 pages of unrelated raw discovery.

---

# 103. Raw Notes Are Secondary

Raw reports preserve discovery context.

Canonical downstream decisions should rely primarily on:

- Problem Cards;
    
- Evidence;
    
- Reference Project files;
    
- Gap records;
    
- AI Opportunity records;
    
- challenge records.
    

---

# 104. No Chain-of-Thought Dependency

Agents must not require another agent's hidden reasoning to continue.

Every handoff must be understandable from explicit artifacts and evidence.

---

# 105. Research Verbosity

Agents should be thorough but structured.

Do not maximize output length.

Prefer:

```text
precise evidence
+
structured artifacts
+
clear uncertainty
```

over:

```text
large narrative reports
```

---

# 106. Agent Retry Policy

If an agent execution fails technically:

### First Failure

Retry once using the same task packet.

### Second Failure

Determine whether the task is:

```text
CRITICAL

NONCRITICAL
```

If critical:

> hold the phase.

If noncritical:

> record the missing coverage and continue.

Do not repeatedly restart an agent without understanding failure.

---

# 107. Research Quality Failure

If an agent returns low-quality research rather than a technical failure:

Do not immediately rerun everything.

Agent 08 or the Root Orchestrator should identify:

```text
specific missing component
```

and issue a targeted correction task.

---

# 108. Source Access Failure

If a source cannot be accessed:

- record the limitation;
    
- seek an alternative authoritative source where appropriate;
    
- do not fabricate its contents.
    

---

# 109. Conflicting Evidence

Conflicting evidence is not an execution error.

Preserve it.

Route meaningful conflicts into:

```text
synthesis/disagreements.md
```

---

# 110. Tool Failure

If web/search/tool access fails temporarily:

- record the affected question;
    
- do not pretend it was verified;
    
- continue unaffected work;
    
- retry only when necessary to decision quality.
    

---

# 111. Cost Discipline

Use expensive research effort where uncertainty is decision-critical.

Prioritize:

```text
P0

P1

then P2
```

Do not spend substantial agent calls resolving P3 issues during problem discovery.

---

# 112. Parallelization Policy

Recommended parallel execution:

```text
Phase 1:
Agents 01–04 parallel
```

Possible parallel execution:

```text
independent cross-examination reviews
```

Primarily sequential:

```text
Agent 05

Agent 06

Agent 07

Agent 08 synthesis
```

because later work depends on earlier artifacts.

---

# 113. Maximum Concurrent Council Agents

Default maximum:

```text
4
```

This matches Phase 1.

Do not create large uncontrolled swarms merely because the platform supports them.

---

# 114. Helper Agent Limit

If a specialist is explicitly permitted to create research helpers:

default maximum:

```text
2 helpers
```

Helpers must:

- receive narrow tasks;
    
- return structured evidence;
    
- terminate after their task.
    

---

# 115. Helper Output

A helper should return to its parent agent.

It should not:

- edit synthesis files;
    
- create canonical Problem Cards;
    
- issue final conclusions.
    

The parent remains responsible.

---

# 116. Agent Freshness

When an agent is reused in a later phase, prefer a fresh invocation with:

- its profile;
    
- current target artifacts;
    
- explicit current phase.
    

Do not rely on long-lived conversational memory where structured files exist.

---

# 117. Why Fresh Invocations Matter

Fresh invocation reduces:

- attachment to earlier conclusions;
    
- hidden context drift;
    
- stale assumptions;
    
- context-window dilution.
    

This is particularly important for:

- Agent 07 final audit;
    
- cross-examination reviews.
    

---

# 118. Director Neutrality

Agent 08 must not tell other agents:

> “This is our strongest idea.”

before synthesis concludes.

This could bias further research.

---

# 119. Red Team Neutrality

Agent 07 should not be told which opportunity the team personally prefers.

Its challenge task should remain independent.

---

# 120. Researcher Neutrality

Agents 01–04 should not be asked:

> “Find evidence supporting this project.”

They should be asked:

> “Investigate whether this problem exists and how important it is.”

---

# 121. Technology Neutrality

Agent 06 must test:

```text
AI

versus

strongest realistic non-AI alternative
```

not:

```text
AI

versus

doing nothing
```

---

# 122. Selection Neutrality

This research cycle ends before final project selection.

The Opportunity Map should produce:

```text
selection-ready opportunities
```

not:

```text
the winner
```

---

# 123. Phase Transition Authority

The Root Orchestrator manages mechanical transitions.

Agent 08 determines research readiness.

A phase proceeds when both are satisfied.

---

# 124. Phase Gate Record

Record each transition in the Run Manifest.

Example:

```text
PHASE 3:
COMPLETE

GATE:
PASSED

DIRECTOR NOTES:
Two problems excluded from market analysis due to weak validation.

NEXT:
PHASE 4
```

---

# 125. Hold State

If a critical dependency prevents progression:

```text
STATUS:
HOLD
```

Include:

```text
BLOCKER:

OWNER:

REQUIRED RESOLUTION:
```

Do not continue by inventing missing evidence.

---

# 126. Discontinued Research Direction

When a direction is killed:

Preserve:

```text
what was tested

why it failed

what evidence disproved it
```

Do not delete the research.

---

# 127. Reopening a Discontinued Direction

A discontinued direction should reopen only if:

- materially new evidence appears;
    
- the user segment changes;
    
- a major technology or product change changes feasibility.
    

Do not reopen because an agent still likes the idea.

---

# 128. Opportunity Map Inputs

Before Agent 08 writes the Opportunity Map, the Root Orchestrator verifies that the available inputs include:

```text
validated problems

market evidence

gap analysis

AI opportunity analysis

non-AI alternatives

trust analysis

Red Team review

cross-examination outcomes
```

---

# 129. Final Traceability Test

Every major Opportunity should be traceable approximately as:

```text
OPP-XXX

→

AI-OP-XXX if applicable

→

GAP-XXX

→

P-XXX

→

Evidence

→

External Source
```

plus:

```text
Red Team challenge

→

Cross-examination result
```

---

# 130. Final Audit for Unsupported Claims

Before cycle completion, Agent 08 should inspect statements containing language such as:

```text
no solution exists

users frequently

most users

the best

unique

unprecedented

highly accurate

Islam says

scholars agree
```

These require particularly strong support.

---

# 131. Final Audit for Overclaiming

Replace unsupported:

> “No competitor solves this.”

with supported:

> “No reviewed competitor was found satisfying these specific conditions.”

Precision is required.

---

# 132. Final Audit for Islamic Attribution

Ensure:

```text
source-specific statements remain source-specific
```

and:

```text
legitimate disagreement remains visible
```

Do not let synthesis universalize individual scholarly positions.

---

# 133. Final Audit for Negative Findings

Verify the Opportunity Map includes:

- disconfirmed problems;
    
- already-solved problems;
    
- AI-unnecessary problems;
    
- major limitations.
    

A synthesis containing only promising opportunities is probably incomplete.

---

# 134. Final Audit for AI Bias

Ask:

> Did we preserve a problem only because it enables impressive AI?

If yes:

re-evaluate.

---

# 135. Final Audit for Demo Bias

Ask:

> Is a visually impressive concept receiving more weight than evidence justifies?

If yes:

reframe the synthesis.

---

# 136. Final Audit for Complexity Bias

Ask:

> Are agents, RAG, knowledge graphs, multimodality, or fine-tuning being treated as value rather than implementation choices?

If yes:

remove the technical prestige bias.

---

# 137. Final Cycle Deliverables

A complete cycle should produce at minimum:

```text
Run Manifest

Agents 01–04 discovery reports

Problem Cards

Evidence records

Problem Registry

Agent 05 landscape report

Reference Project records

Gap Register

Agent 06 AI opportunity report

Agent 07 Red Team report

Cross-Examination Summary

Disagreement Register

Open Questions Register

Opportunity Map

Synthesis Audit
```

---

# 138. Definition of Successful Orchestration

The orchestration succeeded if:

- agents investigated independently before convergence;
    
- evidence remains traceable;
    
- research phases occurred in the correct order;
    
- weak problems were allowed to die;
    
- market gaps were challenged;
    
- AI had to justify itself;
    
- trust constraints remained visible;
    
- Red Team findings affected outcomes;
    
- cross-examination changed or validated claims;
    
- Agent 08 synthesized only after adequate evidence;
    
- the Opportunity Map is decision-ready.
    

---

# 139. Definition of Failed Orchestration

The process failed if:

- agents copied one another;
    
- brainstorming happened before problem validation;
    
- Agent 05 only searched for competitors after a favored idea was chosen;
    
- Agent 06 invented problems to justify AI;
    
- Agent 07 was used only to approve existing conclusions;
    
- cross-examination became unstructured conversation;
    
- Agent 08 selected a winner before synthesis;
    
- unsupported claims appeared in the Opportunity Map;
    
- research loops consumed effort without increasing decision quality.
    

---

# 140. Final Principle

The Orchestrator is not trying to maximize the number of agents working.

It is trying to maximize the quality of the information that reaches the decision point.

The correct sequence is:

> **independent discovery before convergence;**

> **problems before products;**

> **evidence before claims;**

> **market reality before novelty;**

> **non-AI alternatives before AI justification;**

> **adversarial challenge before synthesis;**

> **synthesis before selection.**

Agents should not merely communicate.

They should hand off structured evidence.

Agents should not merely disagree.

They should resolve claims through evidence.

Agents should not merely produce ideas.

They should eliminate weak directions until the remaining opportunities are defensible.

The research council succeeds when the final Opportunity Map contains fewer assumptions than the research process started with.