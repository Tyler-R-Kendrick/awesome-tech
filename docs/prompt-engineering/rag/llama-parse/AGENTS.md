# LlamaParse Cloud Index v2 Setup Agent Instructions

## Scope

These instructions apply to `llama-parse/`.

## Focus area

Maintain this folder as the awesome-index scope for repository ingestion and parsing policy centered on LlamaParse Cloud Index v2.

## Folder-specific guidance

- Do not add alternative parsing or indexing paths that bypass LlamaParse Cloud Index v2.
- Keep setup links pointed at official LlamaIndex documentation.
- Ensure parsing guidance remains compatible with LLM Wiki 2.0 and Open Knowledge expectations.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# LlamaParse Cloud Index v2 Setup` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" llama-parse README.md standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
