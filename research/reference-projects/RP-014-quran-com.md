# [RP-014] Quran.com (The Noble Quran Digital Platform)

---

## 1. Classification
- **Category:** DIRECT COMPETITOR (for digital Quran reading) / PARTIAL COMPETITOR (for Quran comparison) / UX REFERENCE / NON-AI BASELINE
- **Related Problem Cards:** `P-003`, `P-100`, `P-102`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Project Name:** Quran.com
- **Organization / Creator:** Quran.com Foundation (non-profit open-source initiative led by volunteer engineers).
- **Official URL:** https://quran.com
- **Repository URL:** https://github.com/quran/quran.com-frontend-next
- **Launch Date:** 1995 (v1); modern Next.js rewrite (v4) in 2021–2025.
- **Current Status:** Active, the #1 digital Quran website globally (>30M monthly visits).
- **Primary Language(s):** Arabic, English, and dozens of international translations.

---

## 3. Target User & Use Case
- **Target User:** Global Muslims and non-Muslims reading, listening to, and studying the Holy Qur'an.
- **Core Job:** "Read, recite, listen to audio recitation, and inspect translations and tafsir for any verse in the Qur'an."

---

## 4. Key Capabilities & Product Features
1. **World-Class Digital Mushaf:** High-resolution Uthmanic font rendering (King Fahd Complex fonts), tajweed color-coding, verse-by-verse audio playback synchronized with word highlighting.
2. **Comprehensive Translations & Tafsir:** Over 100 translations across 40+ languages; multi-volume classical Arabic tafsirs (Ibn Kathir, Al-Tabari, Al-Qurtubi, Al-Sa'di) and English tafsirs.
3. **Word-by-Word Breakdown:** Tooltip displaying word-level translation, transliteration, and audio pronunciation.
4. **"Pin & Compare" Feature:** Allows users to manually pin specific verses into a persistent drawer to study them side-by-side.
5. **Open API:** Full RESTful API powering hundreds of third-party mobile apps and research tools.

---

## 5. Teardown: Why P-003 (Mutashabihat Friction) Remains Genuinely Unsolved
1. **Strictly Linear Codex Architecture:** Quran.com is architected around the traditional linear book model (Surah 1:1 -> Surah 114:6). It does not natively understand or surface non-linear relational patterns.
2. **"Pin & Compare" is Fully Manual:** The "Pin & Compare" feature requires the user to *already know* that Ayah 17:31 and Ayah 6:151 are similar, manually navigate to both distant surahs, and manually click "Pin" on each.
3. **Zero Automated Mutashabihat Detection or Clustering:** Quran.com does not automatically detect verbally similar verses (*Mutashabihat al-Lafz*), does not generate visual diffs between variations (e.g. highlighting *narzuqukum* vs *narzuquhum*), and contains zero rhetorical explanations (*Balaghah* / *Asrar al-Tanzil*) explaining why the phrasing differs.
4. **No Flashcard / Recall Testing:** Offers no interactive active-recall testing for huffadh preparing for Taraweeh recitation.

---

## 6. Strength Against Our Problem Space
- The undisputed benchmark for digital Quran reading and word-by-word study, but structurally incapable of solving the multi-surah comparative memory breakdown suffered by Quran memorizers (`P-003`).
