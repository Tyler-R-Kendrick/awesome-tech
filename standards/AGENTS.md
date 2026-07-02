# Repository Standards Agent Instructions

## Scope

These instructions apply to `standards/`.

## Focus area

Maintain this folder as the awesome-index scope for repo-wide documentation policy, awesome-index conventions, and enforcement requirements.

## Folder-specific guidance

- Treat this folder as the canonical source for standards and enforcement details.
- When changing standards, update both this folder and any affected scoped `AGENTS.md` files.
- Keep standards actionable and testable; include enforcement checks where possible.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Repository Standards` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" standards README.md standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
