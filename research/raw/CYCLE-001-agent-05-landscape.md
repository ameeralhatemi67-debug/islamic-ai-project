# CYCLE-001 Master Market & Reference Landscape Report
## Comprehensive Competitor Matrix, Workflow Coverage Breakdown & Canonical Gap Register
### Islamic AI Challenge Research Lab — Phase 3 Market Investigation

---

- **Document ID:** CYCLE-001-LANDSCAPE-01
- **Cycle:** CYCLE-001
- **Current Phase:** PHASE 3 — MARKET LANDSCAPE INVESTIGATION
- **Author:** Agent 05 — Market & Reference Landscape Researcher
- **Target Audience:** Agent 06 (AI Opportunity Researcher), Agent 07 (Red Team & Skeptic), Agent 08 (Research Director), and Research Council
- **Date Created:** 2026-09-17
- **Status:** COMPLETE & AUTHORITATIVE (LEVEL 3 MARKET-TESTED BASELINE)
- **Governing Charters:** `AGENTS.md`, `agents/05-market-landscape-researcher.md`, `research-protocol/reference-project-schema.md`, `research-protocol/problem-card-schema.md`

---

## 1. Executive Summary

In accordance with Phase 3 of the Islamic AI Challenge Research Protocol, Agent 05 has executed an exhaustive, evidence-grounded market, competitor, and reference-project investigation across all twelve (12) Level 2 validated Problem Cards (`P-001` through `P-302`) and the four (4) thematic clusters established in the Authoritative Problem Registry.

### 1.1 High-Level Landscape Diagnosis
The contemporary Islamic digital software ecosystem is characterized by **rich content silos separated by severe architectural chasms**:
1. **The Classical Arabic Desktop Silo:** Monumental digital encyclopedias like *Al-Maktabah al-Shāmilah* (`RP-004`) and *Dorar.net* (`RP-001`) contain millions of classical texts, isnads, and scholarly rulings. However, they remain trapped behind legacy desktop interfaces, classical Arabic morphological constraints, and exact-string boolean search engines. They are completely inaccessible to non-Arabic speaking Muslims, bilingual translators, and mobile social media consumers.
2. **The Superficial Bilingual Reading Layer:** Public-facing web portals like *Sunnah.com* (`RP-002`) and *Quran.com* (`RP-014`) offer clean typography and accessible English translations, but are architecturally built as static, linear codices. Their search engines rely on brittle exact-substring matching, miss hundreds of secondary collections, and lack contextual exegesis (*Tafsir*, *Sabab al-Wurud*) and multi-scholar authentication synthesis.
3. **The Polarized & Fragmented Fatwa Web:** Web search for Islamic jurisprudence is dominated by *IslamQA.info* (`RP-007`), whose unmatched SEO surfaces monolithic, hyper-rigid rulings that frequently trigger severe religious scrupulosity (*waswas*) among lay professionals and cause catastrophic family alienation among new converts. Meanwhile, balanced multi-madhhab portals like *SeekersGuidance Answers* (`RP-008`) suffer from multi-week submission backlogs and weak search discovery, while uncurated aggregators like *IslamQA.org* (`RP-009`) dump contradictory rulings with zero synthesis.
4. **The Generative AI Hallucination Wild West:** Emerging Islamic AI chatbots (*AskSunnah*, *HadithGPT*, *IslamicGPT*; `RP-006`) and frontier LLMs attempt to answer religious queries, but consistently suffer from autoregressive hallucination. They fabricate canonical citations ("phantom attributions" pointing to nonexistent Bukhari numbers; `TECH-001`), fail to abstain on ambiguous fiqh queries, and erase classical *Ikhtilaf* by flattening rich legal traditions into flat universal edicts (`TECH-002`, `TECH-003`).

### 1.2 Summary of Market Audit Outcomes
- **Total Problem Cards Tested:** 12
- **Cards Advanced to LEVEL 3 — MARKET-TESTED:** 12 (100%)
- **Cards Disconfirmed as "Already Solved":** 0 (0%)
- **Canonical Reference Projects Authored:** 24 total
  - **17 Canonical Islamic Solvers (`RP-001` through `RP-017`)**
  - **4 Adjacent-Domain Analogues (`ADJ-001` through `ADJ-004`)**
  - **3 Technical Benchmarks (`TECH-001` through `TECH-003`)**
- **Canonical Market Gaps Assigned:** 12 (`GAP-001` through `GAP-012`)
- **Market Disposition:** ALL 12 PROBLEMS APPROVED TO PROCEED TO PHASE 4 (AI OPPORTUNITY EVALUATION).

---

## 2. Comprehensive Master Competitor Matrix

The following matrix synthesizes the operational profile, technical architecture, strengths, and critical failure modes of all 24 reference projects evaluated during Phase 3:

