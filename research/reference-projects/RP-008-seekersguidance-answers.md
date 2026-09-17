# [RP-008] SeekersGuidance Answers Service

---

## 1. Classification
- **Category:** DIRECT COMPETITOR (for traditional Sunni Q&A) / HUMAN SERVICE BASELINE / UX REFERENCE
- **Related Problem Cards:** `P-002`, `P-101`, `P-102`, `P-301`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Project Name:** SeekersGuidance Answers (Global Islamic Seminary & Fatwa Service)
- **Organization / Creator:** SeekersGuidance (The Global Islamic Seminary), founded by Shaykh Faraz Rabbani.
- **Official URL:** https://seekersguidance.org/answers
- **Launch Date:** 2008
- **Current Status:** Active, respected global institution, non-profit / donor-supported.
- **Country / Region:** Canada / International (scholars across Canada, UK, US, Jordan, Turkey).
- **Primary Language(s):** English (primary), with answers rooted in classical Arabic texts.

---

## 3. Target User & Use Case
- **Primary User:** English-speaking Muslims seeking traditional, mainstream Sunni answers adhering to the four orthodox madhahib (specifically Hanafi, Shafi'i, and Maliki), with a strong pastoral, non-judgmental, and spiritually nurturing tone.
- **Core Job:** "Ask a practical religious question and receive a measured, scholar-reviewed answer grounded in traditional jurisprudence that accounts for Western living contexts and personal spiritual wellbeing."

---

## 4. Key Capabilities & Technical Approach
1. **Scholar-Reviewed Answers Archive:** Thousands of published Q&A articles answering practical everyday life dilemmas.
2. **Madhhab-Explicit Categorization:** Answers explicitly state which legal school is being cited (e.g., "Answered according to the Hanafi School by Shaykh Faraz Rabbani").
3. **Pastoral & Psychological Nuance:** Answers actively counteract religious scrupulosity (*waswas*), explicitly advising anxious questioners on purity and prayer doubts to disregard unfounded misgivings.
4. **Contextual Balance for Converts:** Explicitly addresses convert family dilemmas (e.g. attending Christmas or Thanksgiving family dinners with non-Muslim parents, ruling it permissible with proper decorum and boundaries).
5. **Technical Implementation:** WordPress / Custom CMS; search powered by Algolia / standard WP search.

---

## 5. What It Does Well
1. The premier counter-balance to IslamQA's rigidity in the English-speaking world.
2. Direct preservation of the four classical Sunni madhahib.
3. Excellent pastoral counseling for individuals suffering from religious scrupulosity (*waswas*).

---

## 6. Known Limitations & Workflow Friction
1. **Severe Submission Latency & Backlog:** Because every question is routed to human scholars, response turnaround times for new questions frequently take 4 to 12 weeks, or submissions are closed due to backlog (`P-002`, `P-101`).
2. **Search Discovery Friction:** The website search engine is notoriously difficult to navigate. Users looking for an exact answer frequently encounter irrelevant course listings or blog posts instead of the specific fatwa.
3. **Weak Comparative View:** An answer is usually written from the perspective of one madhhab (e.g., Hanafi). If a Shafi'i or Maliki user reads it, they must independently search whether their school differs.
4. **Poor SEO Dominance Compared to IslamQA:** In Google search rankings, SeekersGuidance is frequently buried on page 2 or 3 beneath IslamQA.info.

---

## 7. Strength Against Our Problem Space
- `P-002`: Solves the pastoral tone and scrupulosity issue, but fails on latency and comparative multi-madhhab indexing.
- `P-101`: Best existing human guidance for converts, but discovery friction and submission delays prevent it from solving real-time family crises.
- `P-301`: Provides an ideal benchmark for how qualified human scholars handle nuance and abstention, contrasting sharply with LLM overconfidence.
