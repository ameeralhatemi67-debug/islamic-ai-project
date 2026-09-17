# [ADJ-001] Shepard's Citations & KeyCite (Legal Citators & Precedent Verification)

---

## 1. Classification
- **Category:** ADJACENT-DOMAIN REFERENCE / TECHNICAL REFERENCE
- **Related Problem Cards:** `P-001`, `P-200`, `P-300`, `P-302`
- **Adjacent Domain:** Legal Informatics, Common Law Jurisprudence, Citation Networks
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Systems Reviewed:**
  - **Shepard's Citations (LexisNexis):** Invented by Frank Shepard in 1873; modernized digital citator on Lexis+.
  - **KeyCite (Thomson Reuters Westlaw):** Advanced legal citator and appellate history tracker.
- **Industry:** Legal technology, judicial precedent verification.
- **Primary Users:** Attorneys, judges, paralegals, legal scholars.

---

## 3. Structural Analogy to Islamic Research
| Legal Precedent Workflow (Common Law) | Hadith Takhrij & Verification Workflow (Islamic Law) |
|---|---|
| **Judicial Opinion / Precedent:** A ruling issued by an appellate court. | **Prophetic Hadith / Athar:** A narration transmitted from the Prophet ﷺ or Companions. |
| **Direct History:** Has this case been appealed, reversed, or vacated? | **Isnad Analysis:** Has this chain been broken (*Inqita'*), or is it continuous (*Muttasil*)? |
| **Citing References:** Which subsequent courts have cited, distinguished, or questioned this ruling? | **Takhrij & Turuq:** Which other classical hadith compilers recorded this text through other routes? |
| **Treatment Signals (Red flag, Yellow warning, Green positive):** Instant visual indicator showing if case is still good law or overruled. | **Scholarly Authenticity Gradings (*Hukm*):** Instant indicator whether a hadith is *Sahih*, *Hasan*, *Da'if*, or *Mawdu'*. |
| **Negative Treatment Breakdown:** Explains exactly *why* a court rejected the precedent (e.g. abrogated by statute, distinguished on facts). | **'Ilal al-Hadith (Defects):** Explains *why* scholars rejected a narration (e.g. weak narrator in chain, anomaly/*Shadh*, hidden defect). |
| **Concordance Across Official Reporters:** Translates between US Reports, Supreme Court Reporter, and Law Ed. | **Cross-Edition Concordance:** Translates between Darussalam, Fath al-Bari, and classical manuscript numbering. |

---

## 4. Key Mechanisms to Transfer to Islamic AI
1. **Automated Status Signaling with Epistemic Transparency:**
   - Shepard's uses universal visual signals: Red stop sign (negative treatment/overruled), Yellow triangle (caution/distinguished), Green diamond (positive treatment).
   - *Transferable Mechanism:* Replace ambiguous raw Arabic gradings with an unambiguous consensus barometer (e.g. Consensus Sahih, Contested / Differing Gradings, Severe Weakness / Discredited) while preserving one-click access to the underlying classical rulings.
2. **Cross-Edition Concordance Normalization:**
   - Legal citators solve the problem of multiple legal publishers printing different page numbers by maintaining an immutable universal citation key (e.g., standard neutral citation format).
   - *Transferable Mechanism:* Build an immutable canonical Hadith Entity ID that links a specific prophetic narration across Shamela page numbers, Dorar database keys, and Sunnah.com web URLs.
3. **The Principle of Non-Autonomous Adjudication:**
   - Neither Shepard's nor KeyCite uses generative AI to invent legal opinions. They are deterministic citation graph indices.
   - *Transferable Mechanism:* Verification engines must ground outputs directly in verifiable citation graphs rather than autoregressive language model hallucinations.
