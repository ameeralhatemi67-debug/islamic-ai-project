# [RP-002] Sunnah.com

---

## 1. Classification
- **Category:** DIRECT COMPETITOR (for English hadith reading) / PARTIAL COMPETITOR (for hadith verification and takhrij) / NON-AI BASELINE
- **Related Problem Cards:** `P-001`, `P-200`, `P-300`, `P-302`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Project Name:** Sunnah.com (The Hadith Portal)
- **Organization / Creator:** Non-profit digital initiative led by volunteer developers and digital da'wah activists.
- **Official URL:** https://sunnah.com
- **Repository URL:** https://github.com/sunnah-com
- **Documentation URL:** https://sunnah.com/about
- **Launch Date:** 2011 (Web portal)
- **Current Status:** Active, widely adopted globally, maintained
- **Country / Region:** International / Open-source volunteer team (US, UK, Canada, diaspora)
- **Primary Language(s):** English and Arabic (with emerging Urdu, Indonesian, and French translations)

---

## 3. Target User
- **Primary User:** Non-Arabic speaking practicing Muslims, students of knowledge, youth, converts, and researchers.
- **Secondary Users:** Khutbah preparers (imams/khatibs), content creators looking for English hadith quotes.
- **User Skill Level:** Beginner to Intermediate.
- **Geography:** Global English-speaking Ummah (North America, UK, Europe, South Asia, Southeast Asia, Australasia).
- **Language:** English and Arabic.
- **Relevant Context:** Primary portal for finding translated hadiths on desktop and mobile browsers.

---

## 4. Problem Addressed
- **What Problem Does It Solve:** Provides a clean, bilingual web interface for searching and reading classical hadith collections with parallel English translations.
- **User Job Supported:** "When I need to look up or read a hadith in English or Arabic, I want a clean, indexed digital display that gives me the book name, chapter number, and hadith reference."
- **Workflow Part Addressed:** Reading, basic keyword searching, and collection browsing.

---

## 5. Core User Workflow
- **Trigger:** User remembers a phrase or topic from a hadith (e.g. "smile is charity" or "women deficient in intelligence").
- **Step 1 (Keyword Search):** User types words into the Sunnah.com search bar.
- **Step 2 (Exact String Match):** Search engine looks for matching strings in the indexed English or Arabic text.
- **Step 3 (Result Evaluation):** If found, displays parallel Arabic text and English translation, along with collection reference (e.g., Sahih al-Bukhari 304, Book 6, Hadith 9).
- **Step 4 (Grading Check):** User inspects grading badge (available primarily for Sunan Abi Dawud, Jami' at-Tirmidhi, Sunan an-Nasa'i, Sunan Ibn Majah based mostly on Darussalam / Al-Albani gradings). Note: Bukhari and Muslim are marked by default as Sahih.
- **Outcome:** User copies reference or text to paste in article, social post, or sermon notes.

---

## 6. Core Features
1. **Canonical Collections Indexed:** Covers the Six Books (Sahih al-Bukhari, Sahih Muslim, Sunan Abi Dawud, Jami' at-Tirmidhi, Sunan an-Nasa'i, Sunan Ibn Majah) plus Muwatta Malik, Musnad Ahmad (partial), Riyad as-Salihin, Bulugh al-Maram, 40 Hadith Nawawi, 40 Hadith Qudsi, and Shamail al-Muhammadiyyah.
2. **Parallel Bilingual View:** Arabic text on right, English on left (or responsive vertical stack).
3. **Reference Concordance:** Shows in-book reference, English translation reference, and USC-MSA web reference.
4. **Grading Badges:** Provides Darussalam / Zubair Ali Zai or Al-Albani authenticity tags on the four Sunan books.

---

## 7. Technical Approach
- **AI Used:** No. Deterministic PHP / MySQL / Elasticsearch search architecture.
- **Search Engine:** Traditional inverted index keyword matching (Elasticsearch).
- **Frontend / CMS:** Open-source modern web interface, responsive design.
- **Data Licensing:** Aggregates public domain and translated texts (many legacy translations sourced from Darussalam, Muhsin Khan, Aisha Bewley, etc.).

