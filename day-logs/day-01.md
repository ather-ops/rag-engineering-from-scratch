# Day 1 — Understand RAG and define the baseline

**Goal:** explain RAG in your own words and draw its pipeline before building a framework-heavy implementation.

## 15 min — Recall

- **Why new documents usually do not require LLM retraining:** process the new document and add its content to the retrieval collection. The language model's parameters normally stay unchanged.
- **What retrieval does:** finds potentially relevant information from an available collection. A vector database is one possible retrieval mechanism, not the definition of retrieval itself.
- **Why retrieval can still fail:** a relevant-looking passage may not contain the answer, and a model may misinterpret or go beyond the evidence.

## 20 min — Focused reading

Write original notes about retrieval, generation, and what should happen when useful evidence is absent. Do not copy book pages into this public repository.

## 45 min — Paper baseline

### Synthetic source document: Assignment Policy

> Assignment 2 must be submitted by 5 November 2026.
>
> Students may submit assignments through the university portal.
>
> Late submissions require approval from the course instructor.

### Test questions and expected evidence

1. **Question:** When is Assignment 2 due?
   - **Expected answer:** 5 November 2026.
   - **Expected evidence:** “Assignment 2 must be submitted by 5 November 2026.”
   - **Result of paper review:** Answerable from the source.

2. **Question:** Where should assignments be submitted?
   - **Expected answer:** Through the university portal.
   - **Expected evidence:** “Students may submit assignments through the university portal.”
   - **Result of paper review:** Answerable from the source.

3. **Question:** What is the examination date?
   - **Expected evidence:** None. The source document does not state an examination date.
   - **Expected behavior:** “Sorry, the available documents do not contain information about the examination date.”
   - **Result of paper review:** Unanswerable from this source; the system should not invent a date.

### Day 1 pipeline understanding

Source documents → ingestion and text preparation → chunking → indexing → retrieval → evidence-grounded generation → answer with supporting evidence, or acknowledge that evidence is missing.

A similarity threshold can help reject low-scoring results, but a high similarity score alone does not prove that a passage supports the answer. Prompting can encourage grounded answers, but it cannot guarantee correctness or replace missing evidence.

## 10 min — Log

- **My definition of RAG:** A system that retrieves potentially relevant information from a document collection and uses that context to help generate an answer.
- **Pipeline stages:** Ingestion/preparation, chunking, indexing, retrieval, grounded generation, and answering with evidence or acknowledging missing evidence.
- **Expected evidence for each question:** See the three baseline tests above.
- **Expected response to the unanswerable question:** State that the available source does not contain the examination date; do not guess.
- **One thing I do not yet understand:** How should a system distinguish a passage that is semantically similar to a question from a passage that actually contains enough evidence to answer it?

## Checklist

- [x] Explain RAG without reading a definition.
- [ ] Draw the pipeline in docs/architecture.md or personal notes.
- [x] Create a tiny question set with expected evidence.
- [x] Record one uncertainty.
