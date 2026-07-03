# Retrieval-Augmented Generation (RAG)

A curated index of frameworks, techniques, and evaluation tools for building retrieval-grounded LLM applications. Repository ingestion and parsing use the required LlamaParse setup.

## Contents

- [LlamaParse Cloud Index v2 Setup](./llama-parse/README.md) - Required parsing and indexing setup for repository content.
- [LangChain](https://github.com/langchain-ai/langchain) - Framework for building LLM applications and agents by composing retrievers, chains, and tool integrations.
- [LlamaIndex](https://github.com/run-llama/llama_index) - Data framework connecting custom data sources to LLMs with indexing and retrieval primitives for RAG.
- [Haystack](https://github.com/deepset-ai/haystack) - deepset's orchestration framework for building RAG pipelines, semantic search, and agents from modular components.
- [Microsoft GraphRAG](https://github.com/microsoft/graphrag) - Graph-based RAG system that builds knowledge graphs from source text to support reasoning over complex datasets.
- [RAGatouille](https://github.com/AnswerDotAI/RAGatouille) - Library for using and training late-interaction ColBERT retrieval models within RAG pipelines.
- [txtai](https://github.com/neuml/txtai) - All-in-one embeddings database for semantic search, LLM orchestration, and RAG workflows.
- [FlashRAG](https://github.com/RUC-NLPIR/FlashRAG) - Toolkit with preprocessed datasets and reproducible baselines for efficient RAG research and evaluation.
- [DSPy](https://github.com/stanfordnlp/dspy) - Framework for programming and optimizing modular LLM pipelines, including RAG, instead of hand-writing prompts.
- [Anthropic Contextual Retrieval](https://www.anthropic.com/engineering/contextual-retrieval) - Technique that prepends chunk-specific context before embedding and BM25 indexing to reduce retrieval errors.
- [RAGAS](https://github.com/explodinggradients/ragas) - Framework providing reference-free metrics for evaluating retrieval-augmented generation pipelines.

## Footnotes

- ColBERT ([stanford-futuredata/ColBERT](https://github.com/stanford-futuredata/ColBERT)) is the underlying late-interaction retrieval model behind RAGatouille.
