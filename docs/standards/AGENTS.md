# Repository Standards Agent Instructions

## Scope

These instructions apply to `docs/standards/`.

## Focus area

Maintain this folder as the awesome-index scope for repo-wide documentation policy, awesome-index conventions, enforcement requirements, and the agent interoperability, communication, payment, and commerce protocols this project tracks (for example MCP, ACP, A2A, ARD, A2H, x402, AP2, UCP). Group these protocols under broad sections (communication and interoperability; payments and commerce) so new entries accumulate over time.

## Folder-specific guidance

- Treat this folder as the canonical source for standards and enforcement details.
- When changing standards, update both this folder and any affected scoped `AGENTS.md` files.
- Keep standards actionable and testable; include enforcement checks where possible.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Standards` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/standards docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
