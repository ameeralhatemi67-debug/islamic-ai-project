# [RP-015] Tarteel.ai (AI-Powered Quran Memorization & Speech Recognition)

---

## 1. Classification
- **Category:** DIRECT COMPETITOR (for Quran AI recitation & memorization) / TECHNICAL REFERENCE / UX REFERENCE
- **Related Problem Cards:** `P-003`, `P-100`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Project Name:** Tarteel AI
- **Organization / Creator:** Tarteel Inc. (founded by Anas Al-Nabulsi and Abdellatif Abdelfattah).
- **Official URL:** https://tarteel.ai
- **Launch Date:** 2018 (voice search prototype); 2021 (full AI memorization companion).
- **Current Status:** Active, leading venture-backed commercial Quran AI application (>5M downloads).
- **Country / Region:** United States (San Francisco / remote global team).
- **Primary Language(s):** Classical Arabic (recitation input); English, Arabic, and multilingual UI.

---

## 3. Target User & Use Case
- **Target User:** Quran memorizers (Huffadh), students of Tahfeez schools, and daily reciters.
- **Core Job:** "Recite the Qur'an from memory and have an AI listen in real-time, detect verbal mistakes (word omissions, word substitutions, tashkeel errors), and hide words on the screen to test memory."

---

## 4. Key Capabilities & Technical Architecture
1. **Real-Time Acoustic ASR:** Proprietary acoustic speech recognition model specifically trained on Qur'anic phonemes, tajweed rules, and Arabic recitation styles (*Tartil*, *Hadr*).
2. **Memorization Mode (Hide Ayahs):** Hides text on the Mushaf page, revealing words only as the user recites them correctly, flagging mistakes in red in real-time.
3. **Voice Search ("Shazam for Quran"):** Recite any partial ayah to immediately identify the Surah and verse number.
4. **Historical Mistake Analytics:** Tracks recurring recitation mistakes across Juz and Surahs into a personalized error heatmap.
5. **Mutashabihat Highlighting (Premium Feature):** Color-codes verbally similar phrases directly within the linear Mushaf reading view.

---

## 5. Teardown: Why P-003 (Mutashabihat Recitation Friction) Survives
1. **Linear Recitation Paradigm:** Tarteel operates strictly within sequential recitation (Ayah $N \rightarrow N+1 \rightarrow N+2$). Its speech recognition engine expects the user to recite linearly.
2. **In-Text Color Highlights Only:** Tarteel's "Mutashabihat" feature merely colors words inline on the page. It does **not** provide a split-screen comparative view, does **not** diff the sentence syntax against distant Surahs, and does **not** explain the rhetorical context (*Balaghah*).
3. **Cannot Test Cross-Surah Disambiguation:** When a memorizer is practicing Surah al-Isra (Juz 15) and gets stuck on whether the verse ends with *narzuqukum wa iyyahum* or *narzuquhum wa iyyakum* (Surah al-An'am, Juz 8), Tarteel simply flags a mistake when the wrong word is uttered. It does not provide an interactive disambiguation drill comparing the two verses side-by-side.
4. **Subscription Paywall:** Advanced memorization features and mutashabihat highlights are locked behind a paid subscription ($40–$70/year), creating an adoption barrier for madrasahs and students in developing nations.

---

## 6. Strength Against Our Problem Space
- `P-003`: Phenomenal acoustic engineering for linear recitation verification, but structurally does not address non-linear cross-surah comparative mutashabihat mastery.
- `P-100`: Advanced speech recognition could theoretically help new Muslims, but Tarteel's model is trained on fluent classical recitation and is too strict/unforgiving for beginner converts struggling with basic phonetics.
