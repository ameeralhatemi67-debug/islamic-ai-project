# [ADJ-004] SDL Trados Studio & Smartcat (Enterprise Translation & Controlled Termbases)

---

## 1. Classification
- **Category:** ADJACENT-DOMAIN REFERENCE / TECHNICAL REFERENCE / WORKFLOW BASELINE
- **Related Problem Cards:** `P-102`, `P-202`
- **Adjacent Domain:** Computer-Assisted Translation (CAT), Localization Technology, Terminology Management
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Systems Reviewed:**
  - **SDL Trados Studio (RWS):** Global industry benchmark for professional translation memory (TM) and termbase (TB) management.
  - **Smartcat:** Modern cloud-based collaborative CAT platform integrating neural machine translation and glossary locks.
- **Industry:** Commercial translation, localization, terminology governance.
- **Primary Users:** Professional translators, localization project managers, academic publishing houses.

---

## 3. Structural Analogy to Islamic Text Localization
| Professional CAT Workflow (Specialized Domain) | Classical Islamic Text Localization Workflow |
|---|---|
| **Controlled Termbases (TB):** Standardizes technical terms (e.g. medical/legal) across a global team; prevents translators from using colloquial synonyms. | **Sacred Lexical Termbases (*Istilah Shar'i*):** Standardizing complex theological concepts (*Taqwa*, *Bid'ah*, *Zuhd*) across translations to prevent semantic flattening (`P-202`). |
| **"Do Not Translate" (DNT) / Lock Rules:** Specific trademarked terms, code variables, or Latin names are locked from neural translation. | **Sacred Transliteration & Polysemy Locks:** Ensuring core theological terms are not degraded into secular approximations (e.g. preventing *Taqwa* $\rightarrow$ "fear"). |
| **Concordance Search in Translation Memories:** Instant lookup showing how a specific phrase was translated in 50 previous company manuals. | **Classical Exegetical Concordance:** Instant lookup showing how classical exegetes (*Tafsir Ibn Kathir*, *Al-Razi*) explained a specific Qur'anic or Hadith phrase. |
| **Tag & Footnote Preservation:** Ensures formatting, XML tags, and bibliographic citations are never stripped during translation. | **Classical Footnote & Isnad Provenance Preservation:** Ensuring classical chains, manuscript page citations, and marginal notes survive modern localization. |

---

## 4. Key Mechanisms to Transfer to Islamic AI
1. **The In-Editor Sacred Termbase Engine:**
   - Translators fail on Islamic texts because off-the-shelf CAT tools have zero knowledge of *Tafsir* or classical Arabic lexicons.
   - *Transferable Mechanism for `P-202`:* A specialized localization plugin that integrates *Lisan al-Arab*, *Al-Mufradat*, and classical Tafsir directly into the editor interface, flagging theological polysemes and suggesting scholar-approved glosses in real-time.
2. **Immutable Footnote & Citation Preservation Pipelines:**
   - Machine translation breaks when sentences are interrupted by classical citations (e.g. "[Sahih al-Bukhari 1421]").
   - *Transferable Mechanism:* Abstract citations into immutable semantic tokens before translation, re-injecting verified target-language bibliographic links into the output text.
3. **Collaborative Multi-Scholar Glossaries:**
   - Replacing ad-hoc Google Sheets with a shared, version-controlled repository of Islamic terminology that publishing houses can share and update collaboratively.
