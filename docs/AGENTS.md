# Documentation Root Agent Instructions

## Scope

These instructions apply to `docs/` and all nested documentation folders unless a more specific `AGENTS.md` overrides them.

## Focus area

`docs/` holds the entire curated knowledge index. Keep it organized as a shallow, navigable tree of category folders, each with a `README.md` index and, where it is a distinct scope, an `AGENTS.md`.

## Folder-specific guidance

- Keep the repository root clean: curated content lives under `docs/`, not at the root.
- Group related categories under a parent folder (for example, agent capabilities under `agents/`).
- Every content folder starts with a `# Title` and a concise scope description, then `## Contents`.

## Required structure

- `README.md` is the top-level documentation index and links to each category.
- Use `## Contents`, not `## Table of Contents`.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs` before committing documentation changes.
- Check that new categories are linked from `docs/README.md` and the root `README.md`.
