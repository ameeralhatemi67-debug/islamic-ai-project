# Evidence Record: E04-003

- **EVIDENCE ID:** E04-003
- **CLAIM SUPPORTED:** Frontier Large Language Models exhibit dramatic accuracy dispersion (ranging from 39.8% to 93.8%) and pronounced implicit madhhab bias across structured Islamic knowledge disciplines, with major reliability risks in Hadith and Fiqh reasoning.
- **SOURCE TYPE:** Academic and scientific research (Preprint & public benchmark leaderboard)
- **SOURCE:** Ali Abdelaal, Mohammed Nader Al Haffar, Mahmoud Fawzi, Walid Magdy, "IslamicMMLU: A Benchmark for Evaluating LLMs on Islamic Knowledge", arXiv:2603.23750.
- **URL:** https://arxiv.org/abs/2603.23750
- **DATE:** 2026-03
- **TARGET USER / POPULATION:** AI researchers, Islamic software developers, educators, and Muslim end-users.
- **GEOGRAPHY:** Global
- **LANGUAGE:** Arabic and English
- **DIRECT OR INDIRECT:** Direct evaluation across 26 frontier and domain-specific LLMs.
- **PRIMARY OR SECONDARY:** Primary benchmark study.

## KEY EVIDENCE
1. **Scale & Depth:** IslamicMMLU provides 10,013 multiple-choice questions across three core Islamic disciplines: Qur'an (2,013 questions), Hadith (4,000 questions), and Fiqh (4,000 questions).
2. **Massive Performance Variance:** Evaluating 26 LLMs revealed a wide accuracy spread from 39.8% (near-random guess baseline for 4-option MCQs) to 93.8%, demonstrating that many widely deployed open and proprietary models possess critically poor Islamic knowledge bases.
3. **Madhhab Bias Detection Task:** The benchmark introduces a novel task specifically quantifying school-of-thought bias in LLMs. Findings indicate that models carry implicit biases favoring specific legal schools based on the demographic and corpus weighting of their pretraining datasets.
4. **Hadith Reliability Deficit:** Across the 4,000 Hadith questions, models frequently fail to distinguish between authentic (*Sahih*) narrations and weak (*Da'if*) or fabricated (*Mawdu'*) reports, and frequently misattribute hadiths across different canonical collections.

## LIMITATIONS
- As an MMLU-style multiple-choice dataset, it tests parametric memory and discriminative knowledge rather than generative synthesis or conversational interaction.
- The 26 models evaluated represent a snapshot in time; newer fine-tunes may achieve higher raw scores without necessarily solving underlying epistemological issues.

## CONTRADICTING / DISCONFIRMING EVIDENCE
- Leading closed models (e.g., top-tier GPT-4 variants) score above 90% on aggregate, indicating that extensive pretraining can capture substantial factual Islamic knowledge.

## STRENGTH & CONFIDENCE
- **STRENGTH:** Strong (Extensive 10,013-item dataset, multi-model evaluation, public leaderboard).
- **CONFIDENCE IN INTERPRETATION:** High.
