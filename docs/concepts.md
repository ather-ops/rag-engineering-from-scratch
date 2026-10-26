# Concepts Notebook

Add short, original definitions and examples as you learn.

- **RAG:** retrieve external evidence and supply it to a language model to help answer a query.
- **Corpus:** source documents available for retrieval.
- **Chunk:** smaller text segment indexed and retrieved as a unit.
- **Embedding:** numeric vector representing content for similarity comparison.
- **Vector index:** structure for finding vectors similar to a query vector.
- **Top-k:** k highest-ranked candidates returned by retrieval.
- **Reranking:** score candidates again with a potentially stronger, more expensive relevance model.
- **Grounding:** constrain an answer to supplied evidence.
- **Faithfulness:** whether answer claims are supported by evidence.
- **Abstention:** explicitly report that evidence is insufficient.

## Failure taxonomy
1. Extraction  2. Chunking  3. Embedding/indexing  4. Retrieval/ranking  5. Context assembly  6. Generation  7. Evaluation.
