# [RP-004] Al-Maktabah al-Shāmilah (المكتبة الشاملة / shamela.ws)

---

## 1. Classification
- **Category:** DIRECT COMPETITOR (for classical Islamic scholarly research) / TECHNICAL REFERENCE / NON-AI BASELINE
- **Related Problem Cards:** `P-200`, `P-202`, `P-301`, `P-302`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Project Name:** Al-Maktabah al-Shāmilah (The Comprehensive Library / المكتبة الشاملة)
- **Organization / Creator:** Maktabat Shamela Foundation / Nafi Technology (non-profit Islamic digitization initiative led by Nafi' and team).
- **Official URL:** https://shamela.ws
- **Repository URL:** Desktop software installer (Windows); web version; mobile apps (iOS/Android).
- **Launch Date:** 2005 (v1); Version 4 (desktop rewrite) 2018; web portal continuous.
- **Current Status:** Active, the definitive universal digital library of classical Islam.
- **Country / Region:** Egypt / Saudi Arabia / Global Islamic World.
- **Primary Language(s):** Classical Arabic exclusively.

---

## 3. Target User & Use Case
- **Primary User:** Traditional Islamic scholars, university professors, graduate students (MA/PhD), muftis, editors of classical manuscripts (*Muhaqqiqun*), and advanced students of knowledge.
- **Core Job:** "When conducting academic or legal research across classical Arabic heritage, I want to search full-text across 8,000+ volumes, inspect original book page breaks and volume numbers, view narrator biographies, and cross-reference tafsir and fiqh treatises."

---

## 4. Key Capabilities & Technical Approach
1. **Unmatched Classical Corpus:** Over 8,000 digitized classical books covering Qur'anic sciences, Hadith collections and commentaries, Fiqh across all four Sunni schools, Usul al-Fiqh, Islamic history, Rijal (narrator biographies), Arabic language/lexicons, and poetry.
2. **Page-Number Fidelity:** Matches the pagination and volume numbers of specific verified physical print editions (e.g., Dar al-Fikr, Dar al-Kutub al-Ilmiyyah, Mu'assasat al-Risalah), allowing formal academic citation.
3. **Multi-Field Desktop Search:** Supports complex boolean searching, morphological variations, category-specific filtering, and narrator lookup.
4. **Offline Capability:** The complete 8,000-book collection (~60 GB) can be downloaded and operated 100% offline on Windows.
5. **Technical Architecture:** Desktop version built in C++ / Delphi / SQLite; web portal uses PHP / MySQL with Elasticsearch backend. No AI or neural embeddings.

---

## 5. What It Does Well
1. Unchallenged market authority for classical Islamic full-text retrieval.
2. Faithful page/volume correspondence to printed manuscripts.
3. Completely free, unrestricted scholarly tool without paywalls or ads.

---

## 6. Known Limitations & User Friction
1. **Desktop-Era Usability Barrier:** Legacy Windows interface requires complex folder/category navigation; mobile and web versions have limited search features compared to desktop.
2. **Exact-Match Blindness:** Lacks semantic understanding. If a user does not know the exact classical morphological root or spelling used by the 10th-century author, search returns zero hits.
3. **No Cross-Corpus Graph Linkage:** Does not link an ayah or hadith directly to its isnad graph, Dorar.net authentication verdict, or English translation. Researchers must manually copy-paste text between Shamela, Dorar, and other tools (`P-302`).
4. **Monolingual Classical Arabic:** 100% inaccessible to non-Arabic readers and beginners (`P-001`, `P-102`).
5. **No Madhhab Comparative Synthesis:** While all 4 madhahib books are present, Shamela does not synthesize them into a structured comparison. A researcher must open 4 different fiqh compendia in 4 separate windows and read hundreds of pages.

---

## 7. Strength Against Our Problem Space
- `P-200`: Powerful for advanced imams with Arabic fluency, but takes 1–3 hours to search through multiple commentary volumes under khutbah deadlines.
- `P-202`: Indispensable for translators looking up classical definitions, but completely disconnected from modern CAT tools and word processors.
- `P-301`: Contains the source texts of the 4 madhahib, but cannot prevent LLMs from flattening them.
- `P-302`: The core centerpiece of the problem! Shamela is the primary desktop silo that researchers spend 45–90 minutes navigating in isolation from modern databases.
