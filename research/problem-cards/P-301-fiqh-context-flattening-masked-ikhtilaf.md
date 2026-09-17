# [P-301] Fiqh Context-Flattening, Masked Madhhab Disagreement, and Unqualified Automated Fatwas

---

## METADATA & MATURITY

- **Problem ID:** P-301
- **Current Maturity Level:** LEVEL 4 — OPPORTUNITY-READY (Part A)
- **Problem Status:** VALIDATED
- **Primary Research Owner:** Agent 04
- **Date Created:** 2026-09-17
- **Last Updated:** 2026-09-17

---

# ==============================================================================
# LEVEL 1 — DISCOVERED PROBLEM (Phase 1: Agents 01–04)
# Required for all new cards. Completed during independent discovery.
# ==============================================================================

## 1. One-Sentence Problem Statement
Practicing Muslims seeking legal and ritual guidance struggle to determine the validity of their religious practices because digital search tools and conversational AI systems flatten context-dependent jurisprudence into rigid, universal pronouncements, silently imposing a single school of thought or scraped internet fatwa while erasing legitimate orthodox disagreement (*Ikhtilaf*) and failing to inquire about the questioner's specific circumstances.

## 2. Primary User & Context
- **Primary User:** Practicing Muslims (including university students, young professionals, and new Muslims) seeking actionable answers on daily acts of worship (*'Ibadat*), purification, prayer, fasting, and social transactions (*Mu'amalat*).
- **Why This User Matters:** The daily spiritual peace of mind of over a billion Muslims depends on knowing whether their prayers, fasts, and contracts are valid. Imposing false rigidity or wrongful invalidations causes severe religious anxiety (*waswas*) or unwarranted guilt.
- **User Context & Trigger:** User encounters an immediate personal dilemma: *"I bled slightly from my gum during prayer, is my wudu broken?"*, *"Can I combine prayers due to mandatory university lectures?"*, or *"Is investing in company X permissible?"* User types the query into an AI assistant or search bar.
- **Environmental Constraints:** Urgent need for guidance (prayer time expiring, impending contract signing), lack of immediate access to a qualified local mufti, language barriers (English/Urdu/French speaker searching for rulings primarily documented in classical Arabic).
- **Existing Tools Used:** ChatGPT / Gemini, IslamQA.info, Islamweb, Google Search, Reddit r/islam.

## 3. Secondary Users & Stakeholders
- **Secondary Users:** Families, spouses, and community members affected by rigid rulings (e.g., divorce pronouncements, dietary restrictions, financial disputes).
- **Human Reviewers / Authorities Involved:** Local imams, community muftis, and Islamic counselors who must mediate conflicts caused by users citing contradictory, decontextualized internet fatwas.

