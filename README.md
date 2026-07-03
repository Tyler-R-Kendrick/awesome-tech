# awesome-tech

## Overview

`awesome-tech` is a curated knowledge repository for agentic AI tooling, practices, and infrastructure. It is organized as a lightweight, standards-driven wiki: each category folder contains a `README.md` table of contents, and repository-wide documentation follows the standards in [`standards/README.md`](./standards/README.md).

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

The root [`AGENTS.md`](./AGENTS.md) captures the repository-wide awesome-index standards, writing style, and enforcement checks, and each category folder has its own `AGENTS.md` with folder-specific guidance. Before adding or changing content, read [`standards/README.md`](./standards/README.md), the relevant folder's `AGENTS.md`, and [`llama-parse/README.md`](./llama-parse/README.md). Pull requests should explain how the documentation continues to satisfy these standards.

## How to Use This Project

1. **Start with the standards.** Review the repository standards so that you understand the expected documentation shape, indexing path, and contribution requirements.
2. **Choose a capability area.** Use the navigation table below to open the category that matches your task, such as tracing, evals, harnesses, optimization, or prompt engineering.
3. **Read the category README.** Each category README is a table of contents for that area and should remain the entry point for resources in that folder.
4. **Add or update resources.** Place new resources in the most relevant category. If a new capability area is needed, add a new folder with its own `README.md` table of contents and link it from this root README.
5. **Prepare for ingestion.** Ensure documentation is clear, structured, and compatible with the LlamaParse Cloud Index v2 requirement before indexing or retrieval workflows consume it.

## How to Connect New Work to the Repository Standards

When contributing a new document, resource list, or category:

- Use descriptive headings that make the document easy for humans and LLMs to scan.
- Keep category READMEs focused on navigation and resource discovery.
- Prefer short, factual entries over long unstructured notes.
- Link related repository pages with relative links.
- Make the root README and the relevant category README discover the new content.
- Follow the folder's `AGENTS.md` for category-specific structure and enforcement.
- Use LlamaParse Cloud Index v2 for ingestion/indexing work rather than adding a separate parsing path.
- Document standards compliance in the pull request summary.

## Navigation

| Area | Purpose |
| --- | --- |
| [Repository Standards](./standards/README.md) | Required documentation, indexing, and contribution standards. |
| [LlamaParse Cloud Index v2 Setup](./llama-parse/README.md) | Required setup and policy for parsing and indexing repository content. |
| [Agent Harness](./agent-harness/README.md) | Harnesses and meta-harnesses for running or evaluating agents. |
| [Agent Isolation](./agent-isolation/README.md) | Tools and approaches for isolating, governing, or sandboxing agent behavior. |
| [Agent Evals](./agent-evals/README.md) | Evaluation tools and frameworks for measuring agent behavior. |
| [Agent Tracing](./agent-tracing/README.md) | Tracing and observability resources for agent workflows. |
| [Agent Optimization](./agent-optimization/README.md) | Frameworks and techniques for improving agent performance. |
| [Agent Skill Optimizations](./agent-skill-optimizations/README.md) | Skill-level optimization methods and references. |
| [Token Optimization](./token-optimization/README.md) | Prompt-compression and context-reduction techniques for lowering token cost. |
| [Generative UI (GenUI)](./genui/README.md) | Frameworks and specs for agent- and model-generated interactive interfaces. |
| [Prompt Engineering](./prompt-engineering/README.md) | Prompting tools, frameworks, and structured generation references. |

## Repository Map

```text
awesome-tech/
├── README.md                          # Root project guide and navigation
├── AGENTS.md                          # Repo-wide awesome-index standards and enforcement
├── standards/                         # Required repository standards
├── llama-parse/                       # Required ingestion/indexing setup
├── agent-harness/                     # Agent harness resources
├── agent-isolation/                   # Agent isolation resources
├── agent-evals/                       # Agent evaluation resources
├── agent-tracing/                     # Agent tracing resources
├── agent-optimization/                # Agent optimization resources
├── agent-skill-optimizations/         # Agent skill optimization resources
├── token-optimization/                # Token optimization resources
├── genui/                             # Generative UI (GenUI) resources
└── prompt-engineering/                # Prompt engineering resources
```

Each category folder contains a `README.md` index and an `AGENTS.md` with folder-scoped standards.

## Contribution Checklist

Use this checklist before opening a pull request:

- [ ] The root README links to any new category or top-level documentation.
- [ ] The relevant category README includes the new resource or page.
- [ ] The change follows LLM Wiki 2.0 and Open Knowledge formatting expectations.
- [ ] The change follows the repository and folder-scoped `AGENTS.md` guidance.
- [ ] Ingestion or indexing plans use LlamaParse Cloud Index v2.
- [ ] The pull request explains standards compliance and any navigation changes.
