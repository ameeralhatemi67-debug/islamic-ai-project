# [RP-007] IslamQA.info

---

## 1. Classification
- **Category:** DIRECT COMPETITOR (for online Islamic legal questions / fatwa search) / NON-AI BASELINE
- **Related Problem Cards:** `P-002`, `P-101`, `P-301`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Project Name:** Islam Question and Answer (موقع الإسلام سؤال وجواب)
- **Organization / Creator:** Founded and supervised by Sheikh Muhammad Saalih al-Munajjid (الشيخ محمد صالح المنجد).
- **Official URL:** https://islamqa.info
- **Repository URL:** Closed-source enterprise portal; mobile apps on iOS/Android.
- **Documentation URL:** https://islamqa.info/en/about-us
- **Launch Date:** 1997 (One of the earliest Islamic websites on the internet)
- **Current Status:** Active, colossal global traffic, #1 SEO ranking in English/Arabic Islamic queries.
- **Country / Region:** Saudi Arabia (supervisory board) / International operations.
- **Primary Language(s):** Arabic, English, and 14 other languages (Urdu, French, Indonesian, Spanish, Bengali, Turkish, etc.).

---

## 3. Target User & Use Case
- **Primary User:** Practicing Muslims, converts, and seekers searching Google for practical religious rulings (*Halal* vs *Haram*).
- **Secondary Users:** Researchers studying contemporary Salafi/traditionalist jurisprudence.
- **Core Job:** "When I have a personal, ethical, ritual, or financial dilemma, I Google it and want an authoritative answer citing Qur'an, Hadith, and scholarly rulings."

---

## 4. Key Capabilities & Technical Approach
1. **Massive Question Archive:** Over 100,000 published answers across all spheres of life (worship, family, finance, medical ethics, creed, doubts).
2. **Dominant Global SEO:** Unrivaled Google search optimization; virtually any English query containing words like "haram", "ruling on", "can a Muslim" ranks IslamQA.info in the top 3 results.
3. **Primary-Text Citations:** Answers are heavily grounded with full citations from Qur'anic ayat, canonical hadith reports, classical tafsir, and statements from early scholars (*Salaf*).
4. **Structured Multi-Language Platform:** Full translations of popular fatwas into 16 languages.
5. **Deterministic Search:** Standard full-text search engine with tag and category taxonomy.

---

## 5. Islamic Source Methodology
- **School of Jurisprudence:** Strictly adheres to the Athari/Salafi methodology and Hanbali legal heritage, heavily influenced by the legal school of Sheikh al-Islam Ibn Taymiyyah, Ibn al-Qayyim, and contemporary Saudi scholars (Ibn Baz, Ibn Uthaymeen, Al-Albani).
- **Handling of Ikhtilaf (Disagreement):** Presents its chosen view as the authoritative, objective Islamic position. Often mentions opposing classical opinions only to refute them (*Tarjih*). Does not offer multi-madhhab parity or equal-weight presentation across Hanafi, Maliki, and Shafi'i schools.
- **Contextual Adaptation (*Fiqh al-Aqaliyyat*):** Very low. Answers rarely account for Western legal contexts, non-Muslim family cohabitation, or minority diaspora constraints.

---

## 6. What It Does Well
1. Unmatched speed of discovery via Google search.
2. In-depth textual citations and clear, unapologetic structure.
3. Completely free, ad-free, well-funded infrastructure.

---

## 7. Known Limitations & Toxic User Side-Effects (`P-002`, `P-101`)
1. **Trigger for Clinical Scrupulosity (*Waswas*):** Extensive user reports document that browsing IslamQA frequently induces severe anxiety, OCD symptoms, panic attacks, and fear of imminent damnation (`E01-003`). Its rulings frequently default to the strictest conceivable prohibition (e.g., ruling that all drawing of animate objects, conventional mortgages, non-essential interaction with opposite gender, and family attendance at Thanksgiving/Christmas dinners are grave sins).
2. **Convert Alienation & Family Estrangement:** Converts following IslamQA rulings often break ties with non-Muslim parents and abandon family meals, leading to intense psychological trauma and community fallout (`E02-003`, `E02-004`).
3. **Training Data Contamination in Frontier LLMs:** Because IslamQA has the largest cleanly structured, bilingual fatwa dataset on the public web, web crawlers (Common Crawl) ingest it heavily. As a result, general LLMs (GPT-4o, Claude) inherit its strict Salafi/Hanbali bias, presenting its rulings as universal "Islam" and erasing the four classical madhahib (`P-301`).

---

## 8. Strength Against Our Problem Space
- `P-002`: The exact SEO titan that causes the search paralysis and scrupulosity described in the card.
- `P-101`: The primary source of "convert fatwa whiplash".
- `P-301`: The dominant dataset responsible for LLM fiqh context-flattening.
