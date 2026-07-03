# Agent Memory Agent Instructions

## Scope

These instructions apply to `docs/agents/memory/`.

## Focus area

Maintain this folder as the awesome-index scope for agent memory: persistent, long-term, episodic, semantic, and working memory frameworks and services for LLM agents and multi-agent systems.

## Folder-specific guidance

- Distinguish memory layers (short-term/working vs. long-term/persistent) and storage backends where relevant.
- Prefer maintained, canonical projects with clear memory abstractions over general vector-store wrappers.
- Keep retrieval-corpus tooling in `prompt-engineering/rag` unless it is specifically an agent-memory system.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Agent Memory` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/agents/memory docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
