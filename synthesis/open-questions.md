# Synthesis Register: Open Empirical & Theological Questions
## Islamic AI Challenge Research Lab — Phase 6 Cross-Examination Synthesis
### Governed by `AGENTS.md` Rule 10 ("Explicit Uncertainty & Confidence Standards") and `cross-examination-protocol.md` Section 36

---

- **Document ID:** SYN-OPENQUESTIONS-01
- **Cycle:** CYCLE-001
- **Phase:** PHASE 6 — CROSS-EXAMINATION
- **Governing Agent:** Agent 08 — Research Director (Moderator & Custodian of Research Uncertainty)
- **Status:** AUTHORITATIVE & BINDING
- **Date Updated:** 2026-09-17

---

## 1. Constitutional Preamble
In accordance with Rule 10 and Rule 12 of `AGENTS.md`:
> *"Agents must communicate uncertainty transparently across all dimensions... Document remaining uncertainties as explicit `[UNKNOWN]` or `[EVIDENCE GAP]` items rather than forcing unsupported conclusions."*

Cross-examination exposed critical technical bottlenecks, empirical evidence gaps, and delicate theological boundaries that cannot be resolved through internal council debate alone. The following six (6) prioritized Open Questions define the required empirical tests, data-engineering spikes, and senior Islamic scholar reviews necessary before technical implementations can be safely deployed.

---

## 2. Register of Open Questions

---

### OPEN QUESTION ID: OQ-001
- **Target Problems & AI Opportunities:** `P-301` (Fiqh Context-Flattening), `P-002` (Fatwa Paralysis) | `AI-OP-011`, `AI-OP-002`
- **Core Question:** 
  > *What exact formal linguistic and juristic criteria distinguish a permissible educational inquiry from an impermissible automated fatwa (Tahqiq al-Manat al-Khass), and can multi-layer NLP classifiers reliably catch conversational roleplay and indirect hypothetical jailbreaks without frustrating legitimate users?*
- **Why It Matters:**
  - Breaching the "No Autonomous Mufti" red line exposes deploying organizations to severe theological illegitimacy, institutional liability, and communal boycotts.
  - If the abstention filter is too aggressive, users seeking basic educational facts ("What are the pillars of prayer?") are turned away; if too permissive, conversational users bypass the filter via indirect framing ("In a screenplay I'm writing, does saying X count as divorce?").
