# Synthesis Register: Unflattened Disagreements & Minority Viewpoints
## Islamic AI Challenge Research Lab — Phase 6 Cross-Examination Synthesis
### Governed by `AGENTS.md` Rule 9 ("Evidence Over Consensus") and `cross-examination-protocol.md` Section 61

---

- **Document ID:** SYN-DISAGREE-01
- **Cycle:** CYCLE-001
- **Phase:** PHASE 6 — CROSS-EXAMINATION
- **Governing Agent:** Agent 08 — Research Director (Moderator & Custodian of Council Dissent)
- **Status:** AUTHORITATIVE & UNFLATTENED
- **Date Updated:** 2026-09-17

---

## 1. Constitutional Preamble
In accordance with Rule 9 of the Supreme Global Constitution (`AGENTS.md`):
> *"Agreement is valuable only when independently grounded in evidence. Do not force artificial consensus where legitimate scholarly or technical differences remain. Preserve legitimate disagreements in `synthesis/disagreements.md`."*

The council recognizes that forcing premature or artificial consensus in sacred knowledge domains results in brittle products, hidden failure modes, and theological distortion. The four disagreements recorded below represent substantive, evidence-grounded divergences between specialist council members that survived Phase 6 Cross-Examination without resolution. They must be carried forward visibly into Phase 7 (Opportunity Mapping) and Phase 8 (Hackathon Prioritization).

---

## 2. Register of Unflattened Disagreements

---

### DISAGREEMENT ID: DISAGREE-001
- **Target Problem & AI Opportunity:** `P-003` (Quran Mutashabihat Navigation) | `AI-OP-003`
- **Contested Question:** 
  > *Does on-device acoustic speech recognition (ASR) provide meaningful pedagogical utility for active-recall Quranic recitation testing, or do acoustic error rates on subtle Tajweed rules make speech tracking an unworkable net-negative for memorizers?*

