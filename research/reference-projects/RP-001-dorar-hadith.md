# [RP-001] Dorar.net (Al-Mawsu'ah al-Hadithiyyah / الموسوعة الحديثية)

---

## 1. Classification
- **Category:** DIRECT COMPETITOR (for Arabic hadith verification) / PARTIAL COMPETITOR (for general non-Arabic workflows) / NON-AI BASELINE
- **Related Problem Cards:** `P-001`, `P-200`, `P-300`, `P-302`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Project Name:** Dorar.net Hadith Encyclopedia (الموسوعة الحديثية - الدرر السنية)
- **Organization / Creator:** Dorar Al-Sunniyyah Foundation (مؤسسة الدرر السنية), supervised by Sheikh Alawi ibn Abd al-Qadir al-Saqqaf (الشيخ علوي بن عبد القادر السقاف).
- **Official URL:** https://dorar.net/hadith
- **Repository URL:** Closed source / Proprietary institutional database
- **Documentation URL:** https://dorar.net/article/261
- **Launch Date:** 2002 (Web portal); Continuous major revisions (v4 web / mobile apps 2018–2025)
- **Current Status:** Active, fully maintained, industry gold standard
- **Country / Region:** Kingdom of Saudi Arabia (Dhahran / Khobar)
- **Primary Language(s):** Classical Arabic (English portal is limited / static)

---

