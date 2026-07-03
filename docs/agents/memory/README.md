# Agent Memory

A curated index of frameworks and services that give AI agents persistent, long-term, episodic, semantic, and working memory across sessions.

## Contents

- [Mem0](./mem0.md) - Universal memory layer that adds persistent, personalized long-term memory to agents across vector, key-value, and graph stores.
- [Letta (formerly MemGPT)](https://github.com/letta-ai/letta) - Framework for building stateful agents with self-editing long-term memory and tiered context management.
- [Zep](https://github.com/getzep/zep) - Memory service that builds a temporal knowledge graph from conversations and documents for cross-session context.
- [Graphiti](https://github.com/getzep/graphiti) - Framework for building real-time, temporally-aware knowledge graphs that serve as evolving agent memory.
- [Cognee](https://github.com/topoteretes/cognee) - AI memory platform that turns ingested data into a self-hosted knowledge graph for persistent memory across sessions.
- [LangMem](https://github.com/langchain-ai/langmem) - LangChain SDK providing semantic, episodic, and procedural long-term memory tools with native LangGraph store integration.
- [MemOS](https://github.com/MemTensor/MemOS) - Memory operating system for LLMs and agents that unifies storage, retrieval, and management through a MemCube abstraction.
- [MemoryOS](https://github.com/BAI-LAB/MemoryOS) - Memory operating system for personalized agents using a hierarchical storage, updating, retrieval, and generation architecture.
- [A-MEM](https://github.com/agiresearch/A-mem) - Agentic memory system that dynamically organizes and links memories using Zettelkasten-inspired notes.
- [Memary](https://github.com/kingjulio8238/Memary) - Memory layer for autonomous agents that emulates human memory with a knowledge-graph-backed store.
- [Redis Agent Memory Server](https://github.com/redis/agent-memory-server) - Redis-backed server providing working and long-term memory with semantic, keyword, and hybrid search plus MCP integration.
- [AutoMem](https://github.com/autoLearnMem/AutoMem) - Framework that treats memory management as a trainable skill, using automated optimization loops to improve both the memory structure (prompts, file schemas, action vocabulary) and the model's memory proficiency on long-horizon agent tasks.

## Footnotes

- [MemGPT paper](https://arxiv.org/abs/2310.08560) - Foundational research introducing OS-inspired virtual context management and tiered memory for LLM agents, the basis for Letta.
- [AutoMem paper](https://arxiv.org/abs/2607.01224) - Stanford research (Wu et al., 2026) framing memory management as a trainable metamemory skill; it automates two loops, one revising the memory structure from full-trajectory reviews and one training the model's memory proficiency from its own good memory decisions, with a [project site](https://autolearnmem.github.io/).
- AutoMem is indexed here as an agent-memory system but treats memory as a trainable skill rather than fixed infrastructure, linking this scope to [agent skill optimization](../skills/README.md); it promotes file-system operations to first-class memory actions and reports roughly 2x-4x gains from optimizing memory alone on long-horizon games (Crafter, MiniHack, NetHack).
- MemOS (MemTensor) and MemoryOS (BAI-LAB) are distinct, separately maintained projects with similar names.
