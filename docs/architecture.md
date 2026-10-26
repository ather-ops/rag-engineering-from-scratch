# Capstone Architecture

PDF/TXT → extraction with page metadata → normalization → metadata-preserving chunking → embeddings → local vector index → top-k retrieval → optional reranking → grounded generation → cited answer or abstention → evaluation and error analysis.

## Constraints
- Local-first and CPU-friendly where practical.
- CLI before UI; correctness before polish.
- Preserve source metadata through every stage.
- Keep ingestion, retrieval, generation, and evaluation independently testable.
- A fluent answer is not necessarily correct.

## Questions to revisit
- Which extraction issues damage retrieval?
- What chunk size/overlap works for this corpus?
- Does reranking measurably help?
- When should the system abstain?
- What are the security and privacy boundaries?
