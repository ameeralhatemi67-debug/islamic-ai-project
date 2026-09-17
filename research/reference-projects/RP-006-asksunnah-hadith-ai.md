# [RP-006] AskSunnah & Emerging Hadith AI Verifiers (AskSunnah, HadithGPT, Theo)

---

## 1. Classification
- **Category:** DIRECT COMPETITOR (for AI-based hadith verification) / RESEARCH PROTOTYPE / TECHNICAL REFERENCE
- **Related Problem Cards:** `P-001`, `P-200`, `P-300`, `P-302`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Project Names:**
  - **AskSunnah:** https://asksunnah.online (Web app & mobile verifier)
  - **HadithGPT:** https://hadithgpt.com (Historic prototype, discontinued/re-architecting)
  - **Theo (TheoGrid):** https://theogrid.ai (Scholar-grade isnad AI verification)
  - **Daleel AI:** https://daleel.ai (Mobile Islamic assistant)
- **Organization / Creators:** Independent AI startups, hackathon teams, and AI researchers.
- **Launch Dates:** 2023–2026
- **Current Status:** Emerging / Fragmented / Some discontinued (HadithGPT taken offline for safety; AskSunnah active; Theo in private/beta development).
- **Primary Language(s):** English and Arabic.

---

## 3. Target User & Use Case
- **Target User:** Digital Muslims, content creators, researchers, and youth trying to verify hadiths using natural language or image screenshots.
- **Core Job:** "When I see a quote or screenshot of a hadith online, I want to upload it to an AI and get an immediate answer: Is this authentic, where is it found, and what does it mean?"

---

## 4. Key Capabilities & Technical Approaches
1. **AskSunnah Hadith Verifier:**
   - Text & Image Upload: Users paste English/Arabic text or upload screenshots from TikTok/Instagram.
   - OCR Extraction: Optical Character Recognition extracts the quote text.
   - Vector / Keyword Search: Matches text against indexed Sunnah.com / Six Books collections.
   - Verification Badge: Outputs an authenticity label (*Sahih*, *Da'if*, etc.) with a source link.
2. **HadithGPT (Historic Prototype):**
   - Attempted conversational retrieval on hadith collections using GPT-3.5/GPT-4.
   - Discontinued: Shut down after public criticism from scholars due to hallucinated citations and contradictory rulings.
3. **Theo (TheoGrid AI):**
   - Focuses on deep *Isnad* (chain of transmission) and *Ilal* (hidden defects) analysis.
   - Uses a "Chain-of-Verification" multi-step pipeline for Islamic scholars.

---

## 5. What They Do Well
1. Identify the acute user demand for mobile, natural-language, screenshot-based verification.
2. Pioneer multimodal verification (OCR image-to-hadith matching in AskSunnah).
3. Attempt to tackle the hallucination problem head-on through retrieval constraints.

---

## 6. Critical Vulnerabilities & Why Problems P-001 / P-300 Persist
1. **Shallow Corpus Coverage:** Most consumer tools (AskSunnah, Daleel) only index the Six Books via English Sunnah.com dumps. If a quote is from Musnad Ahmad, Al-Tabarani, or Shu'ab al-Iman, the tool falsely reports: "Not Found / Likely Fabricated".
2. **Autoregressive Hallucination Leakage:** Generative AI layers wrap retrieved quotes in explanations that frequently hallucinate context, companion backstories, or legal implications (`P-300`).
3. **Black-Box Authentication:** Most tools output a single flat label ("Authentic - Sahih") without disclosing that Imam al-Tirmidhi and Imam al-Daraqutni disagreed on the narrator chain (`P-200`, `P-302`).
4. **Scholarly Authority Backlash:** Products like HadithGPT were forced to shut down because deploying autonomous generative models on sacred text without strict provenance guardrails creates catastrophic religious liability.

---

## 7. Strength Against Our Problem Space
- `P-001`: Direct competitor for OCR/mobile verification, but limited by shallow database and high false-negative rates on non-canonical texts.
- `P-200`: Inadequate for khutbah preparation; khatibs do not trust consumer AI bots for pulpits.
- `P-300`: The prime subject of study! These tools prove both the massive market hunger and the severe danger of hallucinated religious citations.
- `P-302`: Too superficial for scholarly takhrij.