---

## 8. Data / Knowledge Sources
- **Corpus:** Primary Sunni hadith collections.
- **Translations:** Historical English translations (some dating to 1970s–1990s).
- **Source Disclosure:** Highly transparent about print editions used for each collection.

---

## 9. Islamic Source Methodology
- **Applicable:** Yes.
- **Islamic Corpus:** Sunni canonical hadith corpus.
- **Handling of Disagreement:** Only lists one primary grading per hadith (e.g., Darussalam's verdict). Does not display the spectrum of classical vs modern hadith scholars (e.g., Ibn Hajar vs Al-Albani).
- **Contextual Commentary (*Sharh*):** Almost entirely absent. Only raw text and translation are shown without *Fiqh al-Hadith*, *Sabab al-Wurud*, or classical explanations (e.g., *Fath al-Bari* or *Sharh Sahih Muslim* by Al-Nawawi).

---

## 10. Trust and Safety Mechanisms
- Direct chapter and hadith numbers.
- Explicit disclaimers regarding translation imperfections and volunteer corrections.
- No algorithmic hallucination (text is strictly static).

---

## 11. User Experience
- **Primary Interaction Model:** Search and collection browsing.
- **UX Strengths:** Clean typography, minimalist design, fast loading, high accessibility.
- **UX Weaknesses:** Search fails on paraphrased queries or synonyms; no semantic cross-lingual matching; archaic English translations cause misunderstandings (`E01-001`).

---

## 12. What It Does Well
1. Beautiful, fast parallel reading interface for the Six Books.
2. Most trusted and linked English hadith URL on the internet.
3. Accessible URL structure (e.g., `sunnah.com/bukhari:1`).

---

## 13. Known Limitations
1. **Search Brittleness:** Exact substring match fails if user searches "charity" instead of "alms", or paraphrases a narration.
2. **Corpus Boundary:** Does not index dozens of major classical collections (e.g. Al-Bayhaqi's Sunan al-Kubra, Al-Tabarani's 3 Mu'jams, Musannaf Abd al-Razzaq, Musannaf Ibn Abi Shaybah, Ibn Hibban, Al-Hakim's Mustadrak).
3. **Translation Polysemy & Semantic Drift:** Uses historical literalist translations that create serious theological misunderstandings (e.g. translating *'Aql* as "intelligence" in Bukhari 304 rather than "legal testimony/reasoning context", prompting user outrage; `E01-001`).
4. **No Isnad Trees or Cross-Corpus Takhrij:** Does not trace transmission paths or narrator biographies.

---

## 14. User Feedback
- **Positive:** Universal appreciation as the default English hadith reference tool.
- **Negative:** Countless forum posts complain that "Sunnah.com search is broken" because paraphrased queries yield 0 results, forcing users to use Google `site:sunnah.com` hacks. Outdated English phrasing draws repeated critique for fueling polemical attacks.

---

## 15. Strength Against Our Problem Space
- **P-001 (Lay User Hadith Verification):** Partial solver. Works if user has exact canonical quote from Bukhari/Muslim; fails completely on social media paraphrases, weak narrations, or obscure books.
- **P-200 (Imam Khutbah Prep):** Partial solver. Khatibs use it to grab English quotes, but cannot verify secondary narrations, resolve grading conflicts, or retrieve *Sabab al-Wurud*.
- **P-300 (AI Phantom Citations):** Target for AI hallucinations. LLMs frequently hallucinate fake Sunnah.com links and hadith numbers.
- **P-302 (Cross-Corpus Takhrij):** Inadequate for scholarly research due to missing collections, lack of isnad trees, and no concordance with Maktabah Shamela.

---

## 16. Remaining Gap
Sunnah.com is a reading portal, not a verification or takhrij engine. It lacks semantic understanding, comprehensive collection coverage, contextual commentary, and multi-scholar authentication synthesis.