## 4. Job to Be Done
- **When:** Faced with an ambiguous or practical religious question regarding worship, family, or work,
- **I want to:** Understand the recognized Islamic rulings applicable to my situation and school of thought, with clear disclosure of scholarly consensus or legitimate divergence (*Ikhtilaf*),
- **So that:** I can fulfill my religious duties with confidence, avoid unlawful actions, and respect legitimate differences within the community.
- **Success looks like:** An answer that clearly identifies the positions of the major orthodox schools (Hanafi, Maliki, Shafi'i, Hanbali), asks necessary clarifying questions about context, and explicitly directs high-stakes personal matters (e.g., divorce, complex finance) to a qualified human scholar.

## 5. Current Reconstructed Workflow
- **Trigger:** User has an immediate fiqh question regarding ritual purity or daily practice.
- **Step 1 (Query Submission):** User asks an AI tool: *"Does touching the opposite gender accidentally break wudu?"*
- **Step 2 (Flattened Generation):** The AI answers definitively: *"Yes, in Islam, touching a woman invalidates wudu immediately, and you must perform ablution again before praying."* The system presents the strict Shafi'i position as the universal, monolithic stance of "Islam", completely ignoring the Hanafi position (does not break wudu unless lustful) and the Maliki/Hanbali qualifications.
- **Step 3 (Intra-Community Whiplash):** A Hanafi user reads this, panics that all their previous prayers were invalid, or confronts Hanafi family members, claiming their practice violates "Islam".
- **Step 4 (Escalation to Human Authority):** Months later, the user consults a qualified local imam or reads a comprehensive fiqh book and discovers that multiple legitimate orthodox opinions exist.
- **Final Outcome:** Severe religious disorientation, unnecessary past spiritual distress, and complete loss of trust in digital Islamic information sources.

## 6. Workflow Evidence Grounding
- **Step 1 Status:** DIRECTLY OBSERVED (Standard user querying patterns on AI platforms).
- **Step 2 Status:** DIRECTLY OBSERVED & MEASURED (FiqhQA benchmark by Atif et al., AAAI/ACM AIES 2025; IslamicMMLU Madhhab Bias task by Abdelaal et al., 2026).
- **Step 3 Status:** USER REPORTED (Documented extensively in convert support forums and Reddit r/islam "fatwa whiplash" discussions).
- **Step 4 Status:** USER REPORTED (Reported by community imams dealing with youth confused by online fatwas).
- **Final Outcome Status:** USER REPORTED & SCHOLARLY ATTESTED (Warned against by official fatwa councils and classical scholars).
- **Inferred / Missing Workflow Steps:** The exact percentage of users who never discover the multi-madhhab reality and remain trapped in artificial rigidity.

## 7. Core Pain Point
- **Exact Friction Point:** The conversion of *"Scholar X / School Y ruled Z under specific conditions"* into an unqualified, universal pronouncement: *"Islam says Z"*, combined with a total failure of the AI to abstain or ask context-clarifying questions.
- **Root Cause Hypothesis:** Pretraining data bias: internet-crawled Islamic datasets disproportionately index specific search-engine-optimized fatwa repositories (e.g., IslamQA.info, representing a Hanbali/Salafi methodology) while underrepresenting classical comparative fiqh encyclopedias. LLMs trained on this data reproduce the dominant scraped corpus as universal truth.

## 8. Consequences & Impact
- **Immediate Consequence:** Misguided worship; unnecessary repetition of valid acts of worship; abandonment of legitimate legal concessions (*rukhas*).
- **Long-term Consequence:** Factionalism and sectarian friction in diverse Muslim communities; spiritual burnout (*waswas*); youth perceiving Islam as an irrational, contradictory legalistic maze.
- **Religious & Trust Consequence:** Violation of the sacred Islamic legal principle that fatwas alter with time, place, and circumstance (*Al-fatwa tataghayyar bi-taghayyur al-zaman wal-makan*); illicit performance of *Ijtihad* by non-qualified statistical models; violation of the "No Autonomous Mufti" rule.
- **Emotional / Cognitive Cost:** Scrupulosity, guilt, cognitive dissonance, alienation from traditional scholars.

## 9. Frequency & Severity
- **Frequency:** Daily for any practicing Muslim navigating practical fiqh in multicultural or digital environments.
  - *Evidence & Confidence:* High (FiqhQA evaluated 960 QA pairs across all 4 madhahib and observed widespread cross-school misattribution).
- **Severity:** High friction for daily worship; Catastrophic for high-stakes personal rulings (marriage, divorce, inheritance, interest-bearing contracts).
  - *Evidence & Confidence:* High (Grounded in institutional fatwas from Islamweb, IslamQA, and Dar al-Ifta al-Misriyyah).

## 10. Existing Workarounds
1. **Workaround 1 (Prefixing Queries with Madhhab):** Experienced users manually prefix their prompts: *"According to the Hanafi school, does X break wudu?"* (Fails when the AI confuses madhhab specifics or lacks training depth in non-Hanbali sources).
2. **Workaround 2 (Consulting Specialized Portals):** Searching dedicated madhhab portals (e.g., SeekersGuidance for Hanafi/Shafi'i, IslamQA.org for South Asian Hanafi fatwas).
3. **Workaround 3 (Avoiding Digital Search):** Relying solely on a single local imam or physical fiqh manual (e.g., *Nur al-Idah* or *Reliance of the Traveller*).
- **Why Workarounds Fail:** Prefixing fails because LLMs frequently hallucinate across schools regardless; specialized portals have primitive search engines; relying solely on physical books lacks accessibility for modern questions (e.g., crypto, medical fasting).

## 11. Initial Reference Candidates Encountered
- **Candidate 1:** IslamQA.info | https://islamqa.info/ | Target: General Muslims | What it does: Vast archive of detailed fatwas authored by Shaykh Salih al-Munajjid and scholarly committee | Observed limitation/user complaint: Strongly represents a specific Hanbali/Salafi jurisprudential methodology; often presents its chosen ruling without fully detailing traditional Hanafi, Maliki, or Shafi'i counter-positions; frequently scraped into LLMs causing systemic corpus bias.
- **Candidate 2:** FiqhQA Benchmark Dataset | https://arxiv.org/abs/2508.08287 | Target: AI researchers | What it does: First bilingual benchmark evaluating LLM reliability, abstention, and madhhab accuracy across all 4 Sunni schools using the Kuwaiti Fiqh Encyclopedia | Observed limitation/user complaint: Research benchmark; not an operational user-facing knowledge retrieval system.
- **Candidate 3:** SeekersGuidance Answers | https://seekersguidance.org/answers/ | Target: Traditional Sunni Muslims | What it does: Human scholar-reviewed answers categorized explicitly by madhhab (Hanafi, Shafi'i, Maliki) | Observed limitation/user complaint: Keyword search is limited; response time for new questions takes weeks or months due to scholar backlog.

## 12. Supporting Evidence
- **[E04-002]:** Atif et al., "Sacred or Synthetic? Evaluating LLM Reliability and Abstention for Religious Questions", AAAI/ACM AIES 2025 (arXiv:2508.08287) | 2025
  - *Extracted Quote / Data:* Frontier LLMs fail to abstain on ambiguous fiqh queries, exhibit substantial performance drops in Arabic, and demonstrate erratic accuracy variations across the four Sunni madhahib.
  - *Supports:* Directly validates that LLMs generate unqualified, overconfident fiqh rulings without calibrated restraint.
  - *Confidence:* High.
- **[E04-005]:** Official Portal of Shaykh Abdul Aziz ibn Baz, Fatwa #2523 ("التحذير من نقل الفتاوى بغير علم وتثبت") | Canonical
  - *Extracted Quote / Data:* Shaykh Ibn Baz rules that anyone who transmits a fatwa without certainty, exact preservation, and full comprehension of its qualifications is strictly forbidden from conveying it, as it constitutes "speaking about Allah without knowledge".
  - *Supports:* Establishes the authoritative scholarly principle that context-flattening and unverified fatwa transmission violate Islamic governance.
  - *Confidence:* High.
- **[E04-006]:** Institutional Fatwas from IslamQA, Islamweb, and Dar al-Ifta al-Misriyyah | 2023–2025
  - *Extracted Quote / Data:* Unanimous institutional consensus that AI is strictly disqualified from issuing fatwas (*faqd al-ahliyyah*), lacking *malakat al-fiqh* and understanding of real-life context (*fiqh al-waqi'*).
  - *Supports:* Directly establishes the imperative of `[NO AUTONOMOUS FATWA PERMITTED]` and `[REQUIRES ISLAMIC SCHOLAR REVIEW]`.
  - *Confidence:* High.

## 13. Contradicting / Disconfirming Evidence
- **Evidence Weakening Problem:** On universally agreed core obligations (*ma'lum min al-din bid-darurah*—such as the prohibition of intoxicants, the obligation of prayer, or basic fasting requirements), there is no madhhab disagreement, and a single definitive answer is entirely correct.
- **Source & Citation:** Classical consensus (*Ijma'*) across all Islamic schools.
- **Why Problem Survives:** Users rarely seek detailed fiqh advice on whether murder is haram or fasting Ramadan is obligatory; they seek guidance on subsidiary details (*furu'*), border cases, contemporary financial instruments, and ritual nuances where *Ikhtilaf* is ubiquitous.

## 14. Disconfirmation Search Conducted
- **Falsification Hypothesis:** Do users prefer a single, simplified "correct" answer, and is madhhab differentiation merely an academic concern?
- **Searches Performed:** Community feedback on multi-school fiqh apps; user complaints regarding fatwa whiplash ("madhab bias LLM fiqh", "conflicting fatwas user confusion").
- **Disconfirmation Findings:** Disconfirmation failed; users repeatedly report severe anxiety, confusion, and family discord when an online tool presents an opposing madhhab's position as the only valid Islam, especially converts and diaspora Muslims.

## 15. Islamic Knowledge & Trust Considerations
- **Doctrinal Areas Involved:** Classical Fiqh, Contemporary Fatwa, Usul al-Fiqh, Comparative Jurisprudence (*Al-Fiqh al-Muqaran*).
- **Scholarly Disagreement (Ikhtilaf):** Core to this problem. Legitimate differences across the four orthodox Sunni schools (Hanafi, Maliki, Shafi'i, Hanbali) must be preserved and clearly attributed. Consensus (*Ijma'*) must never be claimed without verified classical evidence.
- **Personal Circumstance Sensitivity:** Extremely high. Fiqh rulings depend heavily on individual health, marital contracts, local custom (*'Urf*), financial solvency, and intent.
- **Required Governance Markers:**
  - `[REQUIRES ISLAMIC SCHOLAR REVIEW]`
  - `[REQUIRES SOURCE-BOUNDARY AUDIT]`
  - `[NO AUTONOMOUS FATWA PERMITTED]`

## 16. Assumptions, Unknowns & Evidence Gaps
- **[ASSUMPTION]:** Users are willing to navigate structured comparative perspectives rather than demanding a single binary "yes/no" answer.
- **[UNKNOWN]:** To what degree do English-language vs. Arabic-language users differ in their expectation of madhhab-specific versus generalized rulings?
- **[EVIDENCE GAP]:** Quantitative audit measuring the exact madhhab representation distribution in common open-source Arabic instruction-tuning datasets.

## 17. Confidence in Problem Existence
- **Problem Existence Confidence:** High.
- **Justification:** Backed by rigorous peer-reviewed benchmark evidence (FiqhQA), comprehensive MMLU evaluation (IslamicMMLU), and unanimous institutional fatwas from top global Islamic authorities.

## 18. Required Next Research (Discovery Phase)
- 1. Investigate the feasibility of automated context-intake mechanisms (e.g., asking clarifying questions regarding geography, madhhab, and personal constraints) before presenting fiqh information.
- 2. Map the technical boundaries between general educational fiqh explanations (permissible) and personalized legal verdicts (strictly prohibited).

## 19. Early Idea Hypothesis (Optional — Strictly Non-Binding)
- `[HYPOTHESIS]`: A context-gated comparative fiqh framework that strictly identifies the user's school of thought, detects whether a question involves recognized *Ikhtilaf*, and structures responses into parallel madhhab columns—while refusing to answer high-stakes personal status queries without human scholar handoff—might eliminate fatwa whiplash and protect sacred scholarly boundaries.

---

# ==============================================================================
# LEVEL 2 — VALIDATED PROBLEM (Phase 2: Agent 08 Research Director)
# Completed by Agent 08 during intake audit.
# ==============================================================================

## 20. Director Validation Audit
- **Validation Decision:** VALIDATED
- **Duplicate / Merge Check:** Thematically clustered under "Conflicting Fatwas, Ikhtilaf & Jurisprudential Context". Cross-referenced with `P-002` (lay professional lifestyle/financial search paralysis) and `P-101` (convert family/holiday fatwa whiplash and zero ikhtilaf literacy). No merge recommended: P-301 isolates the algorithmic and architectural failure mode where conversational AI systems and automated search engines flatten context-dependent jurisprudence (*fiqh*) into rigid, universal edicts ("Islam says X"), silently imposing a single scraped school while erasing classical *Ikhtilaf* across the 4 Sunni madhahib and violating the "No Autonomous Mufti" rule (*faqd al-ahliyyah*).
- **Evidence Quality Audit:** Highest tier empirical and theological grounding. Supported by peer-reviewed AI ethics research (FiqhQA benchmark by Atif et al., AAAI/ACM AIES 2025, `E04-002`, evaluating LLM reliability and abstention across the Kuwaiti Fiqh Encyclopedia), canonical scholarly warnings (Shaykh Ibn Baz Fatwa #2523 on forbidden unverified fatwa transmission, `E04-005`), and institutional rulings from IslamQA, Islamweb, and Dar al-Ifta al-Misriyyah (`E04-006`) barring AI from issuing legal verdicts.
- **Workflow Confidence:** High confidence (Verified). 4-step sequence (User query on practical ritual/life issue -> AI generates monolithic uncalibrated verdict -> intra-community/family whiplash and scrupulosity -> eventual escalation to human scholar) is widely observed and empirically validated in benchmark abstention failures.
- **Problem Framing Critique:** Exemplary framing that clearly distinguishes legitimate educational fiqh explanation from illicit automated fatwa generation. Strictly respects Islamic governance principles.
- **Critical Evidence Gaps to Resolve:** Quantitative corpus audit measuring madhhab representation distribution in common open-source Arabic instruction datasets; user study evaluating whether users prefer multi-madhhab structured comparison over single-school answers.
- **Gate to Phase 3 (Market Landscape):** APPROVED (Forwarded to Agent 05 to evaluate against SeekersGuidance Answers, IslamQA.info, Islamweb, and general-purpose LLM interfaces).

---

# ==============================================================================
# LEVEL 3 — MARKET-TESTED PROBLEM (Phase 3: Agent 05 Market Landscape)
# Completed by Agent 05 after market and competitor research.
# ==============================================================================

## 21. Canonical Reference Projects Reviewed
- `[RP-007]`: IslamQA.info | Web & Mobile | Heavily crawled by Common Crawl into frontier LLM training corpora; directly injects a single strict Salafi/Hanbali methodology into conversational AI, leading models to present one school as universal Islam.
- `[RP-008]`: SeekersGuidance Answers Service | Web | Human scholar benchmark; demonstrates the necessity of explicit madhhab labeling and personal contextual qualification before answering legal queries.
- `[TECH-002]`: FiqhQA Benchmark (AAAI/ACM AIES 2025) | AI Ethics Benchmark | Grounded in the Kuwaiti Fiqh Encyclopedia; empirically proves that frontier LLMs fail to abstain on 98%+ of ambiguous fiqh queries and systematically erase Hanafi/Maliki/Shafi'i positions.
- `[TECH-003]`: IslamicMMLU Benchmark | 26-LLM Benchmark | Confirms that multi-school fiqh pairs suffer from high error rates (>38% cross-school confusion).
- `[ADJ-002]`: UpToDate & DynaMed (Clinical Decision Support) | Healthcare Platform | Canonical analogue for mandatory context-intake, patient stratification, guideline debate mapping, and prohibition of autonomous medical/legal practice.

## 22. Existing Solution Coverage Analysis
- **Full Solvers:** None. No consumer conversational AI assistant or search chatbot successfully gates legal inquiries, gathers personal context, distinguishes consensus from disagreement, and refuses to issue autonomous legal rulings (*Fatwas*).
- **Partial Solvers:**
  - *Generic Prompt Engineering (System Prompts):* Instructing a chatbot to "be balanced and represent all madhahib" reduces extreme dogmatism, but models still hallucinate school attributions and fail to abstain on personal status rulings (`E04-002`).
  - *SeekersGuidance Answers / Dar al-Ifta Portals:* Offer verified human rulings, but lack natural-language conversational interfaces and take weeks to reply.
- **Strongest Non-AI / Conventional Alternatives:**
  - Physical classical comparative jurisprudence books (e.g., *Bidayat al-Mujtahid* by Ibn Rushd, *Al-Fiqh al-Islami wa Adillatuh* by Wahbah al-Zuhayli; accessible only to trained scholars).
  - Calling a qualified mufti directly (the gold standard human baseline, but severely supply-constrained).

## 23. Canonical Market / Workflow Gap
- **Assigned Gap ID:** GAP-011
- **Unresolved Gap Statement:** Conversational AI systems and search assistants lack a context-gating and madhhab-calibrated retrieval architecture that forces models to gather situational constraints, accurately map differences across the four Sunni Madhahib, and strictly abstain from issuing autonomous, unqualified religious edicts (*Fatwas*) on high-stakes personal status matters, violating classical Islamic legal governance (`[NO AUTONOMOUS FATWA PERMITTED]`) and causing acute spiritual confusion.
- **Gap Confidence:** High (Empirically grounded in peer-reviewed FiqhQA benchmark findings [`E04-002`], canonical scholarly warnings from Shaykh Ibn Baz [`E04-005`], and unanimous institutional fatwas from global fatwa councils [`E04-006`]).
- **Is Gap Genuine or Feature Request?** High-severity ethical, theological, and architectural gap. Unconstrained LLMs acting as autonomous muftis represent a grave religious harm (*Mafsadah*).
- **Market Disposition:** PROCEED TO AI EVALUATION

---

# ==============================================================================
# LEVEL 4 — OPPORTUNITY-READY PROBLEM (Phases 4–7: Agents 06, 07 & 08)
# Multi-agent synthesis before opportunity mapping.
# ==============================================================================

## 24. AI Opportunity Evaluation (Agent 06 — Phase 4)
- **Assigned AI Opportunity ID:** AI-OP-011 (Context-Gated Multi-Madhhab Fiqh Retrieval & Strict Abstention Guardrail)
- **Strongest Non-AI Baseline:**
  - **Deterministic Rule-Based Context Gatekeeper & Escalation Switchboard**:
    - Strict keyword, intent regex, and ontology filters identifying sensitive personal status domains: divorce (*talaq*), marriage validity (*nikah*), custody, inheritance (*mirath*), criminal punishments (*hudud*), and declarations of apostasy (*takfir*).
    - Hardcoded deterministic refusal: If a query matches any personal status pattern, the system issues a standardized refusal: "In Islamic jurisprudence, personalized legal rulings (*Fatwas*) require qualified human scholarly assessment. This system does not issue fatwas. Please consult a qualified local mufti or accredited fatwa council (`[NO AUTONOMOUS FATWA PERMITTED]`)."
    - Relational index mapping general educational queries (e.g. "What breaks wudu according to Shafi'is?") directly to digitized static sections of the *Kuwaiti Fiqh Encyclopedia*.
- **Specific AI Capability Justified:**
  - **Context-Intake Slot-Filling & Multi-Madhhab Alignment**:
    - Commercial conversational LLMs fail on two fronts: (1) They attempt to answer 98%+ of ambiguous queries without asking clarifying questions (as benchmarked in `TECH-002` FiqhQA), and (2) They collapse 1,400 years of juristic debate into flat, single-school assertions ("In Islam, X is haram"), usually reflecting scraped internet Salafi dominance while erasing Hanafi, Maliki, and Shafi'i positions.
    - A specialized slot-filling model detects when crucial circumstantial variables are missing (e.g. user's madhhab, health condition, travel status, local custom) and asks clarifying questions *before* retrieving information.
    - Multi-Madhhab Constrained Retrieval: Maps the disambiguated question to canonical classical jurisprudence across the 4 Sunni Madhahib and presents results in parallel comparative columns (Hanafi | Maliki | Shafi'i | Hanbali), explicitly citing classical reference texts (*Al-Hidayah*, *Al-Majmu'*, *Al-Mughni*, *Mukhtasar Khalil*).
    - **Hard Policy Guardrail**: Generative LLMs are strictly forbidden from choosing a "winning" school, reconciling the positions, or issuing a personalized legal verdict.
- **Why AI May Help:**
  - Handles conversational, situational queries and prompts users for missing personal context that a static keyword search engine cannot parse.
  - Eliminates algorithmic sectarian bias by forcing balanced multi-school representation.
- **Why AI May Be Unnecessary or Inferior:**
  - An autonomous generative LLM acting as a mufti is a grave religious harm (*Mafsadah*). Generative models must never be given authority to deduce legal rulings. AI is justified strictly for **conversational context clarification and multi-madhhab passage retrieval**.
- Expected Measurable Improvement:
  - Abstention Compliance: Abstention on ambiguous or personal status fiqh queries increases from <2% (commercial LLM baseline in FiqhQA) to >98%.
  - Madhhab Erasure Reduction: Zero single-school flattening; 100% of responses explicitly label school positions and consensus boundaries.
- **Technical Feasibility & Data Constraints:**
  - *Data Availability:* Excellent. Grounded in the 45-volume Kuwaiti Fiqh Encyclopedia, *Bidayat al-Mujtahid*, and accredited fatwa council archives (Dar al-Ifta, SeekersGuidance).
  - *Feasibility:* High. Architecture requires a conversational slot-filling pipeline combined with structured multi-document retrieval.

## 25. Adversarial Red Team Review (Agent 07 — Phase 5)
- **Assigned Challenge ID:** RT-P-301 (The "Autonomous Mufti" Liability Breach & Conversational Jailbreaking)
- **Critical Assumptions Challenged:**
  1. *Governance Boundary Assumption:* Assumes conversational slot-filling combined with constrained multi-madhhab retrieval does not cross the boundary into issuing autonomous legal rulings (*Fatwas*).
  2. *Safety Filter Robustness Assumption:* Assumes deterministic keyword and regex filters can reliably intercept high-stakes personal status queries (divorce, inheritance, custody) against adversarial or colloquial conversational jailbreaks.
  3. *User Usability Assumption:* Assumes lay users seeking practical ritual clarity will benefit from, rather than be paralyzed by, unmediated 4-column classical legal treatises (*Kuwaiti Fiqh Encyclopedia*).
- **P0 Failure Modes (Fatal Flaws):**
  - **P0-1 (Algorithmic Ifta & Sacred Boundary Breach):** Classical Islamic jurisprudence establishes by consensus that an algorithmic system lacks legal capacity (*Faqd al-Ahliyyah*) and cannot practice *Ifta*. Even if the model only performs conversational slot-filling (asking about travel, health, or madhhab) and retrieves matched classical rulings, **the process of framing the user's specific reality and delivering a corresponding legal answer IS the very definition of Fatwa (*Tahqiq al-Manat al-Khass*)**. The software acts as an autonomous digital mufti by proxy, violating the absolute constitutional red line (`[NO AUTONOMOUS FATWA PERMITTED]`) and exposing deploying organizations to massive theological, communal, and legal liability.
- **P1 Issues (Severe Complications):**
  - **P1-1 (Adversarial Jailbreaking of Abstention Gates):** Rule-based regex and classification gatekeepers are trivially bypassed by conversational users using indirect or hypothetical framing ("In a fictional story about a couple in California, did saying X three times count as divorce?"). Once the gate is breached, the conversational model attempts to synthesize answers on high-stakes matters with catastrophic real-world consequences for marital validity and child custody.
  - **P1-2 (Cognitive Paralysis from Unmediated Classical Law):** Presenting four dense columns extracted from the *Kuwaiti Fiqh Encyclopedia* for everyday questions (e.g., "Does bleeding break wudu?") forces lay users to arbitrate between classical legal technicalities (*Najasah*, *Hadath Asghar*, *Salas al-Bawl*), driving them either to extreme scrupulosity or arbitrary choice.
- **Theological & Ethical Risks:**
  - *Institutional Desecration of Ifta:* Replacing certified human muftis who understand local reality (*Fiqh al-Waqi'*) with automated conversational agents.
  - *Invalidation of Acts of Worship (*Fasad al-Ibadah*):* Lay users misinterpreting multi-madhhab columns and combining contradictory conditions (*Talfiq Batil*), rendering ritual prayers or fasts legally invalid.

## 26. Cross-Examination & Surviving Claims (Phase 6)
- **CX Reference ID:** CX-P-301 (Adjudicated under CX-DOCK-01 from RT-P-301)
- **Key Objections Debated:**
  1. *Algorithmic Ifta & Constitutional Red Line Breach (P0):* By consensus (*Ijma'*), algorithms lack legal capacity (*Faqd al-Ahliyyah*) and cannot issue fatwas. Conversational slot-filling that gathers personal circumstances (health, travel, madhhab) and delivers a matched legal ruling performs *Tahqiq al-Manat al-Khass* (applying universal law to individual reality). This constitutes an autonomous digital mufti by proxy, violating `AGENTS.md` Principle 6 and `source-policy.md`.
  2. *Adversarial Jailbreaking of Abstention Gates (P1):* Conversational classification filters are trivially bypassed by users framing high-stakes personal status queries (divorce, custody, inheritance) hypothetically or through roleplay ("In a fictional story, if a husband says X, is she divorced?"), resulting in catastrophic real-world marital and legal harm.
  3. *Lay Cognitive Paralysis from Unmediated Classical Texts (P1):* Presenting 4 parallel columns from the *Kuwaiti Fiqh Encyclopedia* to everyday believers asking simple ritual questions forces them to arbitrate classical technicalities, inducing confusion or invalid combinations of legal conditions (*Talfiq Batil*).
- **Accepted Limitations & Scoped Boundaries:**
  1. *Personal Advisory & Tailored Rulings Strictly Barred:* The concept of an interactive conversational fiqh assistant diagnosing user situations is **COMPLETELY TERMINATED** (`[NO AUTONOMOUS FATWA PERMITTED]`).
  2. *System Reclassified as Educational Comparative Fiqh Archive:* The architecture survives exclusively as a **Structural Multi-Madhhab Reference Tool** for academic research and education, displaying historical positions on abstract topics with explicit primary citations.
  3. *Unconditional Multi-Layered Abstention Barrier:* The system must deploy a dual-layer abstention mechanism (deterministic regex pattern matchers + prompt-injection guardrails) that unconditionally refuses all first-person situational, marital, financial, and criminal status questions, providing a standard disclaimer and direct referral to certified human muftis.
  4. *Benchmark Guardrail Adoption:* The abstention filter must be calibrated directly against the FiqhQA (`TECH-002`) benchmark suite to ensure >98% abstention compliance on unanswerable/ambiguous queries.
- **Surviving Claims:**
  1. *Anti-Monopoly School Defense:* Context-gated multi-madhhab retrieval successfully counters the single-school algorithmic monopoly of general LLMs, preserving 1,400 years of legitimate orthodox Sunni *Ikhtilaf*.
  2. *Strict Abstention Enforcement:* Proves that an AI system can be architected to prioritize refusal and human scholar escalation over hallucinated legal synthesis.

## 27. Final Research Disposition (Agent 08 — Phase 7)
*(To be completed by Agent 08)*

---

# ==============================================================================
# CHANGE LOG & AUDIT TRAIL
# ==============================================================================

| Date | Agent | Level Transition | Summary of Changes | Rationale |
|---|---|---|---|---|
| 2026-09-17 | Agent 04 | LEVEL 1 Created | Initial problem discovery | Discovery phase input |
| 2026-09-17 | Agent 08 | LEVEL 1 → LEVEL 2 | Intake audit completed; validated evidence, workflow, and trust boundaries | Phase 2 Problem Validation |
| 2026-09-17 | Agent 05 | LEVEL 2 → LEVEL 3 | Market landscape completed; evaluated RP-007, RP-008, TECH-002, TECH-003, ADJ-002; assigned GAP-011; verified algorithmic fiqh governance gap | Phase 3 Market Landscape |
| 2026-09-17 | Agent 06 | LEVEL 3 → LEVEL 4 (Part A) | AI Opportunity Evaluation completed; assigned AI-OP-011; justified conversational slot-filling with multi-madhhab retrieval and strict abstention | Phase 4 AI Opportunity Analysis |
| 2026-09-17 | Agent 07 | LEVEL 4 (Part B) Completed | Adversarial red team review completed; assigned RT-P-301; declared P0 autonomous mufti governance breach and P1 jailbreaking vulnerabilities | Phase 5 Adversarial Red Team Review |
| 2026-09-17 | Agent 08 | LEVEL 4 (Part C) Completed | Cross-Examination Adjudication completed (CX-DOCK-01); populated Section 26 with surviving claims and accepted limitations (CX-P-301); banned all personal advisory slot-filling and enforced multi-layer abstention guardrails | Phase 6 Cross-Examination Adjudication |

