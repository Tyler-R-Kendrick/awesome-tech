# Agent Harness Agent Instructions

## Scope

These instructions apply to `agent-harness/`.

## Focus area

Maintain this folder as the awesome-index scope for agent harnesses, orchestration testbeds, runners, and meta-harnesses that execute or coordinate agents.

## Folder-specific guidance

- Prioritize resources that help run, supervise, or compare agents reproducibly.
- Distinguish concrete harness implementations from higher-level meta-harness patterns.
- Document execution assumptions when adding runnable harnesses.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Agent Harness` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" agent-harness README.md standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