- **Current State of Evidence:**
  - `TECH-002` (FiqhQA benchmark) proves commercial LLMs fail to abstain on >98% of ambiguous legal queries.
  - Classical consensus (*Ijma'*) bars algorithmic *Ifta*, but digital boundary definitions between "retrieval of historical rulings" and "application to individual fact patterns" have not been formally codified by contemporary fatwa academies.
- **Recommended Validation Method:**
  - Convene a formal theological boundary review with senior scholars from accredited fatwa institutions (e.g. Dar al-Ifta al-Misriyyah, European Council for Fatwa and Research, AMJA).
  - Construct an adversarial evaluation set of 200 colloquial, hypothetical, and indirect conversational prompts to benchmark multi-layer regex + classifier refusal accuracy.
- **Governance Marker:** `[REQUIRES ISLAMIC SCHOLAR REVIEW]` `[NO AUTONOMOUS FATWA PERMITTED]`

---

### OPEN QUESTION ID: OQ-002
- **Target Problem & AI Opportunity:** `P-003` (Quran Mutashabihat Navigation) | `AI-OP-003`
- **Core Question:**
  > *What is the empirical Phoneme Error Rate (PER) and Word Error Rate (WER) of on-device acoustic models (e.g. Wav2Vec2-Quran, Whisper fine-tuned on Qira'at) when evaluating non-native Arabic Quranic recitation across diverse accent cohorts (South Asian, West African, Southeast Asian, Western converts)?*
- **Why It Matters:**
  - The council demoted ASR to an optional experimental add-on due to concerns over Tajweed false-positive error flags.
  - If on-device acoustic phoneme alignment against a closed reference text achieves a low false-error rate (<5%), the hands-free active recall drill can be safely re-integrated; if error rates exceed 15%, the feature will infuriate memorizers and must be permanently discarded.
- **Current State of Evidence:**
  - General Arabic ASR benchmarks show high word error rates (>25%) on non-native speakers, but constrained phoneme alignment against a single known target ayah has not been systematically benchmarked across multi-dialect Tajweed datasets.
- **Recommended Validation Method:**
  - Assemble a diverse speech test set of 500 audio recordings of 50 common mutashabihat verse pairs recited by Huffadh from 5 geographic regions.
  - Measure false-rejection rate (correct recitation flagged as error) and false-acceptance rate (verbal twin swap missed by model).
- **Governance Marker:** `[REQUIRES EMPIRICAL BENCHMARK]`

---

### OPEN QUESTION ID: OQ-003
- **Target Problems & AI Opportunities:** `P-300` (Hadith Hallucination & Phantoms), `P-302` (Classical Takhrij Chasm), `P-001` (Lay Hadith Verification) | `AI-OP-010`, `AI-OP-012`, `AI-OP-001`
- **Core Question:**
  > *What is the current machine-readable coverage of cross-edition canonical hadith numbering concordance tables (linking Darussalam, Fu'ad Abd al-Baqi, Fath al-Bari, and USC-MSA numbering keys), and what engineering effort is required to achieve 100% canonical coverage across the Six Books?*
- **Why It Matters:**
  - The deterministic primary-key hallucination barrier (`P-300`) was barred by council adjudication from launching without a multi-edition concordance table, to prevent falsely blocking authentic hadiths that use non-default print numbering.
- **Current State of Evidence:**
  - Sunnah.com maintains internal cross-reference mappings between Darussalam and classical numbering for parts of Bukhari and Muslim, but public machine-readable coverage across Abu Dawud, Tirmidhi, Nasa'i, Ibn Majah, and Musnad Ahmad is incomplete and fragmented across disparate academic projects.
- **Recommended Validation Method:**
  - Perform a data-engineering intake audit of existing open-source hadith databases (Sunnah.com API, Dorar.net dumps, Shamela metadata).
  - Quantify the exact percentage of narrations in the Six Books possessing verified 1-to-1 cross-edition keys, and scope the manual reconciliation task for remaining gaps.
- **Governance Marker:** `[REQUIRES TECHNICAL DATA AUDIT]`

---

### OPEN QUESTION ID: OQ-004
- **Target Problem & AI Opportunity:** `P-100` (Solitary Salah Learning Overload) | `AI-OP-004`
- **Core Question:**
  > *Does an adaptive earbud-based audio coach using Voice Activity Detection (VAD) and smart-tempo pacing successfully reduce NASA-TLX cognitive load for Days 1–90 converts without causing auditory distraction, earbud dislodgement during Sujud, or spiritual unease?*
- **Why It Matters:**
  - The council permanently terminated smartphone camera pose tracking due to physical garment occlusion and surveillance anxiety, pivoting the architecture entirely to an adaptive hands-free audio coach.
  - The practical physical ergonomics of wearing an earbud during prayer and the psychological acceptability of whispered liturgical cues require direct validation with actual new Muslims.
- **Current State of Evidence:**
  - Validated evidence (`E02-001`, `E02-002`) documents severe cognitive overload with paper cheat sheets and YouTube videos, but no empirical study has evaluated real-time adaptive audio pacing during solitary Salah.
- **Recommended Validation Method:**
  - Conduct a structured 14-day usability trial with 15 adult first-year converts comparing three modalities: (A) Static paper floor guide, (B) Fixed-tempo timer audio, and (C) Adaptive VAD-prompted earbud audio.
  - Measure motor-recitation desynchronization episodes, NASA-TLX cognitive load scores, and qualitative reports of spiritual focus (*Khushu'*).
- **Governance Marker:** `[REQUIRES USER FIELD TRIAL]`

---

### OPEN QUESTION ID: OQ-005
- **Target Problem & AI Opportunity:** `P-302` (Fragmented Classical Takhrij Chasm) | `AI-OP-012`
- **Core Question:**
  > *Can rule-based biographical constraints (filtering by teacher-student transmission pairs, narrator generation era / Tabaqah, and geographical migration) increase classical Arabic narrator entity disambiguation accuracy from 95% to >99.5%, preventing the compounding error cascade across isnad trees?*
- **Why It Matters:**
  - In `CX-DOCK-07`, the council established that a 5% link extraction error compounds into a 26% invalid isnad graph across a 6-link transmission chain, which is academically and theologically unacceptable.
  - Determining whether relational biographical rules can eliminate ambiguous namesake mismatches (e.g. distinguishing between 30 different narrators named "Sufyan") determines whether automated isnad graph construction is scientifically viable beyond small curated sets.
- **Current State of Evidence:**
  - Classical Hadith biographical compendia (*Tahdhib al-Kamal*, *Taqrib al-Tahdhib*) document explicit teacher-student lists and generational tiers (*Tabaqat*), but these rules have not been formally combined with transformer-based sequence taggers in an end-to-end evaluation.
- **Recommended Validation Method:**
  - Test a hybrid NERD pipeline (AraBERT/CAMeL Tools sequence tagger + relational Rijal constraint filter) on an annotated evaluation corpus of 1,000 diverse isnad chains from Sahih al-Bukhari and Sunan al-Tirmidhi.
  - Measure whole-chain accuracy before and after biographical constraint filtering.
- **Governance Marker:** `[REQUIRES ALGORITHMIC BENCHMARK & SCHOLAR AUDIT]`

---

### OPEN QUESTION ID: OQ-006
- **Target Problem & AI Opportunity:** `P-200` (Khutbah Hadith Verification) | `AI-OP-007`
- **Core Question:**
  > *How do community imams and volunteer Friday khatibs respond when presented with an unweighted comparative scholarly evaluation matrix instead of a single definitive authenticity grade, and does it increase pulpit confidence or create decision paralysis under Thursday night deadlines?*
- **Why It Matters:**
  - The council stripped Shepard's traffic-light consensus badges because hadith criticism has no single supreme court, mandating an unweighted comparative list of scholar evaluations (e.g. Tirmidhi Hasan, Ibn Hajar corroborated, Albani Da'if).
  - If volunteer khatibs under deadline pressure find an unweighted matrix too ambiguous to use on the minbar, the tool may fail to achieve real-world pulpit adoption.
- **Current State of Evidence:**
  - Surveys of 25 imams (`E03-002`) confirm acute fear of preaching weak hadiths, but their operational threshold for evaluating divergent scholar gradings without a single summary score has not been tested in live sermon drafting workflows.
- **Recommended Validation Method:**
  - Deploy an interactive clickable prototype of the unweighted comparative scholar matrix to a cohort of 20 practicing imams and volunteer khatibs during weekly sermon preparation.
  - Evaluate whether the interface successfully aids sermon completion within <30 minutes, or whether khatibs demand an editorial summary consensus tier.
- **Governance Marker:** `[REQUIRES PRACTITIONER FIELD TRIAL]`

---

## 3. Governance Sign-off & Transition to Phase 7
These six Open Questions represent the formal research frontier for CYCLE-001. They must be explicitly referenced in Phase 7 Opportunity Mapping when establishing the feasibility and risk profiles of candidate projects.

*Signed,*  
**Agent 08 — Research Director**  
*Islamic AI Challenge Research Lab — CYCLE-001*