#### Position A: Bounded ASR Provides Real Active-Recall Leverage
- **Primary Proponents:** Agent 06 (AI Architect), supported by Agent 01 (Muslim User Researcher)
- **Core Rationale & Evidence:**
  - When testing active recall between distant verbal twins (e.g. Al-Baqarah 2:48 vs 2:123), the speech model is not performing unconstrained transcription; it is performing **constrained phoneme alignment against a known reference text**.
  - Open models (e.g., Wav2Vec2-Quran, Whisper fine-tuned on Qira'at) can reliably detect word-level token substitutions (*tatawwu'an* vs *tatawwa'a*).
  - Enables hands-free recitation review while standing or pacing in solitary prayer revision, freeing the memorizer from tapping phone screens or holding tablets.
- **Evidence Cited:** Benchmark alignments on Quranic audio corpora (`AI-OP-003`); field user reports of recitation confusion during Ramadan Taraweeh (`E01-004`).

#### Position B: Tajweed Acoustic Sensitivity Renders ASR a Frustrating Gimmick
- **Primary Proponent:** Agent 07 (Red Team & Skeptic)
- **Core Rationale & Evidence:**
  - Quranic recitation is governed by sacred phonetic rules (*Ahkam al-Tajweed*): nasalization (*ghunnah*), concealment (*ikhfa*), bouncing consonants (*qalqalah*), elongation (*madd*), and canonical variant readings (*Qira'at*).
  - Across diverse non-Arab reciting populations (South Asian, West African, Southeast Asian, Western converts), acoustic models exhibit high false-error rates, flagging correct recitations as errors due to regional accents.
  - In a sacred act of worship, an algorithmic false alarm breaks spiritual focus (*Khushu'*) and induces anger. Huffadh prefer self-testing against synchronized human audio playback or human recitation partners (*Muraja'ah*).
- **Evidence Cited:** Red Team Adversarial Audit `RT-P-003`; high word error rates of commercial speech engines on non-native Arabic.

#### Why It Remains Unresolved:
The council lacks empirical field trial data measuring the exact Phoneme Error Rate (PER) of on-device models across diverse reciter accents on specific mutashabihat pairs. The Director ruled that the core diff engine must be 100% deterministic, while ASR is retained strictly as an optional experimental secondary feature pending empirical testing (`OQ-002`).

---

### DISAGREEMENT ID: DISAGREE-002
- **Target Problem & AI Opportunity:** `P-101` (Convert Fatwa Whiplash) | `AI-OP-005`
- **Contested Question:**
  > *Should a digital convert guidance tool actively promote minority jurisprudential dispensations (Fiqh al-Aqaliyyat, e.g., attending non-Muslim family Thanksgiving meals or church funerals), or does arming converts with minority rulings trigger severe social ostracization from conservative local diaspora mosques?*

#### Position A: Minority Fiqh Dispensations Are Essential for Convert Preservation
- **Primary Proponents:** Agent 02 (New Muslim Researcher), supported by Agent 06 (AI Architect)
- **Core Rationale & Evidence:**
  - Mainstream internet search is dominated by rigid, uncontextualized edicts (IslamQA.info) telling converts it is haram to attend their mother's funeral or sit at a family Thanksgiving table where turkey is served.
  - This rigidity is directly responsible for acute family rupture, psychological trauma, and a documented **20% to 30% apostasy/disillusionment rate within 3 years of conversion** (`E02-003`, `E02-004`).
  - Authoritative minority jurisprudence councils (European Council for Fatwa and Research, Fiqh Council of North America, SeekersGuidance) have issued validated concessions (*Rukhas*) prioritizing filial piety (*Birr al-Walidayn*) and gradualism (*Taysir*). Providing these rulings is an existential pastoral duty.
- **Evidence Cited:** Academic convert retention studies (Pew 2017, Cambridge convert surveys); institutional fatwas from ECFR and FCNA.

#### Position B: Minority Rulings Provoke Destructive In-Group Mosque Alienation
- **Primary Proponent:** Agent 07 (Red Team & Skeptic)
- **Core Rationale & Evidence:**
  - The lived reality of Western diaspora mosques is dominated by conservative immigrant communities and imams who reject *Fiqh al-Aqaliyyat* as an illegitimate modernist compromise of the Shari'ah.
  - A vulnerable new convert who attends a church funeral or family holiday and cites an app's minority ruling will be aggressively censured, corrected, or socially shunned by their new mosque peers.
  - This merely transfers alienation from the biological family to the spiritual community, leaving the convert in total social isolation. Automated tools should not encourage positions that local religious leaders consider compromised without direct pastoral accompaniment.
- **Evidence Cited:** Red Team Adversarial Audit `RT-P-101`; sociological field observations of diaspora convert policing.

#### Why It Remains Unresolved:
This dispute reflects an authentic, ongoing theological and sociological tension within contemporary Western Islam between academic minority jurisprudence (*Fiqh al-Nawazil*) and grassroots communal traditionalism. The Director ruled that minority rulings must never be displayed in isolation, but must include communication guidance ("How to speak with your local Imam") and immediate escalation to human convert mentors.

---

### DISAGREEMENT ID: DISAGREE-003
- **Target Problem & AI Opportunity:** `P-300` (Hadith Hallucination & Phantom Attribution) | `AI-OP-010`
- **Contested Question:**
  > *Can Natural Language Inference (NLI) cross-encoders reliably detect span-level text corruptions in classical Arabic hadith texts, or does the linguistic nature of classical Arabic impose an accuracy ceiling that creates a dangerous false sense of security?*

#### Position A: NLI Alignment Provides Critical Linguistic Grounding Beyond Regex
- **Primary Proponents:** Agent 06 (AI Architect), supported by Agent 04 (Islamic Trust Researcher)
- **Core Rationale & Evidence:**
  - Non-AI regex primary-key checking only works when an explicit numerical citation (e.g. `[Bukhari #4821]`) is present. It is completely blind when an LLM quotes unnumbered text ("The Prophet said: ...") or subtly alters 2–3 words in an authentic narration (*span corruption*).
  - Fine-tuned cross-encoder NLI models trained on Islamic corpora can distinguish between legitimate paraphrasing and theological corruption, providing an essential secondary line of defense against synthetic sacred speech.
- **Evidence Cited:** Architectural benchmarks in `AI-OP-010`; span-level corruption detection baselines in `TECH-001` (IslamicEval 2025).

#### Position B: 68% NLI Accuracy is Lethally Insufficient for Sacred Speech
- **Primary Proponent:** Agent 07 (Red Team & Skeptic)
- **Core Rationale & Evidence:**
  - In `TECH-001` (IslamicEval 2025), state-of-the-art cross-encoder systems hit an accuracy ceiling of only **68.18%** on detecting span-level hadith corruptions in classical Arabic.
  - Classical Arabic text features complex morphology, case inflections (*I'rab*), and manuscript variants (*Riwayat*) where a single vowel change can reverse theological meaning.
  - An NLI classifier operating at ~68% accuracy will assign false-positive "Entailment" badges to subtly corrupted hadiths, giving content creators and publishers a dangerous, rubber-stamped false guarantee of prophetic authenticity. Sacred text demands 100% mathematical precision, not probabilistic guesses.
- **Evidence Cited:** IslamicEval 2025 shared task evaluation results (`TECH-001`); classical hadith textual transmission standards (`source-policy.md`).

#### Why It Remains Unresolved:
Whether fine-tuning on larger domain-specific datasets can raise classical Arabic NLI precision from 68% to >90% without catastrophic false positives remains an unproven empirical hypothesis. The Director ruled that NLI cannot grant absolute authenticity badges, acting strictly as an internal advisory anomaly linter.

---

### DISAGREEMENT ID: DISAGREE-004
- **Target Problem & AI Opportunity:** `P-202` (Theological Terminology Drift in Localization) | `AI-OP-009`
- **Contested Question:**
  > *Does developing specialized translation tooling for classical Arabic-to-English religious translation justify technical effort, given the microscopic global user base (300–500 translators) and rigid workflow lock-in to Microsoft Word?*

#### Position A: Sacred Polysemy Preservation Justifies Vertical Tooling
- **Primary Proponents:** Agent 03 (Educator & Translator Researcher), supported by Agent 06 (AI Architect)
- **Core Rationale & Evidence:**
  - General machine translation engines (Google, DeepL) cause catastrophic "computational flattening" of core theological polysemes (*Taqwa* $\rightarrow$ "fear", *Ijtihad* $\rightarrow$ "independent thinking", *Bid'ah* $\rightarrow$ "innovation").
  - An exegetical copilot and termbase recommender that integrates classical lexicons (*Lisan al-Arab*, *Lane's Lexicon*) and preserves isnad footnote tags protects the epistemic integrity of sacred literature in the English language.
  - Word/Trados plugins directly meet translators inside their existing workflows, eliminating tab-juggling across 6 dictionaries.
- **Evidence Cited:** Corpus linguistics analysis of English Islamic publishing (`E03-005`); translator productivity benchmarks (`AI-OP-009`).

#### Position B: Enterprise Workflow Lock-in and Micro-TAM Guarantee Commercial Abandonment
- **Primary Proponent:** Agent 07 (Red Team & Skeptic), supported by Agent 05 (Market Landscape Researcher)
- **Core Rationale & Evidence:**
  - The total global pool of active classical Arabic-to-English Islamic book translators is microscopically small (300–500 individuals worldwide). Developing, testing, and maintaining vertical software for this niche is commercially unsustainable.
  - Major publishing houses (Darussalam, IIIT, Turath) enforce rigid in-house style guides. A static, deterministic CAT Termbase (TBX format) with locked regex rules solves 90% of consistency problems with zero AI inference cost and zero latency.
  - Translators will not adopt third-party plugins that disrupt established typesetting and macro pipelines.
- **Evidence Cited:** Publishing industry workflow audits (`RT-P-202`); software commercial viability criteria (`AGENTS.md` Sec 8).

#### Why It Remains Unresolved:
Whether Islamic academic institutions or non-profit publishing endowments will subsidize the development of an open-source Word/Trados translation add-in remains an open funding and adoption question. The Director ruled that standalone web CAT suites are permanently abandoned, preserving only an embeddable Word add-in scope.

---

## 3. Governance Audit & Next Steps
All four disagreements have been recorded without flattening or forced consensus. They will serve as explicit risk and sensitivity parameters during Phase 7 Opportunity Mapping and Phase 8 Prioritization.

*Signed,*  
**Agent 08 — Research Director**  
*Islamic AI Challenge Research Lab — CYCLE-001*
