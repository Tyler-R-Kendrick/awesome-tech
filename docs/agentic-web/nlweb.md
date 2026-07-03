# NLWeb

An open project from Microsoft that simplifies building conversational, natural-language interfaces for websites. NLWeb lets a publisher turn a site's existing structured and semi-structured content into an AI-queryable app for both people and agents, and — because every instance is also a Model Context Protocol (MCP) server — exposes that content to the agent ecosystem. It was announced at Microsoft Build on 19 May 2025 and is positioned as playing "a similar role to HTML for the agentic web"; the reference repository frames it as "NLWeb is to MCP/A2A what HTML is to HTTP."

## Contents

- [nlweb-ai/NLWeb](https://github.com/nlweb-ai/NLWeb) - Canonical Python reference implementation, MIT-licensed (transferred from the `microsoft` org, which now redirects here).
- [nlweb.ai/docs](https://nlweb.ai/docs/intro) - Official documentation site.
- [NLWeb Specification](https://nlweb.ai/docs/specification) - Versioned protocol specification (v0.55 as of this writing).
- [Introducing NLWeb](https://news.microsoft.com/source/features/company-news/introducing-nlweb-bringing-conversational-interfaces-directly-to-the-web/) - Microsoft newsroom announcement with goals and launch collaborators.
- [Microsoft Build 2025: the open agentic web](https://blogs.microsoft.com/blog/2025/05/19/microsoft-build-2025-the-age-of-ai-agents-and-building-the-open-agentic-web/) - Official Build 2025 blog introducing NLWeb.

## How it works

- **Reuses existing structured data.** NLWeb builds on formats sites already publish — Schema.org, RSS, and JSONL — and adds an LLM-powered natural-language layer, so publishers who already mark up their content can add a conversational interface without re-modeling their data.
- **Two endpoints: `/ask` and `/mcp`.** A site exposes `/ask` for its natural-language query interface and `/mcp` for the same capability formatted for MCP clients. Per the README, "every NLWeb instance also acts as an MCP server (and soon A2A)," with `ask` as the core method; `/mcp` also implements the standard `list_tools`, `list_prompts`, `call_tool`, and `get_prompt` methods.
- **Structured, Schema.org responses.** The `ask` method returns JSON containing a `results` array whose items carry `url`, `name`, `site`, `score`, an LLM-generated `description`, and a `schema_object` encoded in Schema.org — so answers are structured rather than free-text prose. Query modes are `list` (default), `summarize`, and `generate` (traditional RAG).
- **Stateless retrieval pipeline.** The included implementation keeps no server-side state (conversation context is passed back with each request); a query is first decontextualized via parallel LLM calls, retrieved from a vector database, then scored and snippeted by further LLM calls.
- **Bring-your-own model and store.** The reference implementation ships connectors for multiple LLM providers (OpenAI, DeepSeek, Gemini, Anthropic, Inception, Hugging Face) and vector databases (Qdrant, Snowflake, Milvus, Azure AI Search, Elasticsearch, Postgres, Cloudflare AutoRAG), plus data-ingestion tooling and a sample UI.

## Origin and vision

- Conceived and led by **R.V. Guha** — Microsoft CVP and Technical Fellow, and creator of RSS, RDF, and Schema.org.
- Stated goal: to be "the fastest and easiest way to effectively turn your website into an AI app," with the "HTML for the agentic web" framing that any publisher can add an intelligent natural-language experience the way HTML let anyone publish a page.

## Ecosystem

Initial publishing and ecosystem collaborators named in the announcement are Chicago Public Media, Common Sense Media, DDM (Allrecipes, Serious Eats), Eventbrite, Hearst (Delish), Inception Labs, Milvus, O'Reilly Media, Qdrant, Shopify, Snowflake, and Tripadvisor; Cloudflare separately productized NLWeb with its AutoRAG service. O'Reilly's deployment offers conversational search over roughly 59,000 books using Schema.org metadata without web crawling.

## Footnotes

- License is MIT (copyright Microsoft Corporation); the repository is under active development and publishes no tagged releases, while the protocol itself is versioned separately (spec v0.55) — pin to a specific commit for reproducible builds.
- Responses are described as "JSON using Schema.org" via a `schema_object` field; primary sources do not use the term "JSON-LD."
- NLWeb sits on the content-access side of the agentic web (making a site's data answerable), complementary to in-page control agents such as [PageAgent](./page-agent.md). See also [MCP](../standards/mcp.md) and [A2A](../standards/a2a.md).