## 3. Target User
- **Primary User:** Arabic-literate Islamic researchers, scholars, students of Islamic knowledge (*Talabat al-'Ilm*), imams, and du'at.
- **Secondary Users:** General Arabic-speaking Muslims verifying received messages; bilingual translators using machine translation to bridge Arabic results.
- **User Skill Level:** Intermediate to Advanced in classical Arabic and *Mustalah al-Hadith* (hadith terminology).
- **Geography:** Global Arabic-speaking Ummah and Arabic-literate diaspora.
- **Language:** Classical / Modern Standard Arabic.
- **Relevant Context:** Accessible via responsive web portal, Android app, and iOS app.

---

## 4. Problem Addressed
- **What Problem Does It Solve:** Provides instant, authoritative access to over 2 million hadith narrations with authentic scholarly authentication rulings, isnad metadata, and comparative source citations across dozens of classical hadith compendia.
- **User Job Supported:** "When I encounter a hadith narration or quotation in Arabic, I want to quickly inspect its transmission paths, check its grading by classical and modern scholars, and confirm the exact primary source."
- **Workflow Part Addressed:** Takhrij retrieval, grading inspection, and variant comparison in classical Arabic.

---

## 5. Core User Workflow
- **Trigger:** User encounters an Arabic hadith text or partial quote and needs to verify its authenticity.
- **Step 1 (Query Formulation):** User enters a distinctive 2–4 word substring in Arabic (e.g., "إنما الأعمال بالنيات" or "طلب العلم فريضة").
- **Step 2 (Filtering):** User applies optional filters: search scope (All Hadiths vs. Only Sahih/Authentic), book filter (e.g., Sahih Bukhari, Sunan Abi Dawud), or specific scholar filter (e.g., Ibn Hajar, Al-Albani, Shu'ayb al-Arna'ut).
- **Step 3 (Results Inspection):** System returns a list of matching narrations. For each narration, it displays:
  - Full text of the narration (*Matn*).
  - Rawi (Companion narrator, e.g., Umar ibn al-Khattab).
  - Muhaddith (Author of the collection or verifier, e.g., Al-Bukhari, Al-Albani).
  - Source book and page/hadith number (e.g., Sahih al-Bukhari #1).
  - Grading verdict (*Hukm*), e.g., *Sahih*, *Hasan*, *Da'if*, *Mawdu'*, or detailed commentary.
- **Step 4 (Deep Dive / Takhrij):** User clicks "Takhrij" or "Alternative Paths" to inspect identical or similar narrations reported through other chains.
- **Outcome:** The user determines whether the narration is authentic according to documented scholars and cites the primary collection.

---

## 6. Core Features
1. **Exhaustive Hadith Database:** Indexes major, secondary, and tertiary hadith compendia (Kutub al-Sittah, Musnad Ahmad, Al-Mu'jam al-Kabir, Al-Bayhaqi, Ibn Hibban, etc.).
2. **Scholarly Verdict Aggregation:** Cites classical rulings (Al-Tirmidhi, Al-Daraqutni, Ibn Hajar, Al-Dhahabi) and modern verifiers (Al-Albani, Ahmad Shakir, Shu'ayb al-Arna'ut).
3. **Alternative Chains & Routes (*Turuq*):** Groups narrations with similar matn to trace isnad convergence.
4. **Sharh al-Hadith Integration:** Links narrations to verified classical explanations and contemporary simplified commentaries.
5. **Mobile Applications:** Full-featured iOS and Android apps with offline search capability for high-frequency narrations.

---

## 7. Technical Approach
- **AI Used:** No. Fully deterministic relational database with morphological indexing and advanced SQL / full-text search indexing.
- **Search Engine:** Arabic root and lemma-based substring and fuzzy matching; morphological normalization (alif, yaa, taa marbuta).
- **Database:** Proprietary normalized relational database structuring narrators, chains, collections, and rulings.
- **Evidence Source:** Direct inspection of Dorar.net platform and API behaviors.

---

## 8. Data / Knowledge Sources
- **Data Corpus:** Hundreds of thousands of classical hadith texts digitized from verified scholarly printed editions (*Tahqiqat*).
- **Source Disclosure:** 100% transparent. Every entry explicitly cites the primary book, volume, page, hadith number, and specific tahqiq edition.
- **Licensing:** Proprietary to Dorar Foundation; public web and mobile access free of charge.

---

## 9. Islamic Source Methodology
- **Applicable:** Yes.
- **Islamic Corpus:** Sunni canonical hadith corpus.
- **Scholarly Orientation:** Mainstream Sunni / Salafi-traditionalist methodology with broad inclusion of classical multi-madhhab hadith commentators (Ibn Hajar, Al-Nawawi, Al-Zayla'i, Al-Shawkani).
- **Handling of Disagreement:** Displays divergent gradings chronologically or by scholar. However, does not provide a meta-synthesis or consensus barometer for why Al-Tirmidhi graded a hadith *Hasan* while Al-Albani graded it *Da'if*.
- **Personal Fatwa Handling:** Out of scope; platform strictly indexes hadiths, not contemporary fiqh fatwas.

---

## 10. Trust and Safety Mechanisms
- **Direct Primary Citations:** Every entry links directly to a verifiable physical edition.
- **Editorial Review:** Supervised by a dedicated board of verified hadith researchers in Saudi Arabia.
- **Refusal / Uncertainty:** Does not synthesize or guess. If a text is not found in canonical collections, search returns zero results, indicating potential fabrication or severe obscurity.

---

## 11. User Experience
- **Primary Interaction Model:** Search bar with structured facet filters.
- **Key UX Strengths:** Extremely fast, highly reliable, zero hallucination, authoritative across the Arab Islamic world.
- **Key UX Weaknesses:** Strictly Arabic interface; dense typographical layouts; requires understanding of technical *Mustalah* abbreviations; no cross-lingual semantic query matching.

---

## 12. What It Does Well
1. Unmatched comprehensiveness for Arabic hadith verification.
2. Unflinching bibliographic provenance back to classical print editions.
3. Fast retrieval of variant chains (*turuq*) and narrator identifications.

---

## 13. Known Limitations
1. **Classical Arabic Lockout:** Completely unusable for non-Arabic speakers or English queries.
2. **Exact Substring Fragility:** If a user searches a colloquial paraphrase or translated concept, Dorar fails to match the classical Arabic matn.
3. **Raw Scholarly Disagreement Without Synthesis:** A novice or non-specialist imam searching an obscure hadith is confronted with 5 conflicting scholar judgments without guidance on which verdict represents majority consensus.

---

## 14. User Feedback
- **Positive Themes:** Considered by scholars and imams worldwide as the single most indispensable digital hadith tool; praised for saving days of manual book lookup.
- **Negative Themes:** Western converts, diaspora youth, and non-Arabic speakers frequently express frustration that they cannot access Dorar's goldmine of authentication data without relying on broken browser Google Translate extensions (`E01-002`).

---

## 15. Vendor Claims vs. Reality
- **Claim:** "The most comprehensive and accurate digital hadith encyclopedia in the world."
- **Assessment:** Validated. Within classical Arabic literature, Dorar is empirically verified as the market benchmark.

---

## 16. Project Maturity & Activity
- **Maturity:** Production enterprise platform (20+ years operational).
- **Usage Scale:** Tens of millions of monthly pageviews; millions of mobile app downloads.
- **Status:** Actively maintained.

---

## 17. Strength Against Our Problem Space
- **P-001 (Lay User Mobile Verification):** Weak coverage. Non-Arabic speakers cannot use it directly; English interface is minimal.
- **P-200 (Imam Khutbah Prep):** Partial solver. Imams with Arabic literacy use it constantly, but spend substantial time reconciling conflicting gradings and copying text across tabs into their English sermon drafts.
- **P-300 (AI Phantom Citation Guardrail):** Critical baseline. Represents the exact ground-truth database against which AI-generated citations must be validated.
- **P-302 (Cross-Corpus Scholarly Takhrij):** Partial solver. Provides raw data, but lacks integration with Maktabah Shamela text readers, isnad graph visualizations, or English translations.

---

## 18. Remaining Gap (Why Our Problem Survives)
Dorar.net provides the supreme Arabic verification database, but is structurally isolated:
- It has no cross-lingual semantic layer (cannot resolve English conceptual queries to Arabic matns).
- It does not provide automated consensus synthesis for divergent gradings.
- It does not connect directly to educator drafting tools or AI verification APIs.

---

## 19. Lessons Learned
- **What to Emulate:** Strict bibliographic attribution standard, inclusion of multiple scholar verdicts, clean separation of matn and isnad metadata.
- **What NOT to Emulate:** Monolingual confinement, dense unassisted technical jargon, lack of conceptual semantic retrieval.
