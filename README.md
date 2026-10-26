# RAG Engineering from Scratch

A 30-day hands-on journey to understand, build, evaluate, and improve a Retrieval-Augmented Generation (RAG) system from first principles.

**Capstone:** a local-first knowledge assistant that answers questions from PDF/text documents with source references and abstains when evidence is insufficient.

## Roadmap
- **Days 1–5:** RAG fundamentals, failure modes, baseline, prompting
- **Days 6–10:** document ingestion, metadata, chunking
- **Days 11–15:** embeddings, vector index, retrieval
- **Days 16–20:** reranking and grounded generation
- **Days 21–26:** evaluation, monitoring, controlled optimization
- **Days 27–30:** regression tests, security, documentation, demo

## Daily routine (90 minutes)
15 min recall · 20 min focused reading · 45 min implementation/experiments · 10 min progress log.

## Start here
1. Read `docs/learning-roadmap.md`.
2. Complete `day-logs/day-01.md`.
3. Review `docs/architecture.md` and `docs/concepts.md`.

## Setup
Python 3.11+ recommended.
```bash
git clone https://github.com/ather-ops/rag-engineering-from-scratch.git
cd rag-engineering-from-scratch
python -m venv .venv
```
Activate using `.venv\\Scripts\\Activate.ps1` (Windows PowerShell) or `source .venv/bin/activate` (macOS/Linux), then run `code .`.

Keep early stages lightweight and CPU-friendly. Never commit secrets, private documents, or copyrighted handbook pages. Commit original notes, code, and synthetic examples.

**North star:** build understanding first, then build a system whose behavior you can explain and measure.
