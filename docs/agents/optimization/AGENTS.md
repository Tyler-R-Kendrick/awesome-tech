# Agent Optimization Agent Instructions

## Scope

These instructions apply to `docs/agents/optimization/`.

## Focus area

Maintain this folder as the awesome-index scope for optimization frameworks, trace-driven improvement loops, training methods, and performance tuning for AI agents.

## Folder-specific guidance

- Identify what is optimized: cost, latency, reliability, trajectory quality, or task success.
- Prefer entries with reproducible methods, papers, code, or clear methodology.
- Keep tracing-only resources in `docs/agents/tracing` unless they directly support optimization workflows.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Agent Optimization` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/agents/optimization docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
