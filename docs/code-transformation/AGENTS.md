# Code Transformation Agent Instructions

## Scope

These instructions apply to `docs/code-transformation/`.

## Focus area

Maintain this folder as the awesome-index scope for automated, rules-based code-transformation tooling: deterministic engines that refactor, migrate, and modernize source code at scale, and the interfaces through which agents drive them.

## Folder-specific guidance

- Track deterministic transformation engines and codemod tooling here (recipe- or rule-based refactoring, migration, and upgrade tools), not the agent-to-agent wire protocols in `docs/standards/` or the documentation formats in `docs/documentation/`.
- State whether each entry is a tool, an engine, or a platform, and name its originating organization and open-source license.
- Emphasize the agentic angle: how deterministic transformations complement probabilistic model edits, and how agents invoke them (for example via MCP or agent skills).
- Cross-reference `docs/standards/mcp.md` and `docs/agents/skills/README.md` when an entry ships agent-facing integrations.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Code Transformation` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/code-transformation` before committing documentation changes.
- Run `bun run konsistent` to confirm the folder keeps its `README.md` index and `AGENTS.md`.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
