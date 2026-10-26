# Day 1 — Understand RAG and define the baseline

**Goal:** explain RAG in your own words and draw its pipeline before building a framework-heavy implementation.

## 15 min — Recall
Without searching, answer: What problem does a language model have with private or updated documents? What is retrieval? Why can retrieved context still fail to produce a correct answer?

## 20 min — Focused reading
Read the introductory RAG section in your chosen handbook. Write original notes about retrieval, generation, and what should happen when useful evidence is absent. Do not copy book pages into this public repository.

## 45 min — Paper baseline
Create one short synthetic source document, two questions answerable from it, and one unanswerable question. Record the expected evidence for each. Draw the pipeline in `docs/architecture.md` or your own notes. No embeddings or LLM are required today.

## 10 min — Log
- My definition of RAG:
- Pipeline stages:
- Expected evidence for each question:
- Expected response to the unanswerable question:
- One thing I do not yet understand:

## Checklist
- [ ] Explain RAG without reading a definition.
- [ ] Draw the pipeline.
- [ ] Create a tiny question set with expected evidence.
- [ ] Record one uncertainty.
