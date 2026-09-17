# Evidence Record: E04-002

- **EVIDENCE ID:** E04-002
- **CLAIM SUPPORTED:** LLMs frequently fail to abstain when encountering ambiguous, context-dependent Islamic jurisprudence questions, and display severe performance degradation in Arabic compared to English alongside erratic accuracy across the four Sunni madhahib (Hanafi, Maliki, Shafi'i, Hanbali).
- **SOURCE TYPE:** Academic and scientific research (Peer-reviewed conference paper)
- **SOURCE:** Farah Atif, Nursultan Askarbekuly, Kareem Darwish, Monojit Choudhury, "Sacred or Synthetic? Evaluating LLM Reliability and Abstention for Religious Questions", Proceedings of the 8th AAAI/ACM Conference on AI, Ethics, and Society (AIES 2025) / arXiv:2508.08287.
- **URL:** https://arxiv.org/abs/2508.08287
- **DATE:** 2025-08
- **TARGET USER / POPULATION:** Muslims seeking jurisprudential rulings (*ahkam*), students of Islamic law, and developers building religious AI applications.
- **GEOGRAPHY:** Global
- **LANGUAGE:** Arabic and English (Bilingual parallel evaluation)
- **DIRECT OR INDIRECT:** Direct empirical evaluation of frontier LLMs.
- **PRIMARY OR SECONDARY:** Primary research study introducing the FiqhQA benchmark.

## KEY EVIDENCE
1. **FiqhQA Benchmark Composition:** 960 multiple-choice question-answer pairs derived from the authoritative *Kuwaiti Fiqh Encyclopedia* (*Al-Mawsu'ah al-Fiqhiyyah al-Kuwaytiyyah*, Kuwait Ministry of Awqaf and Islamic Affairs), covering acts of worship (*Fiqh al-'Ibadat*) across the four major Sunni schools of thought (Hanafi, Maliki, Shafi'i, Hanbali).
2. **Abstention Failure:** The study introduces the critical metric of *abstention*?evaluating whether an LLM can decline to answer when a question is unanswerable or requires contextual nuance. Most frontier models exhibit overconfidence, attempting to answer context-dependent or ambiguous fiqh questions rather than declaring uncertainty or referring to a scholar.
3. **Severe Arabic Language Penalty:** All tested models (including GPT-4o, Gemini, and open models) exhibited a noticeable performance drop when processing queries in Arabic compared to English, demonstrating that Arabic religious reasoning is substantially weaker than English surface-level reasoning.
4. **Madhhab Inconsistency:** Models display erratic performance variance across the four schools of thought, frequently conflating the ruling of one madhhab with another, or asserting that a minority or school-specific position is universally binding on all Muslims.
5. **Model Variance:** While GPT-4o achieved the highest raw accuracy, systems like Gemini and Fanar demonstrated better calibrated abstention, proving that high generative capability does not correlate with appropriate religious restraint.

## LIMITATIONS
- Focuses specifically on *Fiqh al-'Ibadat* (ritual worship); does not yet evaluate complex modern transactions (*Mu'amalat*), financial contracts, or bioethics.
- Multiple-choice format measures factual discrimination rather than open-ended conversational advice generation.

## CONTRADICTING / DISCONFIRMING EVIDENCE
- Advanced prompting and system-level calibration (e.g., explicit instructions to abstain when uncertain) can improve abstention behavior in select models, showing that failure to abstain is partially an architectural and prompt calibration issue rather than an intrinsic impossibility.

## STRENGTH & CONFIDENCE
- **STRENGTH:** Strong (Peer-reviewed at AAAI/ACM AIES 2025, rigorous methodology, canonical reference corpus).
- **CONFIDENCE IN INTERPRETATION:** High.
