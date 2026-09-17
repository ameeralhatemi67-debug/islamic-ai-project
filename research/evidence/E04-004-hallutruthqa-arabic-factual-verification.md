# Evidence Record: E04-004

- **EVIDENCE ID:** E04-004
- **CLAIM SUPPORTED:** Arabic question answering suffers from fine-grained, span-level hallucinations where models generate fluent, grammatically flawless Arabic containing fabricated attributions, false historical narrators, and corrupted texts that evade standard sentence-level filters.
- **SOURCE TYPE:** Academic and scientific research (Preprint & Shared Task Corpus)
- **SOURCE:** "HalluTruthQA: A Fine-Grained Benchmark for Hallucination Detection, Localization, and Explanation in Arabic Question Answering" (arXiv:2607.20219) & "HalluTruthQA-4K: A Fine-Grained Corpus and Annotation Process for Arabic Hallucination Detection and Truth Verification" (arXiv:2608.03966).
- **URL:** https://arxiv.org/abs/2607.20219
- **DATE:** 2026-07 / 2026-08
- **TARGET USER / POPULATION:** Arabic-speaking researchers, students, and general users seeking factual religious and historical knowledge.
- **GEOGRAPHY:** MENA / Global Arabic-speaking community
- **LANGUAGE:** Arabic
- **DIRECT OR INDIRECT:** Direct empirical corpus analysis and annotation of LLM outputs.
- **PRIMARY OR SECONDARY:** Primary benchmark and evaluation study.

## KEY EVIDENCE
1. **Fine-Grained Span-Level Annotation:** HalluTruthQA-4K provides 4,000 expert-curated Arabic QA instances across four knowledge-intensive domains: Islamic knowledge, history, science, and geography.
2. **Character- and Span-Level Localization:** The study establishes that Arabic hallucinations cannot be adequately detected using binary response-level classifiers. In religious texts, hallucinations are localized to specific tokens (e.g., an altered narrator name in an *isnad*, an altered preposition changing a legal ruling in a *matn*, or a fabricated book title).
3. **The "Illusion of Eloquence":** The benchmark documents that Arabic LLMs generate linguistically sophisticated, grammatically impeccable classical Arabic (*Fusha*) that creates an illusion of authoritative scholarly knowledge while asserting entirely fabricated facts.
4. **Human Explanation Requirement:** Automated evaluation metrics correlate poorly with human expert explanations of religious errors, highlighting the necessity of domain-specific ground truth and scholarly verification pipelines.

## LIMITATIONS
- Encompasses four domains (Islamic knowledge is one of four); specific hadith chain mechanics are analyzed alongside general Arabic historical facts.

## CONTRADICTING / DISCONFIRMING EVIDENCE
- Newer fine-grained hallucination detectors trained on span-level data achieve higher detection recall than general-purpose toxicity or alignment filters.

## STRENGTH & CONFIDENCE
- **STRENGTH:** Strong (4,000 expert-curated items, fine-grained span annotations, Arabic-native focus).
- **CONFIDENCE IN INTERPRETATION:** High.