| Ref ID | Project Name | Type / Platform | Target User | AI Stack | Key Capabilities & Strengths | Critical Failure Modes & Workflow Gaps | Evaluated Against |
|---|---|---|---|---|---|---|---|
| **RP-001** | **Dorar.net** (Al-Mawsu'ah al-Hadithiyyah) | Web & Mobile (Saudi Arabia) | Arabic researchers, scholars, imams | None (Deterministic Relational DB) | >2M narrations; comprehensive isnad gradings from classical & modern scholars; alternative chains (*turuq*). | Classical Arabic lockout; exact substring fragility; unmediated raw conflicting verdicts; no cross-lingual semantic search. | `P-001`, `P-200`, `P-300`, `P-302` |
| **RP-002** | **Sunnah.com** | Web Portal (Open Source) | English/Arabic readers, students | None (Elasticsearch Inverted Index) | Clean parallel bilingual view; indexes Six Books + Muwatta, Ahmad (partial); Darussalam/Albani grading tags. | Brittle substring search; missing secondary/tertiary collections; archaic translations cause semantic drift; no isnad trees. | `P-001`, `P-200`, `P-300`, `P-302` |
| **RP-003** | **HadeethEnc.com** | Web Portal & API (Saudi Arabia) | Multilingual learners, educators | None (Curated Editorial DB) | High-quality translations in 30+ languages; phrase-level vocabulary; contextual commentary and derived benefits. | Strictly capped at ~4,000 famous hadiths; 0% takhrij coverage for obscure, weak, or viral claims found in the wild. | `P-001`, `P-102`, `P-200`, `P-202` |
| **RP-004** | **Al-Maktabah al-Shāmilah** (shamela.ws) | Windows Desktop Suite & Web | Islamic scholars, university researchers | None (C++ / SQLite / PHP) | 8,000+ classical Arabic volumes; exact print pagination & volume numbers; comprehensive tafsir, fiqh, rijal. | Legacy desktop UI; exact-match boolean blindness; no cross-corpus isnad graph; siloed from modern translation/drafting tools. | `P-200`, `P-202`, `P-301`, `P-302` |
| **RP-005** | **Turath.io** (Nuqayah) | Web App & Turath AI | Modern Arabic researchers, devs | RAG / Hybrid (Turath AI) | Fast sub-second search over Shamela corpus; clean typography; open JS SDK; mobile responsive. | Arabic-only; Turath AI vulnerable to RAG hallucinations; lacks isnad tree graphs and multi-edition concordances. | `P-200`, `P-202`, `P-301`, `P-302` |
| **RP-006** | **AskSunnah & Hadith AI** (HadithGPT, Theo) | Web, Mobile & Prototypes | Digital Muslims, creators, scholars | OCR + Vector RAG / Multi-step LLM | Screenshot OCR extraction; natural language query; deep isnad checks (Theo). | Shallow Six Books indexing; high false-negatives; generative hallucination leakage; HadithGPT shut down for safety. | `P-001`, `P-200`, `P-300`, `P-302` |
| **RP-007** | **IslamQA.info** | Web & Mobile (16 Languages) | General Muslims searching Google | None (Taxonomy Search) | #1 global Google SEO; massive 100k+ question archive; extensive Qur'an and Hadith textual citations. | Monolithic Athari/Salafi strictness; erases 4 Madhahib; triggers clinical scrupulosity (*waswas*); convert alienation. | `P-002`, `P-101`, `P-301` |
| **RP-008** | **SeekersGuidance Answers** | Web Seminary (Canada/Global) | Traditional Sunni Muslims, converts | None (Algolia Search) | Scholar-reviewed Q&A tagged by madhhab (Hanafi, Shafi'i, Maliki); pastoral anti-waswas counseling; convert balance. | 4–12 week submission backlog; difficult search UX; single-school focus per answer without comparative columns. | `P-002`, `P-101`, `P-102`, `P-301` |
| **RP-009** | **IslamQA.org** | Web Aggregator | Traditional Sunni Muslims | None (Database Aggregator) | Aggregates 100k+ fatwas from accredited Darul Ulooms; madhhab filters; seminary attribution. | Uncurated collision of contradictory rulings; zero synthesis or *Usul* explanation; severe brand confusion with IslamQA.info. | `P-002`, `P-101`, `P-301` |
| **RP-010** | **Islamic Finance Guru** (IFG) | Web & Fintech Portal (UK) | Muslim professionals & investors | None (Editorial Fintech) | Exceptional comparative fatwa tables; breaks down opposing views, proofs, and practical consensus for modern finance. | Strictly limited to commercial finance/investments; high manual editorial cost; not extensible to general daily fiqh. | `P-002`, `P-301` |
| **RP-011** | **PrimaryIlm & Weekend Learning** | Physical Books & PDF Downloads | Madrasah teachers, homeschoolers | None (Print / PDF) | Standardized 10-level textbook series; 2,500+ printable coloring sheets and crafts for elementary children. | Static PDF/print trap; zero dynamic lesson scaffolding; unengaging rote textbook reading; no teen curriculum support. | `P-201` |
| **RP-012** | **Almaany & ejtaal.net** (Lane's Lexicon) | Web Dictionaries | Arabic students, translators | None (Digitized Lexicons) | Comprehensive root lookup in classical dictionaries (Lane, Wehr, Lisan al-Arab); free access. | ejtaal is static scanned bitmaps; Almaany is ad-cluttered with colloquial noise; isolated from CAT translation editors. | `P-102`, `P-202` |
| **RP-013** | **Yaqeen Institute & Tarbiyah** | Web Think-Tank & Curriculum | Western youth, educators, seekers | None (Academic Publishing) | High-quality long-form papers tackling intellectual doubts; visionary character development frameworks. | 20–40 page academic papers too dense for in-flow reading tooltips; lacks 40-min turnkey classroom lesson plans. | `P-101`, `P-102`, `P-201` |
| **RP-014** | **Quran.com** | Web & Mobile (Global Non-Profit) | Global Quran readers & students | None (Next.js / REST API) | World-class Uthmanic typography; 100+ translations; audio sync; manual "Pin & Compare" study drawer. | Strictly linear codex (Surah 1 to 114); "Pin & Compare" requires manual verse knowing; zero mutashabihat clustering. | `P-003`, `P-100`, `P-102` |
| **RP-015** | **Tarteel.ai** | Mobile App (US Venture) | Quran memorizers, reciters | Acoustic Speech Recognition (ASR) | Real-time voice tracking; hides text to test memory; flags verbal mistakes; inline mutashabihat color highlights. | Linear sequential recitation only; mutashabihat feature is inline color highlight without split-screen diffing or balaghah. | `P-003`, `P-100` |
| **RP-016** | **Aswaatul Qurraa & Ayaty** | Web & Android Apps | Hifdh students, Taraweeh imams | None (Static Lists) | Catalogs similar verses by Juz; printed margin references (*Mushaf al-Huffadh*). | Zero interactive word diffing; no synchronized audio comparison; no balaghah rationales; crude static lists. | `P-003` |
| **RP-017** | **Namaz App, Revertly & Pillars** | Mobile Applications | Converts, beginners, children | Audio/Visual UI (iSalati AI tracking) | 2D/3D posture guides; step-by-step audio; Revertly path-to-prayer lessons; Pillars privacy tracking. | Mandates full adult Arabic liturgy from Day 1; ignores Prophetic *Tadrij*; phone-on-floor disrupts prayer continuity. | `P-100` |
| **ADJ-001** | **Shepard's & KeyCite** | Legal Precedent Citators | Attorneys, legal scholars | Citation Graphs / Deterministic | Universal treatment signals (Red/Yellow/Green); tracks appellate overruling; cross-reporter concordance. | Proprietary legal domain; does not process religious isnads or Semitic texts. | `P-001`, `P-200`, `P-300`, `P-302` |
| **ADJ-002** | **UpToDate & DynaMed** | Clinical Decision Support | Physicians, medical trainees | Graded Evidence Syntheses | Executive summaries + detailed evidence; maps guideline conflicts; patient context gating; clinician oversight. | Healthcare-specific; requires human clinical panels. | `P-002`, `P-101`, `P-301` |
| **ADJ-003** | **Duolingo & Adaptive Learning** | EdTech Mobile Platforms | Language learners, beginners | Cognitive Scaffolding / Spaced Rep | Micro-unit chunking; zero-shame error tolerance; hands-free audio pacing; in-flow vocabulary tooltips. | General secular language focus; no ritual or worship modalities. | `P-100`, `P-102`, `P-201` |
| **ADJ-004** | **SDL Trados & Smartcat** | Enterprise CAT Platforms | Professional translators | Termbases & Translation Memories | Controlled termbases; "Do Not Translate" locks; concordance memory search; footnote/tag preservation. | Context-blind on classical Arabic; lacks tafsir and classical Islamic exegesis dictionaries. | `P-102`, `P-202` |
| **TECH-001** | **IslamicEval 2025** | ACL ArabicNLP Shared Task | AI researchers | Hallucination Detection Benchmark | Evaluates LLM hallucination and source retrieval in Islamic content. | Proves LLM retrieval precision is MAP@10 ~0.23 and correction failure rate is >31.8%. | `P-001`, `P-300`, `P-302` |
| **TECH-002** | **FiqhQA Benchmark** | AAAI/ACM AIES 2025 | AI researchers | Multi-Madhhab Reliability Benchmark | Evaluates LLM reliability, abstention, and madhhab accuracy on Kuwaiti Fiqh Encyclopedia. | Proves LLMs fail to abstain on 98%+ of ambiguous fiqh queries and systematically flatten madhahib. | `P-002`, `P-101`, `P-301` |
| **TECH-003** | **IslamicMMLU Benchmark** | arXiv:2603.23750 (2026) | AI researchers | 26-LLM Multi-Task Benchmark | Tests 12,000 questions (Hadith, Fiqh, Tafsir) across 26 models. | Proves accuracy dispersion (39.8% to 93.8%) and >38% cross-madhhab confusion on paired questions. | `P-001`, `P-300`, `P-301`, `P-302` |

---

## 3. Cluster-by-Cluster Workflow Coverage Breakdown

### 3.1 Cluster 1: Hadith Takhrij, Authentication & Provenance Verification
**Cards Evaluated:** `P-001` (Lay User Mobile Verification), `P-200` (Imam Khutbah Preparation), `P-300` (AI Hallucination & Phantom Attribution), `P-302` (Scholarly Cross-Corpus Fragmentation).

#### Current Workflow vs. Tool Coverage
```
[User encounters quote] ──> [Exact Keyword Search] ──> [Arabic Database Barrier] ──> [Conflicting Scholars] ──> [Manual Cross-Corpus Chase]
        │                             │                            │                         │                             │
    Trigger                    Sunnah.com (RP-002)          Dorar.net (RP-001)        Raw Rulings               Shamela (RP-004)
                              Fails on paraphrase          Classical Arabic only     No consensus synthesis    Desktop silo / 45-90 min
```

#### Detailed Coverage Breakdown:
1. **Query Initiation:** Sunnah.com (`RP-002`) and Google provide basic keyword lookup, but fail immediately when a query uses modern colloquial synonyms or paraphrases. AskSunnah (`RP-006`) provides mobile OCR screenshot lookup, but only covers the Six Books, generating false negatives on any secondary text.
2. **Authentication & Takhrij:** Dorar.net (`RP-001`) offers exhaustive authentication (>2M hadiths), but requires classical Arabic fluency. Furthermore, Dorar lists raw scholar rulings (e.g. Al-Tirmidhi vs Ibn Hajar vs Al-Albani) without a meta-synthesis explaining the divergence, leaving lay users and busy khatibs paralyzed.
3. **Deep Commentary & Sabab al-Wurud:** Maktabah Shamela (`RP-004`) and Turath.io (`RP-005`) contain the full-text classical commentaries (*Fath al-Bari*, *Sharh Sahih Muslim*), but operate as isolated reading silos. An imam preparing a khutbah (`P-200`) spends 2–4 hours manually copying texts and cross-checking isnads across multiple open browser windows.
4. **AI Generation Guardrails:** In conversational AI tools (`P-300`), the lack of external deterministic constraints leads models to fabricate citations ("Sahih al-Bukhari #4821"). Benchmarks (`TECH-001`, `TECH-003`) confirm that vector-based RAG achieves an abysmal MAP@10 of ~0.23, proving that statistical embeddings cannot reliably locate canonical hadith passages.

*Cluster Conclusion:* **CRITICAL WORKFLOW GAPS REMAIN UNSOLVED.** Assigned `GAP-001`, `GAP-007`, `GAP-010`, and `GAP-012`.

---

### 3.2 Cluster 2: Conflicting Fatwas, Ikhtilaf & Jurisprudential Context
**Cards Evaluated:** `P-002` (Lay Search Paralysis & Scrupulosity), `P-101` (Convert Fatwa Whiplash & Family Rupture), `P-301` (Algorithmic Fiqh Context-Flattening & Unqualified Fatwas).

#### Current Workflow vs. Tool Coverage
```
[Practical Dilemma] ──> [Google Search / Prompt] ──> [SEO Monolith Collision] ──> [Sectarian Whiplash] ──> [Scrupulosity / Family Rupture]
        │                         │                             │                          │                              │
    Trigger                    Google / ChatGPT              IslamQA.info (RP-007)      Opposing Seminaries        Severe Religious OCD
                              Uncontextualized query        #1 SEO / Hanbali strict    IslamQA.org (RP-009)       Apostasy Risk / Guilt
```

#### Detailed Coverage Breakdown:
1. **Search Discovery:** Google search for any practical lifestyle or worship question is overwhelmingly dominated by IslamQA.info (`RP-007`). Its rulings enforce a monolithic Athari/Salafi legal methodology, reject the validity of alternative classical madhahib, and default to the strictest prohibition.
2. **User Impact:** For working professionals (`P-002`), browsing IslamQA frequently triggers clinical religious scrupulosity (Scrupulosity OCD / *al-waswas al-qahri*; `E01-003`). For first-year converts (`P-101`), discovering that celebrating Thanksgiving or attending non-Muslim family dinners is declared "grave sin" causes acute familial rupture, trauma, and a 20–30% apostasy vulnerability (`E02-003`, `E02-004`).
3. **Alternative Portals:** SeekersGuidance (`RP-008`) provides balanced traditional rulings and pastoral anti-waswas guidance, but suffers from low search visibility and a 4–12 week submission backlog. IslamQA.org (`RP-009`) aggregates traditional seminary links, but presents an uncurated brawl of conflicting opinions without *Usul* explanation. Islamic Finance Guru (`RP-010`) provides the ideal comparative synthesis table, but is strictly restricted to commercial investments.
4. **Conversational AI Failure:** LLMs (`P-301`) flatten jurisprudence into flat universal statements ("Islam says X"), silently imposing one scraped school while failing to ask clarifying questions about personal circumstance. As proven by the FiqhQA benchmark (`TECH-002`), models fail to abstain on 98%+ of ambiguous legal queries, violating the sacred governance rule (`[NO AUTONOMOUS FATWA PERMITTED]`).

*Cluster Conclusion:* **CRITICAL WORKFLOW GAPS REMAIN UNSOLVED.** Assigned `GAP-002`, `GAP-005`, and `GAP-011`.

---

### 3.3 Cluster 3: Sacred Terminology, Localization & Curriculum Pedagogy
**Cards Evaluated:** `P-102` (Convert Jargon Barrier & Cultural Conflation), `P-201` (Madrasah Volunteer Lesson Adaptation), `P-202` (Semantic Drift & Citation Severance in Localization).

#### Detailed Coverage Breakdown:
1. **Learner-Side Reading Assistance (`P-102`):** Non-Arabic readers encountering Islamic texts must constantly interrupt their reading flow to Google loanwords (*Wudu*, *Ghusl*, *Taharah*, *Fard*). Existing tools (Islamicity Glossary, ejtaal) are static web pages or scanned dictionaries. Furthermore, standard tools fail to disambiguate universal divine law (*Shari'ah*) from immigrant cultural customs (*'Urf*), causing converts to feel alienated as "cultural imposters" (`E02-003`).
2. **Weekend Madrasah Classroom Assembly (`P-201`):** Over 80% of weekend madrasah teachers are unpaid volunteers (`E03-003`). Existing curriculum providers (Weekend Learning Publishers, PrimaryIlm; `RP-011`) trap teachers between dry textbooks and fragmented printable PDFs. No tool generates a modular, 40-minute lesson plan with age-appropriate hooks, discussion prompts, and vetted activities, forcing teachers into 3–5 hours of late-night Saturday web scraping (`E03-004`) and driving 40–60% annual volunteer turnover.
3. **Professional Translation & Localization (`P-202`):** Off-the-shelf CAT tools (SDL Trados Studio, memoQ; `ADJ-004`) and neural machine translation engines (DeepL, Google Translate) suffer from severe "computational flattening" on classical Arabic religious texts (`E03-005`). They translate multidimensional theological polysemes into secular equivalents (*Taqwa* $\rightarrow$ "fear", *Ijtihad* $\rightarrow$ "independent thinking") and sever classical bibliographic citations, forcing translators to spend hours manually consulting scanned dictionaries on ejtaal (`RP-012`).

*Cluster Conclusion:* **CRITICAL WORKFLOW GAPS REMAIN UNSOLVED.** Assigned `GAP-006`, `GAP-008`, and `GAP-009`.

---

### 3.4 Cluster 4: Specialized Standalone Ritual Workflows
**Cards Evaluated:** `P-003` (Quran Mutashabihat al-Lafz Navigation), `P-100` (Convert Solitary Salah Learning Overload).

#### Detailed Coverage Breakdown:
1. **Mutashabihat al-Lafz Disambiguation (`P-003`):** Quran memorizers (Huffadh) regularly suffer recitation memory lapses during congregational prayers (e.g. Taraweeh) due to verbal similarities across distant Surahs (`E01-006`). Leading platforms like Quran.com (`RP-014`) and Tarteel.ai (`RP-015`) are architected strictly as linear codices. Tarteel highlights similar words inline on the page, but offers no split-screen comparative view, no syntactic diffing, and no rhetorical (*Balaghah*) explanations. Memorizers are forced into crude manual workarounds, including pasting screenshots into GoodNotes (`E01-005`) or penciling notes in Mushaf margins.
2. **Convert Solitary Salah Learning (`P-100`):** Adult converts in their first 90 days face multi-modal cognitive overload attempting to synchronize 17 physical postures, unfamiliar Arabic recitations, and sequence rules. Existing mobile apps (Namaz App, Step by Step Salat; `RP-017`) completely omit the classical Prophetic pedagogical concession of gradualism (*Tadrij*; *Sunan Abi Dawud 858*; `E02-002`), which permits beginners to recite simple Tasbeeh while learning movements. Instead, apps mandate full adult Arabic liturgy from Day 1 and require touchscreen tapping mid-prayer, forcing converts to place paper cheat sheets on the floor (`E02-001`) and inducing acute spiritual guilt.

*Cluster Conclusion:* **CRITICAL WORKFLOW GAPS REMAIN UNSOLVED.** Assigned `GAP-003` and `GAP-004`.

---

## 4. Canonical Gap Register (GAP-001 through GAP-012)

The following register formally establishes the twelve (12) canonical Market and Workflow Gaps identified, validated, and linked to the Level 3 Problem Cards:

| Gap ID | Linked Card | Canonical Gap Title | Exact Unresolved Workflow Friction Statement | Evidence Confidence | Market Disposition |
|---|---|---|---|---|---|
| **GAP-001** | `P-001` | Bilingual Semantic Takhrij & Scholar Consensus Bridge | Inability of non-Arabic speaking Muslims to take an English, transliterated, paraphrased, or non-canonical hadith quote from social media and resolve it to authentic primary Arabic hadith collections with verified multi-scholar consensus gradings in under 30 seconds. | High (`E01-001`, `E01-002`, `TECH-001`) | **PROCEED TO AI EVALUATION** |
| **GAP-002** | `P-002` | Structured Comparative Ikhtilaf & Usul Attribution Engine | Absence of an objective, non-judgmental comparative fiqh interface that structures rulings across the 4 Sunni Madhahib, distinguishes immutable consensus (*Ijma'*) from legitimate disagreement (*Ikhtilaf*), and explains legal rationale (*Sabab al-Ikhtilaf*) for modern lifestyle dilemmas without triggering religious scrupulosity (*waswas*). | High (`E01-003`, `E01-004`, `TECH-002`) | **PROCEED TO AI EVALUATION** |
| **GAP-003** | `P-003` | Non-Linear Mutashabihat Visual Diffing & Rhetorical Memory Graph | Lack of a non-linear comparative Quran study and active-recall interface that automatically clusters verbally similar verses (*Mutashabihat al-Lafz*) across disparate Surahs, highlights word-level variations with automated visual diffing, provides comparative audio playback, and contextualizes differences using classical *Balaghah*. | High (`E01-005`, `E01-006`) | **PROCEED TO AI EVALUATION** |
| **GAP-004** | `P-100` | Embodied Prophetic Gradualism (*Tadrij*) & Hands-Free Salah Coach | Total absence of a hands-free, motion-adaptive ritual prayer learning coach that implements the authentic Prophetic pedagogical concession of gradualism (*Tadrij*; Sunan Abi Dawud 858), forcing isolated converts into multi-sensory cognitive overload, motor desynchronization, and paper-on-the-floor cheat sheet workarounds. | High (`E02-001`, `E02-002`) | **PROCEED TO AI EVALUATION** |
| **GAP-005** | `P-101` | Convert Minority-Fiqh Navigator & Familial Dilemma Guardrail | Lack of a context-aware legal guidance framework tailored for newly converted Muslims navigating high-stakes non-Muslim family dilemmas (holidays, funerals, shared meals) that builds foundational *Ikhtilaf* literacy, directly preventing the family rupture and apostasy vulnerability caused by unmediated internet search results. | High (`E02-003`, `E02-004`) | **PROCEED TO AI EVALUATION** |
| **GAP-006** | `P-102` | In-Flow Progressive Terminology Lexicon & Cultural Deconflation Scaffolder | Lack of an in-flow, progressive reading assistant that provides tiered micro-definitions for sacred Arabic loanwords and actively disambiguates universal Shari'ah obligations from local ethnic cultural customs (*'Urf*), eliminating reading interruption and cultural alienation. | High (`E02-003`, `E02-006`) | **PROCEED TO AI EVALUATION** |
| **GAP-007** | `P-200` | Khatib Khutbah Workbench with Unified Takhrij & Sabab al-Wurud Synthesis | Absence of a unified bilingual khutbah preparation workbench for community imams that couples rapid thematic search with automated takhrij—synthesizing conflicting classical gradings and retrieving historical context (*Sabab al-Wurud*)—compressing 3+ hours of manual tab-juggling while preventing the pulpit dissemination of weak hadiths. | High (`E03-001`, `E03-002`) | **PROCEED TO AI EVALUATION** |
| **GAP-008** | `P-201` | Modular Time-Budgeted Madrasah Instructional Scaffolder | Lack of a time-budgeted, modular lesson scaffolding engine that translates abstract Islamic curricula into turnkey, pedagogically sequenced 40-minute classroom instructional flows (Hook $\rightarrow$ Story $\rightarrow$ Interactive Activity $\rightarrow$ Comprehension Check) with scholar-audited orthodox citations, eliminating volunteer burnout and high teacher turnover. | High (`E03-003`, `E03-004`) | **PROCEED TO AI EVALUATION** |
| **GAP-009** | `P-202` | Sacred Exegetical Localization Workbench with Citation Preservation | Absence of a domain-specific localization workbench that embeds classical Arabic lexicons (*Lisan al-Arab*) and Tafsir directly into the text editor, suggesting scholar-vetted equivalents for theological polysemes while safeguarding classical citation metadata and eliminating neural machine translation computational flattening. | High (`E03-005`, `E03-006`, `E03-007`) | **PROCEED TO AI EVALUATION** |
| **GAP-010** | `P-300` | Primary-Source Cryptographic Hadith Grounding Barrier | Total lack of a deterministic, token-constrained verification barrier between generative AI systems and public discourse that enforces exact matching against immutable primary Arabic hadith collections, permanently eliminating "phantom attributions" and synthetic sacred speech. | High (`E04-001`, `E04-003`, `TECH-001`) | **PROCEED TO AI EVALUATION** |
| **GAP-011** | `P-301` | Context-Gated Madhhab-Calibrated Fiqh Retrieval Guardrail | Failure of conversational AI systems to gather situational constraints, accurately represent differences across the four Sunni Madhahib, and strictly abstain from issuing autonomous, unqualified religious edicts (*Fatwas*) on personal status matters (`[NO AUTONOMOUS FATWA PERMITTED]`). | High (`E04-002`, `E04-005`, `E04-006`, `TECH-002`) | **PROCEED TO AI EVALUATION** |
| **GAP-012** | `P-302` | Unified Cross-Corpus Islamic Provenance Graph & Concordance Engine | Complete architectural fragmentation separating desktop classical Arabic text suites (Maktabah Shamela), online authentication databases (Dorar.net), and bilingual collections (Sunnah.com), lacking cross-edition pagination concordance and isnad transmission graph harmonization. | High (`E04-007`, `E04-001`, `ADJ-001`) | **PROCEED TO AI EVALUATION** |

---

## 5. Disconfirmed & "Already-Solved" Problems Audit

In compliance with Principle 7 (Disconfirmation & Falsification Discipline) of `AGENTS.md`, Agent 05 actively tested whether any of the 12 candidate problems were already adequately solved by existing commercial software, open-source repositories, or non-AI tools.

### 5.1 What IS Already Solved (Out of Scope for Innovation)
Our market audit definitively identified several workflow areas that are **already solved** and must **NOT** be targeted by downstream AI teams:
1. **Reading the Canonical Qur'an with Translations and Audio:** *Quran.com* (`RP-014`) completely solves linear Quranic recitation, high-resolution Uthmanic font rendering, synchronized word-level audio playback, and multi-translation browsing. Re-building a general Quran reader has zero marginal value.
2. **Linear Memorization Recitation Tracking:** *Tarteel.ai* (`RP-015`) has mastered real-time acoustic speech recognition for sequential recitation, word-hiding, and vocal mistake flagging. Competing with Tarteel on linear recitation tracking is redundant.
3. **Keyword Lookup for the Top 500 Most Famous Hadiths:** For universally known hadiths (e.g. 40 Hadith Nawawi, Bukhari Book of Faith/Prayer), Sunnah.com (`RP-002`) and Google search work reliably. Innovation is only needed for paraphrased, obscure, non-canonical, or cross-corpus takhrij.
4. **Clear-Cut Consensus Fiqh Queries:** For universally established legal obligations (*Ma'lum min al-din bid-darurah*; e.g., prohibition of alcohol, five daily prayers, fasting Ramadan), existing search portals (Islamweb, IslamQA) provide clear answers without paralysis. Innovation is strictly justified for multi-school *Ikhtilaf* and contemporary dilemmas.
5. **Basic Prayer Times and Qibla Compass:** Applications like *Pillars* and *Athan* have perfected ad-free, privacy-preserving prayer schedules.

### 5.2 Why All 12 Problem Cards Survived Falsification
Despite the maturity of tools in adjacent areas, each of the 12 Problem Cards survived aggressive attempts to disprove its underlying pain point:
- `P-001`, `P-200`, `P-300`, `P-302` survive because **no tool bridges the language barrier between English queries and Arabic takhrij engines**, and **no tool unifies siloed classical text databases with isnad graphs**.
- `P-002`, `P-101`, `P-301` survive because **the internet's fatwa architecture remains dogmatically polarized**, actively harming convert retention and triggering documented clinical OCD.
- `P-102`, `P-201`, `P-202` survive because **general translation and educational software fail on sacred Arabic polysemy and time-budgeted madrasah classroom constraints**.
- `P-003` and `P-100` survive because **digital Quran apps remain trapped in linear book layouts**, and **prayer apps refuse to implement Prophetic gradualism (*Tadrij*)**.

---

## 6. Adjacent-Domain Architectural Insights

High-trust industries outside the Islamic domain have already engineered robust, battle-tested architectural mechanisms to solve structurally identical information retrieval and decision-support problems. Agent 05 recommends transferring four (4) core architectural patterns to downstream teams:

```
           ADJACENT DOMAIN                                      ISLAMIC DOMAIN APPLICATION
┌──────────────────────────────────────┐               ┌──────────────────────────────────────────┐
│  LEGAL CITATORS (Shepard's / KeyCite)│  ───────────> │  Hadith Isnad & Takhrij Graph            │
│  • Direct appellate history          │               │  • Continuous vs Broken chains (Inqita') │
│  • Negative treatment warning flags  │               │  • Scholarly consensus status badges     │
│  • Cross-reporter page concordance   │               │  • Cross-edition manuscript concordance  │
└──────────────────────────────────────┘               └──────────────────────────────────────────┘

┌──────────────────────────────────────┐               ┌──────────────────────────────────────────┐
│  CLINICAL DECISION SUPPORT (UpToDate)│  ───────────> │  Comparative Fiqh & Ikhtilaf Synthesizer │
│  • Executive summary + deep evidence │               │  • Consensus summary + 4-Madhhab columns │
│  • Guideline conflict reconciliation │               │  • Usul rationale (Sabab al-Ikhtilaf)    │
│  • Context-gating & contraindications│               │  • Context-intake & non-autonomous mufti │
└──────────────────────────────────────┘               └──────────────────────────────────────────┘

┌──────────────────────────────────────┐               ┌──────────────────────────────────────────┐
│  ADAPTIVE EDTECH (Duolingo / Mastery)│  ───────────> │  Convert Ritual Pedagogy (Tadrij)        │
│  • Micro-unit chunking               │               │  • 4-tier Prophetic gradualism in Salah  │
│  • In-flow tiered vocabulary tooltips│               │  • In-flow loanword cultural tooltips    │
│  • Hands-free audio pacing           │               │  • Motion-paced audio prayer coaching    │
└──────────────────────────────────────┘               └──────────────────────────────────────────┘

┌──────────────────────────────────────┐               ┌──────────────────────────────────────────┐
│  ENTERPRISE CAT (Trados / Smartcat)  │  ───────────> │  Sacred Text Exegetical Localization     │
│  • Controlled domain termbases       │               │  • In-editor Lisan al-Arab / Tafsir      │
│  • "Do Not Translate" locks          │               │  • Polysemy preservation (Taqwa, Bid'ah) │
│  • Immutable footnote tag integrity  │               │  • Classical citation & isnad links      │
└──────────────────────────────────────┘               └──────────────────────────────────────────┘
```

---

## 7. Strategic Handoff to Agent 06 (AI Opportunity Researcher)

As Phase 3 concludes, the research corpus is formally transferred to **Agent 06 (AI Opportunity Researcher)** to author Section 24 across all 12 cards and establish where AI genuinely earns its place against the strongest non-AI baselines.

### 7.1 Direct Directives for Agent 06:
1. **Force AI to Earn Its Place Against Strong Non-AI Baselines:**
   - In `P-003` (Mutashabihat), can relational graph databases and Levenshtein string diffing solve 90% of verse clustering without needing a heavy LLM? What specific role does AI play (e.g. semantic embeddings for thematic matching vs deterministic n-gram matching)?
   - In `P-302` (Takhrij Chasm), does the solution require generative AI, or is it fundamentally a deterministic citation knowledge graph (like Shepard's)?
2. **Evaluate Multimodal Acoustic / Computer Vision Leverage:**
   - In `P-100` (Salah Learning), evaluate on-device pose estimation (e.g. MediaPipe / CoreML) and voice activity detection (VAD) for hands-free, motion-paced prayer guidance without requiring smartphones on the floor.
   - In `P-001`, evaluate cross-lingual semantic embeddings that map noisy English colloquial queries directly into canonical classical Arabic matn vector spaces.
3. **Enforce Deterministic Grounding & Abstention Architectures:**
   - In `P-300` (Hadith Hallucination), design a verification barrier that enforces exact token-level matching against canonical corpora before text generation occurs.
   - In `P-301` (Fiqh Context-Flattening), benchmark context-gating decision trees that force conversational models to abstain on personal status queries and structure responses into parallel Madhhab columns.

---
*End of Master Landscape Report — CYCLE-001.*
