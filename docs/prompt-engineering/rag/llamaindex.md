# LlamaIndex

Open-source (MIT) data and agent framework for building context-augmented LLM applications, maintained as `run-llama/llama_index` and available in Python and TypeScript. LlamaIndex connects custom and enterprise data to LLMs through three primitives: **data connectors** that ingest existing sources and formats (APIs, PDFs, documents, SQL, and more), **indices** that structure that data for efficient lookup, and a **retrieval/query interface** that turns a prompt into retrieved context plus a knowledge-augmented answer. This makes it a core building block for retrieval-augmented generation, and it integrates with application frameworks such as LangChain, Flask, and Docker.

Beyond retrieval, LlamaIndex ships agent primitives and **Workflows** — an event-driven, async-first, step-based way to orchestrate multi-step processes that combine retrieval, tools, and one or more agents. Its managed cloud, **LlamaCloud**, packages the harder document work as services: Parse (agentic OCR and document parsing), Extract (structured data extraction), Index (managed ingestion and RAG pipelines), Split (document segmentation), and Agents (end-to-end document agents built on Workflows). The project now describes itself as a document-agent and OCR platform, reflecting its focus on turning messy documents into agent-ready data.

## Contents

- [run-llama/llama_index](https://github.com/run-llama/llama_index) - Source repository (MIT) for the core framework.
- [llamaindex.ai](https://www.llamaindex.ai/llamaindex) - Framework overview and LlamaCloud services.
- [Developer documentation](https://developers.llamaindex.ai/) - Guides and API reference for Python and TypeScript.
- [Workflows](https://www.llamaindex.ai/workflows) - Event-driven multi-step and multi-agent orchestration.

## Footnotes

- The core framework is MIT-licensed and free; LlamaCloud is a managed service with a free tier and paid production tiers.
- Repository ingestion in this project uses LlamaParse (part of LlamaCloud) via the required [LlamaParse Cloud Index v2 setup](./llama-parse/README.md); LlamaIndex is the parent framework behind that parser.
- Indexed here as a RAG framework; see the [RAG index](./README.md) for retrievers, techniques, and evaluation tools that complement it.
