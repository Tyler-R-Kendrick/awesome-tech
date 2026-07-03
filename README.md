# awesome-tech

## Overview

`awesome-tech` is a curated knowledge repository for agentic AI tooling, practices, and infrastructure. It is organized as a lightweight, standards-driven wiki: all curated content lives under [`docs/`](./docs/README.md), each category folder contains a `README.md` index, and repository-wide documentation follows the standards in [`docs/standards/README.md`](./docs/standards/README.md).

Use this project to:

- Discover relevant tools and references for agent development.
- Group agentic AI resources by capability area.
- Maintain documentation that is ready for LLM-oriented retrieval, parsing, and indexing.
- Keep new contributions aligned with the repository standards before they are ingested.

## Repository Standards

All new and updated documentation must follow the repository standards:

1. **LLM Wiki 2.0 (LangChain standard)** for LLM-friendly structure, clear headings, and concise navigable sections.
2. **Open Knowledge format (Google standard)** for discoverable, reusable, and well-scoped knowledge entries.
3. **LlamaParse Cloud Index v2** for repository ingestion and indexing workflows.

The root [`AGENTS.md`](./AGENTS.md) captures the repository-wide awesome-index standards, writing style, and enforcement checks, and each category folder has its own `AGENTS.md` with folder-specific guidance. Before adding or changing content, read [`docs/standards/README.md`](./docs/standards/README.md), the relevant folder's `AGENTS.md`, and [`docs/prompt-engineering/rag/llama-parse/README.md`](./docs/prompt-engineering/rag/llama-parse/README.md). Pull requests should explain how the documentation continues to satisfy these standards.

## How to Use This Project

1. **Start with the standards.** Review the repository standards so that you understand the expected documentation shape, indexing path, and contribution requirements.
2. **Choose a capability area.** Use the navigation table below (or the [documentation index](./docs/README.md)) to open the category that matches your task, such as agents, prompt engineering, generative UI, or standards.
3. **Read the category README.** Each category README is an index for that area and should remain the entry point for resources in that folder.
4. **Add or update resources.** Place new resources in the most relevant category. If a new capability area is needed, add a new folder under `docs/` with its own `README.md` index and link it from the parent index.
5. **Prepare for ingestion.** Ensure documentation is clear, structured, and compatible with the LlamaParse Cloud Index v2 requirement before indexing or retrieval workflows consume it.

## How to Connect New Work to the Repository Standards

When contributing a new document, resource list, or category:

- Use descriptive headings that make the document easy for humans and LLMs to scan.
- Keep category READMEs focused on navigation and resource discovery.
- Prefer short, factual entries over long unstructured notes.
- Link related repository pages with relative links.
- Make the parent index and the relevant category README discover the new content.
- Follow the folder's `AGENTS.md` for category-specific structure and enforcement.
- Use LlamaParse Cloud Index v2 for ingestion/indexing work rather than adding a separate parsing path.
- Document standards compliance in the pull request summary.

## Navigation

| Area | Purpose |
| --- | --- |
| [Documentation Index](./docs/README.md) | Top-level index linking every category. |
| [Agents](./docs/agents/README.md) | Harnesses, sandboxes, optimization, skills, memory, tracing, and evals. |
| [Agentic Web](./docs/agentic-web/README.md) | Making existing websites queryable and operable by agents (NLWeb, PageAgent). |
| [Prompt Engineering](./docs/prompt-engineering/README.md) | Prompt programming, RAG, context engineering, and token optimization. |
| [Generative UI (GenUI)](./docs/genUI/README.md) | Frameworks and specs for agent- and model-generated interfaces. |
| [Documentation](./docs/documentation/README.md) | Tooling and formats for agent- and LLM-facing documentation, knowledge, and design context. |
| [Code Transformation](./docs/code-transformation/README.md) | Deterministic, recipe-based engines for automated code refactoring and migration. |
| [Standards](./docs/standards/README.md) | Documentation standards and tracked interoperability, payment, and commerce protocols (MCP, A2A, ARD, A2H, x402, AP2, UCP). |

## Repository Map

```text
awesome-tech/
├── README.md                              # Root project guide and navigation
├── AGENTS.md                              # Repo-wide awesome-index standards and enforcement
├── package.json                           # Bun manifest: Konsistent dev dependency and scripts
├── bun.lock                               # Bun lockfile pinning the toolchain
├── konsistent.json                        # Konsistent structural-convention rules for docs/
├── .github/
│   └── workflows/
│       └── konsistent.yml                 # CI: enforce structural conventions on every PR
└── docs/                                  # Curated knowledge index
    ├── README.md                          # Documentation index
    ├── agents/                            # Agent capabilities
    │   ├── harnesses/
    │   ├── sandboxes/
    │   ├── optimization/
    │   ├── skills/
    │   ├── memory/
    │   ├── tracing/
    │   └── evals/
    ├── agentic-web/                       # Agentic web: NLWeb, PageAgent
    ├── prompt-engineering/                # Prompt programming and related subtopics
    │   ├── rag/                           # Retrieval-augmented generation
    │   │   └── llama-parse/               # Required ingestion/indexing setup
    │   ├── context-engineering/
    │   └── token-optimization/
    │       └── models/                    # Model-based prompt compression
    ├── genUI/                             # Generative UI (GenUI)
    ├── documentation/                     # Agent-facing documentation tooling and knowledge formats
    ├── code-transformation/               # Deterministic code refactoring and migration engines
    └── standards/                         # Documentation and interoperability standards
```

Each category folder contains a `README.md` index and an `AGENTS.md` with folder-scoped standards.

## Contribution Checklist

Use this checklist before opening a pull request:

- [ ] The parent index links to any new category or top-level documentation.
- [ ] The relevant category README includes the new resource or page.
- [ ] The change follows LLM Wiki 2.0 and Open Knowledge formatting expectations.
- [ ] The change follows the repository and folder-scoped `AGENTS.md` guidance.
- [ ] Ingestion or indexing plans use LlamaParse Cloud Index v2.
- [ ] The pull request explains standards compliance and any navigation changes.
