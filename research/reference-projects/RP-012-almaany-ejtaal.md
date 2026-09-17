# [RP-012] Almaany.com & ejtaal.net (Classical Arabic Lexical Engines)

---

## 1. Classification
- **Category:** DIRECT COMPETITOR (for Arabic lexical lookup) / TECHNICAL REFERENCE / NON-AI BASELINE
- **Related Problem Cards:** `P-102`, `P-202`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Project Names:**
  - **Almaany.com:** https://www.almaany.com (Universal Arabic dictionary portal)
  - **ejtaal.net (Arabic Almanac):** http://ejtaal.net/aa/ (Digitized classical lexicons: Lane's Lexicon, Hans Wehr, Lisan al-Arab)
- **Launch Dates:** ejtaal (~2010); Almaany (~2011).
- **Current Status:** Both active and relied upon by Arabic students and translators globally.
- **Primary Language(s):** Arabic, English, and multilingual dictionaries.

---

## 3. Target User & Use Case
- **Target User:** Arabic language students, translators, academics, and readers of classical texts.
- **Core Job:** "Look up the root meaning of a classical Arabic word across authoritative historical dictionaries (e.g. *Lisan al-Arab*, *Al-Qamus al-Muhit*, Edward William Lane's *Arabic-English Lexicon*, and Hans Wehr)."

---

## 4. Key Capabilities & Differences
1. **ejtaal.net (Arabic Almanac):**
   - Revolutionary digitization of Lane's Lexicon, Hans Wehr, Hava, Steingass, and classical Arabic dictionaries (*Lisan al-Arab*, *Taj al-Arus*).
   - Fast root-based navigation (e.g., typing `q-w-l` instantly jumps to the corresponding scanned page of Lane's Lexicon).
   - 100% free, minimalist interface.
2. **Almaany.com:**
   - Vast modern search engine indexing contemporary, technical, and classical meanings.
   - Specialized tabs: Qur'anic meanings, Fiqh terms, General terms, Bilingual translations.

---

## 5. Known Limitations & Workflow Gaps (`P-202`)
1. **Disconnected from Modern Translation Pipelines:** Neither tool integrates with Computer-Assisted Translation (CAT) software (Trados, memoQ) or word processors. Translators must constantly alt-tab between their translation editor and browser, breaking cognitive translation flow.
2. **ejtaal Scanned-Image Limitation:** ejtaal displays static scanned page images rather than editable text, meaning translators cannot copy-paste definitions or search full English definitions programmatically.
3. **Almaany Ad Clutter & Context-Blindness:** Almaany displays dozens of contradictory contemporary and colloquial definitions alongside classical ones, confusing non-expert translators and failing to identify specific theological exegesis (*Tafsir*).
4. **No Provenance or Footnote Automation:** Neither tool helps translators manage citation metadata or preserve classical footnotes.

---

## 6. Strength Against Our Problem Space
- Essential non-AI baselines for lexicography, but their isolation from modern publishing workflows is the exact root cause of the 3x translation latency documented in `P-202`.
