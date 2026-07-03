# Agent Evals Agent Instructions

## Scope

These instructions apply to `docs/agents/evals/`.

## Focus area

Maintain this folder as the awesome-index scope for evaluation frameworks, benchmark methods, quality gates, regression suites, and governance checks for AI agents.

## Folder-specific guidance

- Favor resources that define measurable evaluation criteria.
- Separate benchmark tooling from governance or policy tooling when the list grows.
- Call out whether an entry is a CLI, SDK, hosted product, or methodology when known.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Agent Evals` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/agents/evals docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
