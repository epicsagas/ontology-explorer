# The Ontology Lineage / 온톨로지 계보

From Aristotle's categories to ontology-constrained LLMs in 2026 — 2,300 years of
ontology research on one static page: the lineage timeline, theoretical
foundations, LLM/GraphRAG/knowledge-engine synthesis, an integrated reference
architecture, a five-stage learning route, and a browser for all 425 papers.

- **[English](https://epicsagas.github.io/ontology-explorer/en/)**
- **[한국어](https://epicsagas.github.io/ontology-explorer/)**

## How it was built

All 425 papers were collected, organized, gap-analyzed, and rated with
[research-agent](https://github.com/epicsagas/research-agent) — a personal
long-term research assistant that indexes arXiv / Semantic Scholar / local PDFs
into SQLite with full-text search, tracks a topic hierarchy, and runs LLM
knowledge-gap analysis and report generation. The initial survey logged 9
research gaps; a follow-up collection closed 8 of them, and this site presents
the closure ledger alongside the one problem that remains open.

## Stack

Static site — one HTML file per language plus `data/papers.json` (exported from
the research-agent DB). No framework, no build step, no backend.

## Local preview

```bash
python3 -m http.server 8899
# http://localhost:8899 (한국어) · http://localhost:8899/en/ (English)
```
