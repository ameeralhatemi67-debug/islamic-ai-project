# Evidence Record: E04-001

- **EVIDENCE ID:** E04-001
- **CLAIM SUPPORTED:** General-purpose and specialized Large Language Models exhibit severe, measurable hallucination rates when quoting, citing, or correcting Qur'anic ayahs and Hadith texts, with dedicated mitigation pipelines failing to correct over 31.8% of errors and retrieval precision remaining critically low (MAP@10 ~0.23).
- **SOURCE TYPE:** Academic and scientific research (Peer-reviewed conference shared task)
- **SOURCE:** Hamdy Mubarak, Tamer Elsayed, et al., "IslamicEval 2025: The First Shared Task of Capturing LLMs Hallucination in Islamic Content", ArabicNLP 2025 (co-located with EMNLP 2025), ACL Anthology.
- **URL:** https://aclanthology.org/2025.arabicnlp-1.0/
- **DATE:** 2025
- **TARGET USER / POPULATION:** Developers, researchers, educators, and end-users querying LLMs for Islamic textual citations (Qur'an and Hadith).
- **GEOGRAPHY:** Global (Research consortium across Qatar Computing Research Institute, HBKU, and international universities)
- **LANGUAGE:** Arabic and English
- **DIRECT OR INDIRECT:** Direct empirical measurement on standardized test sets.
- **PRIMARY OR SECONDARY:** Primary benchmark report.

## KEY EVIDENCE
1. **Subtask 1A (Identification of Sacred Text Spans):** Top-performing systems achieved F1 scores of 86.1% to 87.2% in detecting Ayahs and Hadiths in LLM outputs, demonstrating that even recognizing when an LLM is reciting religious text is non-trivial and prone to boundary errors.
2. **Subtask 1B (Validation of Authenticity & Accuracy):** Validation accuracy reached approximately 89.8%, meaning ~10% of generated religious quotes were incorrectly classified as genuine or erroneous.
3. **Subtask 1C (Hallucination Correction):** The most challenging task; the leading dedicated pipeline achieved only 68.18% accuracy in correcting hallucinated verses and hadith matn/isnad. More than 31.8% of hallucinated religious texts remained uncorrected even with state-of-the-art hybrid models.
4. **Subtask 2 (Retrieval-Augmented Question Answering):** Dense and sparse retrieval mechanisms achieved a Mean Average Precision at rank 10 (MAP@10) of only ~0.23. This demonstrates that standard RAG pipelines fail to retrieve the correct authoritative Islamic reference in over 75% of ranked attempts.
5. **Span-Level Vulnerability:** Hallucinations in Islamic texts do not only present as grand fictional narratives; they frequently occur as subtle character-level or word-level corruptions in the *matn* (text), fabricated narrators in the *isnad* (chain), or invented chapter/hadith numbers, which escape coarse response-level automated filtering.

## LIMITATIONS
- Evaluated on a competition test set curated by researchers; real-world user prompts may feature broader variations in phrasing, typos, dialectal Arabic, and conversational confusion.
- The shared task primarily evaluated text generation and retrieval against canonical collections, rather than evaluating lay user behavioral reactions to hallucinations.

## CONTRADICTING / DISCONFIRMING EVIDENCE
- Hybrid pipelines combining dense retrieval (e.g., mE5-base) with domain-adapted LLMs demonstrate substantial improvement over vanilla zero-shot LLMs (which exhibited significantly higher raw hallucination rates).

## STRENGTH & CONFIDENCE
- **STRENGTH:** Strong (Controlled, competitive, reproducible benchmark with multi-team participation).
- **CONFIDENCE IN INTERPRETATION:** High.
