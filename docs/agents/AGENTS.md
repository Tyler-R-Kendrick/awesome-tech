# Agents Agent Instructions

## Scope

These instructions apply to `docs/agents/`.

## Focus area

Maintain this folder as the parent scope for agent-capability categories: harnesses, sandboxes, optimization, skills, memory, tracing, and evals. Each capability is its own subfolder index.

## Folder-specific guidance

- Keep each capability in its own subfolder; do not merge distinct capabilities into one index.
- Place a resource in the single most relevant capability; cross-reference rather than duplicate.
- `README.md` here is a navigation index to the capability subfolders.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Agents` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/agents docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
