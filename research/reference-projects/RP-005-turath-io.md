# [RP-005] Turath.io (Modern Digital Islamic Heritage Suite)

---

## 1. Classification
- **Category:** DIRECT COMPETITOR (for modern classical Islamic reading & search) / TECHNICAL REFERENCE / UX REFERENCE
- **Related Problem Cards:** `P-200`, `P-202`, `P-301`, `P-302`
- **Research Owner:** Agent 05 — Market & Reference Landscape Researcher
- **Review Date:** 2026-09-17
- **Last Updated:** 2026-09-17

---

## 2. Basic Information
- **Project Name:** Turath.io (تراث) / Turath AI
- **Organization / Creator:** Nuqayah / Ragaeeb (Independent developer & researcher collective led by open-source contributors).
- **Official URL:** https://app.turath.io / https://turath.ai
- **Repository URL:** https://github.com/ragaeeb/turath-sdk , https://github.com/nuqayah
- **Documentation URL:** https://turath.io
- **Launch Date:** ~2021 (Web app); Turath AI (~2024–2025)
- **Current Status:** Active, growing rapidly among modern students of knowledge and researchers.
- **Country / Region:** International / Open-source distributed.
- **Primary Language(s):** Classical Arabic; English interface elements.

---

## 3. Target User & Use Case
- **Primary User:** Modern Arabic-literate researchers, tech-savvy students of Islamic knowledge, educators, and software engineers building Islamic applications.
- **Core Job:** "Search, browse, read, and cross-reference thousands of classical Islamic books on the web and mobile with a modern, fast, Notion-like user experience, and query sources via AI."

---

## 4. Key Capabilities & Technical Approach
1. **Modernized Shamela Corpus on Web:** Re-indexes thousands of classical Shamela volumes into a clean, cloud-hosted, mobile-responsive web application.
2. **Instant As-You-Type Search:** Highly optimized search engine delivering sub-second results across millions of pages with root/morphological awareness.
3. **Turath AI Integration:** Connects classical books to retrieval-augmented generative AI (Turath AI) for querying classical sources with footnotes.
4. **Developer Ecosystem:** Provides public JavaScript SDK (`ragaeeb/turath-sdk`) and open APIs for third-party developers to interact with classical book texts programmatically.
5. **Clean Reader UX:** Typography-first reading experience with customizable Arabic fonts, diacritics toggle, book table-of-contents navigation, and instant copy with citation.

---

## 5. What It Does Well
1. Solves the archaic Windows desktop UI limitation of Maktabah Shamela, bringing classical Arabic research to web, Mac, Linux, and mobile browsers.
2. Ultra-fast, clean, and distraction-free typography.
3. Pioneer in attempting to bridge classical Islamic corpora with modern AI and developer APIs.

---

## 6. Known Limitations & Workflow Gaps
1. **Monolingual Focus:** Primarily indexes Arabic classical texts; does not solve English cross-lingual semantic matching (`P-001`).
2. **Raw AI Hallucination Vulnerability in Turath AI:** Like other LLM-based assistants, Turath AI still suffers from generative paraphrasing errors and occasional misattribution when synthesizing classical opinions.
3. **No Isnad Network Visualization:** Lacks transmission chain graph visualization and cross-scholar consensus barometers (`P-200`, `P-302`).
4. **No Direct CAT Integration:** Cannot be plugged into Trados, Word, or translation pipelines for translators (`P-202`).

---

## 7. Strength Against Our Problem Space
- `P-200`: Greatly speeds up Arabic text browsing for tech-savvy imams, but still leaves the khutbah drafting and consensus synthesis manual.
- `P-300`: Emerging reference for how RAG is applied to classical Arabic texts, but demonstrates the persistent hallucination risk in production.
- `P-302`: Strong partial solver for web access to Shamela, but still does not unify Dorar.net authentication verdicts, isnad trees, and English translations.
