# 30-Day Learning Roadmap

## Days 1–5 — Understand the problem
1. Define RAG; draw the pipeline; write questions and expected evidence.
2. Separate retrieval failures from generation failures.
3. Create a tiny synthetic corpus with known answers.
4. Explore grounding and abstention when evidence is missing.
5. Run a baseline and classify failures.

## Days 6–10 — Prepare documents
6. Inspect PDF/text extraction and layout issues.
7. Extract text while preserving document/page metadata.
8. Implement fixed-size chunking and overlap.
9. Compare chunk sizes on a fixed question set.
10. Compare chunk boundaries and metadata.

## Days 11–15 — Retrieval
11. Understand embeddings and similarity.
12. Embed chunks with a small suitable model.
13. Build a local vector index and inspect top-k results.
14. Evaluate hit-rate/recall at k.
15. Diagnose misses and establish a baseline.

## Days 16–20 — Grounded generation
16. Learn reranking and its trade-offs.
17. Compare candidates before and after reranking.
18. Build an evidence-only generation interface.
19. Include source/page references and a no-evidence response.
20. Integrate a CLI and test success/failure paths.

## Days 21–26 — Evaluation and optimization
21. Version the evaluation dataset.
22. Define correctness, faithfulness, and retrieval metrics.
23. Add a repeatable evaluation script.
24. Inspect concrete failures, not only aggregate scores.
25. Run one controlled optimization experiment.
26. Record latency, resource use, trade-offs, and remaining failures.

## Days 27–30 — Delivery
27. Add regression tests for previous failures.
28. Review privacy, prompt injection, document handling, and secrets.
29. Reproduce setup from a clean environment and polish the demo.
30. Present architecture, results, limitations, and next experiments.

Use `day-logs/_template.md` for each session. Reading alone does not complete a day: capture evidence of understanding or implementation.
