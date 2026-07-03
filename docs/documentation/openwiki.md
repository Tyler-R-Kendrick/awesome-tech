# OpenWiki

An open-source agent and CLI from LangChain (announced July 2026) that generates and maintains documentation for a codebase, built specifically for agents. It writes a repository wiki, links it into agent instruction files such as `AGENTS.md` and `CLAUDE.md`, and keeps the docs current through a GitHub Action that reads git diffs since the last run. It supports multiple model providers, including OpenAI, Anthropic, OpenRouter, Fireworks, and Baseten.

## Contents

- [Introducing OpenWiki](https://www.langchain.com/blog/introducing-openwiki-an-open-source-agent-for-repo-documentation) - LangChain launch announcement.
- [github.com/langchain-ai/openwiki](https://github.com/langchain-ai/openwiki) - Official repository with the CLI and GitHub Action.

## Footnotes

- OpenWiki is a documentation-generation tool, not a knowledge-format specification; for a portable knowledge format see [Open Knowledge Format](./okf.md).
- The project builds on prior "repo wiki" work such as DeepWiki, AutoWiki, and Andrej Karpathy's informal "LLM Wiki" concept.
