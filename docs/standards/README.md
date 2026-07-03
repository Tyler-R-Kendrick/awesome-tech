# Standards

Standards that govern this repository's documentation, and the agent and interoperability standards this project tracks.

## Contents

- [Required Standards](#required-standards) - Required knowledge formats for repository documents.
- [Awesome-Index Structure](#awesome-index-structure) - Markdown structure used by repository indexes.
- [Enforcement](#enforcement) - Checks and expectations for repository changes.
- [Indexing Requirement](#indexing-requirement) - Required parsing and indexing workflow.
- [Communication and Interoperability](#communication-and-interoperability) - Agent discovery, communication, and coordination protocols.
- [Payments and Commerce](#payments-and-commerce) - Agent payment and commerce protocols.

## Required Standards

All repository documents **must** follow:

1. **LLM Wiki 2.0 (LangChain standard)**
2. **[Open Knowledge format (Google standard)](../documentation/okf.md)**

## Awesome-Index Structure

- Use `## Contents` for index navigation; do not use `## Table of Contents` in awesome indexes.
- Root and category indexes should start with a `#` title and a concise scope description.
- Keep Contents shallow and focused on the most important sections or resources.
- Prefer verified Markdown links with short descriptions for curated resources.
- Descriptions should be neutral, concise, and end with a period.
- Place secondary notes in `## Footnotes` only when needed, and keep that section out of Contents.

## Enforcement

- New and updated documentation must conform to both required standards above.
- Pull requests should describe how changes satisfy both standards.
- Category folders must keep a `README.md` that acts as a curated contents index.
- Every folder scope should include an `AGENTS.md` file with standards and focus-area guidance.
- The `README.md` and `AGENTS.md` folder-structure rules above are enforced automatically by [Konsistent](https://www.npmjs.com/package/konsistent), a structural-convention linter configured in [`konsistent.json`](../../konsistent.json). Run `bun run konsistent` locally; continuous integration runs it on every pull request.
- Run `git diff --check` and `rg "^## Table of Contents"` before committing documentation changes.

## Indexing Requirement

All repository ingestion/indexing work must use:

- **LlamaParse Cloud Index v2**
- Getting started guide: <https://developers.llamaindex.ai/llamaparse/cloud-index-v2/getting_started/>
- Repository setup and policy: [`../prompt-engineering/rag/llama-parse/README.md`](../prompt-engineering/rag/llama-parse/README.md)

## Communication and Interoperability

Open standards for agent discovery, communication, and coordination that this repository tracks:

- [Model Context Protocol (MCP)](./mcp.md) - Standard for connecting AI applications to tools, data, and workflows.
- [Agent Communication Protocol (ACP)](./acp.md) - IBM/BeeAI protocol for agent communication, now converged with A2A.
- [Agent2Agent Protocol (A2A)](./a2a.md) - Standard for cross-framework agent discovery and coordination.
- [Agentic Resource Discovery (ARD)](./ard.md) - Runtime discovery layer for finding tools, skills, and agents across federated registries.
- [Agent-to-Human Protocol (A2H)](./a2h.md) - Twilio protocol for channel-agnostic, auditable agent-to-human communication.

## Payments and Commerce

Open standards for agent-led payments and commerce that this repository tracks:

- [x402 Payment Protocol](./x402.md) - HTTP 402-based programmatic payments for agents and APIs.
- [Agent Payments Protocol (AP2)](./ap2.md) - Google protocol for secure, mandate-based agent payments, built as an A2A extension.
- [Universal Commerce Protocol (UCP)](./ucp.md) - Google standard for agent-driven commerce across discovery, checkout, and order management.
