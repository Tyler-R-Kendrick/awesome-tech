# Retrieval-Augmented Generation Agent Instructions

## Scope

These instructions apply to `docs/prompt-engineering/rag/`.

## Focus area

Maintain this folder as the awesome-index scope for retrieval-augmented generation: retrieval frameworks, indexing and parsing pipelines, retrieval techniques, and RAG evaluation. The `llama-parse/` subfolder is the required parsing/ingestion setup.

## Folder-specific guidance

- Cover the full RAG loop: parse/ingest, chunk, index, retrieve, rerank, and evaluate.
- Keep repository ingestion policy in the `llama-parse/` subfolder; link to it rather than duplicating it.
- Prefer canonical frameworks and well-known techniques; note when a resource is a technique vs. a framework vs. an eval tool.

## Required structure

- `README.md` is the category index for this scope.
- Start with `# Retrieval-Augmented Generation (RAG)` and a concise description of the scope.
- Use `## Contents`, not `## Table of Contents`.
- Keep entries grouped and consistently formatted.
- Prefer `- [Name](URL) - Description.` for verified resources.
- Preserve repo-wide requirements from the root `AGENTS.md` and `docs/standards/README.md`.

## Enforcement

- Run `git diff --check` after edits.
- Run `rg "^## Table of Contents" docs/prompt-engineering/rag docs/standards/README.md` before committing documentation changes.
- Check that new entries are relevant to this folder's focus and are not better placed in a sibling category.
