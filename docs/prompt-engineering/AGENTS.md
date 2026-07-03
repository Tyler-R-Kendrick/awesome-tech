# Prompt Engineering Agent Instructions

## Scope

These instructions apply to `docs/prompt-engineering/`.

## Focus area

Maintain this folder as the awesome-index scope for prompt programming, structured generation, guidance libraries, and prompt optimization methods.

## Folder-specific guidance

- Prioritize resources that make prompts more reliable, testable, or constrained.
- Describe whether a resource is a framework, library, compiler, optimizer, or technique.
- Keep agent-skill-specific optimization content in `docs/agents/skills` when it is not broadly prompt-engineering focused.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Prompt Engineering` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/prompt-engineering docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
