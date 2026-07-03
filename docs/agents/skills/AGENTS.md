# Agent Skill Optimizations Agent Instructions

## Scope

These instructions apply to `docs/agents/skills/`.

## Focus area

Maintain this folder as the awesome-index scope for skill discovery, skill learning, prompt/program optimization, and reusable capability improvement for agents.

## Folder-specific guidance

- Focus on reusable skills or optimization of agent capabilities.
- Differentiate skill-generation systems from generic prompt optimization systems.
- Cross-reference prompt-engineering only when the entry is primarily prompt-centric.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Agent Skill Optimizations` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/agents/skills docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
