# Mem0

Universal memory layer for AI agents, open-source under Apache-2.0 (`mem0ai/mem0`). Mem0 extracts and consolidates the salient facts from conversations and interactions into structured, long-term memories that agents retrieve on demand, so an assistant remembers user preferences, prior decisions, and context across sessions instead of restarting cold each time. It exposes a simple add/search API and provides **multi-level memory** that retains User, Session, and Agent state with adaptive personalization.

Under the hood Mem0 uses a hybrid store — vector storage for semantic recall, a graph store for structured entity relationships, and key-value storage for exact-match lookups — with multi-signal retrieval that fuses semantic similarity, keyword search, and entity matching into a single ranked result. It ships in three forms: an open-source library (`pip`/`npm`) for embedding memory directly, a self-hostable server (Docker), and a fully managed cloud platform. **OpenMemory** is Mem0's local-first, MCP-based memory server that gives MCP-compatible tools — such as Claude Desktop, Cursor, and Windsurf — a shared, persistent memory that stays on the user's machine.

## Contents

- [mem0ai/mem0](https://github.com/mem0ai/mem0) - Source repository (Apache-2.0) and quickstart.
- [mem0.ai](https://mem0.ai/) - Product site and managed cloud platform.
- [Documentation](https://docs.mem0.ai/) - Guides, API reference, and SDKs.
- [Open-source overview](https://docs.mem0.ai/open-source/overview) - Self-hosted library and server setup.

## Footnotes

- Mem0 is offered as both open-source (Apache-2.0 library and server) and a separately priced hosted platform; choose based on whether memory should stay in your infrastructure or be managed.
- [OpenMemory](https://github.com/mem0ai/mem0) is the local-first, MCP memory server component; it connects Mem0 to the [Model Context Protocol](../../standards/mcp.md) so memory is portable across MCP hosts.
- Mem0 reports a rewritten memory algorithm (2026) with gains on long-conversation benchmarks such as LoCoMo and LongMemEval; treat the specific figures as vendor-reported and verify against the current documentation.
- Indexed alongside sibling memory frameworks in this folder; see the [memory index](./README.md) for alternatives with different storage and retrieval trade-offs.
