# [TECH-002] FiqhQA Benchmark (Evaluating LLM Reliability and Abstention for Islamic Jurisprudence)

---

## 1. Classification
- **Category:** TECHNICAL BENCHMARK / RESEARCH PROTOTYPE / METRIC BASELINE
- **Related Problem Cards:** `P-002`, `P-101`, `P-301`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Benchmark Name:** FiqhQA: Evaluating Large Language Model Reliability, Abstention, and Bias in Islamic Jurisprudence
- **Organization / Authors:** A. Atif et al. (AAAI/ACM Conference on AI, Ethics, and Society / AIES 2025; arXiv:2508.08287).
- **Official URL:** https://arxiv.org/abs/2508.08287
- **Launch Date:** 2025
- **Current Status:** Authoritative peer-reviewed ethical/technical benchmark.
- **Primary Language(s):** Arabic and English.

---

## 3. Dataset Architecture & Evaluation Focus
1. **Ground-Truth Corpus:** Built directly upon the authoritative 45-volume *Kuwaiti Fiqh Encyclopedia* (الموسوعة الفقهية الكويتية), the largest pan-Islamic codification of comparative Sunni jurisprudence across all four schools (Hanafi, Maliki, Shafi'i, Hanbali).
2. **Key Evaluation Dimensions:**
   - **Madhhab Discrimination:** Can the LLM accurately identify differences between schools on a specific question?
   - **Abstention Calibration:** Does the model abstain or express uncertainty when presented with unresolvable or context-dependent legal dilemmas?
   - **Linguistic Parity:** Evaluates performance degradation between English queries and classical Arabic queries.

---

## 4. Key Benchmark Findings & Empirical Baselines
1. **Total Failure to Abstain:** Commercial frontier LLMs (including GPT-4, Claude, and Llama-3) attempt to answer 98%+ of ambiguous or high-stakes fiqh queries, refusing to abstain even when lacking necessary context (e.g. user health, local custom, madhhab).
2. **Context-Flattening across Madhahib:** Generative models systematically flatten nuanced multi-school debates into a single flat assertion ("In Islam, the rule is X"), usually defaulting to the most common internet-scraped Salafi/Hanbali perspective while erasing Hanafi and Maliki counter-positions (`P-301`).
3. **Severe Arabic Degradation:** LLM accuracy drops significantly when queried in classical Arabic fiqh terminology compared to simplified English prompts.

---

## 5. Architectural Significance for Islamic AI Challenge
- Provides empirical proof that LLMs cannot be trusted as autonomous legal advisors (`[NO AUTONOMOUS FATWA PERMITTED]`).
- Serves as the quantitative benchmark for testing whether a system successfully implements context-gating, multi-madhhab preservation, and appropriate abstention.
