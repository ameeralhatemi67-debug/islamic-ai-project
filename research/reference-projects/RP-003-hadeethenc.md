# [RP-003] HadeethEnc.com (Encyclopedia of Translated Prophetic Hadiths)

---

## 1. Classification
- **Category:** PARTIAL COMPETITOR / ADJACENT ISLAMIC PROJECT / NON-AI BASELINE
- **Related Problem Cards:** `P-001`, `P-102`, `P-200`, `P-202`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Project Name:** Encyclopedia of Translated Prophetic Hadiths (موسوعة الأحاديث النبوية المترجمة)
- **Organization / Creator:** HadeethEnc / Islamic Translation Center (supervised by institutional Islamic da'wah bodies in Saudi Arabia).
- **Official URL:** https://hadeethenc.com
- **Repository URL:** Closed-source web platform; open public API available for developers.
- **Launch Date:** ~2018
- **Current Status:** Active, maintained, expanding translations
- **Country / Region:** Saudi Arabia / International
- **Primary Language(s):** Arabic, English, and 30+ international languages (French, Spanish, Urdu, Indonesian, Russian, Turkish, Bengali, Chinese, etc.).

---

## 3. Target User
- **Primary User:** Non-Arabic speaking Muslims, new Muslims, educators, translators, and da'wah workers needing pre-vetted, translated authentic hadiths with simplified commentary.
- **User Skill Level:** Novice to Intermediate.

---

## 4. Problem Addressed & Key Capabilities
- **What It Solves:** Solves the problem of mistranslated or unauthenticated hadiths in non-Arabic languages by providing a curated, scholar-vetted selection of authentic narrations (*Sahih* / *Hasan* only) with reliable multilingual translations, concise phrase-by-phrase explanations, vocabulary definitions, and derived benefits (*Fawa'id*).
- **Core Features:**
  1. Multilingual Translations: Professional, reviewed translations in 30+ languages.
  2. Integrated Commentary (*Sharh*): Every hadith includes a simplified explanation explaining the context and meaning.
  3. Vocabulary Definitions: Highlights difficult words (*Gharib*) and provides accessible definitions.
  4. Derived Rulings & Benefits: Bulleted list of theological, moral, and jurisprudential lessons.
  5. Public API: Free API for apps to fetch curated hadiths with translations.

---

## 5. Technical Approach & Islamic Methodology
- **Technical Stack:** Modern web architecture, Elasticsearch, clean multilingual taxonomy, RESTful API.
- **AI Used:** No. Hand-translated, scholar-vetted static editorial content.
- **Source Methodology:** Strictly selects narrations that meet high authentication thresholds (*Sahih* or *Hasan*). Unauthentic (*Da'if*) or fabricated (*Mawdu'*) narrations are excluded by design.

---

## 6. What It Does Well
1. Best-in-class translated explanations for the narrations it contains.
2. Direct phrase-level lexical breakdowns and benefits.
3. High institutional trust and rigorous translation review.

---

## 7. Known Limitations & Why Our Problem Space Survives
1. **Severely Limited Scope (~4,000–5,000 Hadiths):** Only includes curated high-frequency authentic traditions.
2. **Zero Takhrij for Wild / Paraphrased Claims:** When a user encounters a viral quote on TikTok, a controversial narration in a book, or an unverified quote on WhatsApp (`P-001`, `P-200`), HadeethEnc is useless because it does not index weak, contested, or uncurated narrations.
3. **No Isnad or Cross-Corpus Variant Analysis:** Does not provide full narrator chains or comparative transmission paths needed by imams and researchers (`P-200`, `P-302`).

---

## 8. Strength Against Our Problem Space
- `P-001`: Solves verification only for the curated 4,000 hadiths; 0% coverage for obscure, weak, or viral misattributed quotes.
- `P-102`: Strong partial solver for learners needing vetted explanations of core hadith terminology.
- `P-200`: Useful for finding a safe sermon quote, but useless when an imam needs to investigate an unfamiliar hadith under deadline.
