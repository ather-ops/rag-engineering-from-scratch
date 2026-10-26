# Capstone — Local Knowledge RAG

Ask questions over local PDF/text documents, retrieve relevant evidence, and return grounded answers with source/page references. If evidence is insufficient, say so rather than fabricate.

Stages: ingestion/extraction → metadata-preserving chunking → embeddings/local index → retrieval and optional reranking → grounded generation/citations → evaluation and regression tests.

Start CPU-friendly and local-first. No paid API is required for the first learning stages. Never commit private documents, credentials, or copyrighted source material. Correctness and observability come before UI polish.
