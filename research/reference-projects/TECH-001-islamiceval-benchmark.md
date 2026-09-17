# [TECH-001] IslamicEval 2025 Shared Task (Capturing LLM Hallucinations in Islamic Content)

---

## 1. Classification
- **Category:** TECHNICAL BENCHMARK / RESEARCH PROTOTYPE / METRIC BASELINE
- **Related Problem Cards:** `P-001`, `P-300`, `P-302`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Benchmark Name:** IslamicEval 2025: The First Shared Task of Capturing LLMs Hallucination in Islamic Content
- **Organization / Authors:** Hamdy Mubarak, Sabri Boughorbel, et al. (ArabicNLP 2025, Association for Computational Linguistics / ACL Anthology).
- **Official URL:** https://aclanthology.org/2025.arabicnlp-1.0/ / Shared Task Portal
- **Launch Date:** 2025
- **Current Status:** Authoritative peer-reviewed benchmark.
- **Primary Language(s):** Arabic and English.

---

## 3. Dataset Architecture & Subtasks
1. **Subtask 1: Hallucination Detection & Correction in Ayahs & Hadiths:**
   - Evaluates whether an NLP model can identify span-level hallucinated words, misattributed narrators, or corrupted texts in generated Islamic content and correct them to authentic canonical wording.
2. **Subtask 2: Retrieval-Augmented Canonical Source Identification:**
   - Given a query or claim, evaluates whether a retrieval system can locate the exact canonical Hadith or Qur'anic verse across large corpora.

---

## 4. Key Benchmark Findings & Empirical Baselines
1. **Correction Accuracy Capped at 68.18%:**
   - The top-performing system in the entire global competition achieved only 68.18% accuracy in correcting corrupted hadiths, leaving **over 31.8% of errors completely uncorrected**.
2. **Abysmal Retrieval Precision (MAP@10 ~0.23):**
   - Mean Average Precision at rank 10 across canonical hadith retrieval was only approximately 0.23, demonstrating that off-the-shelf dense vector embeddings (like text-embedding-ada-002 or multilingual BERT) fail catastrophically on classical Arabic religious texts.
3. **Fluency Masks Fabrication:**
   - Models generate grammatically impeccable classical Arabic while fabricating entire chains of narrators (*Isnad*) and inventing collection numbers ("Sahih al-Bukhari #9999").

---

## 5. Architectural Significance for Islamic AI Challenge
- Proves empirically that standard RAG pipelines and prompt-engineering cannot solve the hadith hallucination problem (`P-300`).
- Establishes the mandatory baseline that any viable solution must employ cryptographic token matching against verified corpora rather than probabilistic vector approximations.
