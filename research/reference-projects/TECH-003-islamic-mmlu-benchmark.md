# [TECH-003] IslamicMMLU Benchmark (Massive Multitask Islamic Understanding Benchmark)

---

## 1. Classification
- **Category:** TECHNICAL BENCHMARK / RESEARCH PROTOTYPE / METRIC BASELINE
- **Related Problem Cards:** `P-001`, `P-300`, `P-301`, `P-302`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Benchmark Name:** IslamicMMLU: A Comprehensive Multitask Benchmark for Evaluating LLMs on Islamic Knowledge
- **Organization / Authors:** M. Abdelaal, K. Al-Sabahi, et al. (arXiv:2603.23750, 2026).
- **Official URL:** https://arxiv.org/abs/2603.23750
- **Launch Date:** 2026
- **Current Status:** The largest multi-discipline Islamic AI evaluation benchmark.
- **Primary Language(s):** Arabic and English.

---

## 3. Dataset Architecture & Scope
1. **Scope:** Over 12,000 vetted multiple-choice and open-ended questions covering:
   - 4,000 Hadith Science questions (Isnad evaluation, narrator status, collection concordance, grading).
   - 3,500 Fiqh & Usul al-Fiqh questions across the 4 Sunni Madhahib.
   - 2,500 Qur'anic Sciences & Exegesis (*Tafsir*).
   - 2,000 Islamic Creed (*'Aqeedah*) & History.
2. **Evaluated Models:** Tested across 26 open-source and proprietary LLMs (GPT-4o, Claude 3.5 Sonnet, Gemini 1.5 Pro, Llama-3-70B, Jais, Fanous, AceGPT).

---

## 4. Key Benchmark Findings & Empirical Baselines
1. **Massive Accuracy Dispersion (39.8% to 93.8%):**
   - General models perform unpredictably; while top proprietary models score well on high-level general facts, open-source and smaller models perform near random chance on detailed isnad criticism.
2. **The "Famous vs Obscure" Hadith Divide:**
   - On the top 500 mutawatir hadiths, top LLMs exceed 90% accuracy.
   - On narrations outside the Six Books (e.g. Musnad Ahmad, Tabarani, Bayhaqi), accuracy drops below 45%, with severe narrator hallucination.
3. **Cross-Madhhab Confusion:**
   - When asked to identify the specific Shafi'i ruling vs Hanafi ruling on complex transactions or ritual doubts, models confuse school positions in over 38% of test pairs.

---

## 5. Architectural Significance for Islamic AI Challenge
- Demonstrates why raw parametric LLM memory cannot be trusted for hadith authentication or multi-school legal analysis without an external, deterministic grounding graph.
