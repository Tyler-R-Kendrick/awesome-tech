# Repository Agent Instructions

## Scope

These instructions apply to the entire repository unless a nested `AGENTS.md` provides more specific guidance.

## Awesome-index standards

This repository is an `awesome-*` style knowledge index. Maintain it as a curated, consistent set of Markdown indexes rather than an unstructured notes dump.

Extracted standards from established awesome repositories and tooling:

- Use a short `#` title followed by a concise description of the index scope.
- Use a `## Contents` section, not `## Table of Contents`, and place it before topical sections.
- Keep Contents shallow: one level of bullets whenever practical.
- Use clear category names and keep entries grouped by topic.
- Prefer linked entries. Each resource entry should use `- [Name](URL) - Description.` when a trustworthy URL is known.
- Every entry should include a short, neutral description unless the title is fully self-explanatory.
- Keep formatting consistent across the repo: sentence case descriptions, terminal periods, and no marketing-heavy language.
- Curate for quality. Do not add every possible resource; add resources that are useful, maintained, canonical, or clearly relevant.
- Keep licensing and contribution metadata outside README indexes unless a scoped instruction says otherwise.
- Put secondary notes, source notes, or caveats in a bottom `## Footnotes` section when needed; do not include that section in Contents.

## Repo-specific standards

- Preserve the repository's required knowledge formats: LLM Wiki 2.0 and Open Knowledge format.
- Category folders must keep a `README.md` that acts as the category index.
- Root `README.md` is the repository-wide index and links to each category folder.
- The `standards/README.md` file is the canonical repo policy page; update it when changing standards or enforcement expectations.
- LlamaParse Cloud Index v2 is the required ingestion/indexing path for repository document parsing.

## Standard enforcement

Before committing documentation changes:

1. Check for `## Table of Contents` and replace it with `## Contents` unless the text is discussing the phrase itself.
2. Confirm every touched Markdown index has a clear title, description, `## Contents`, and consistent bullets.
3. Confirm category README files link back to relevant repo standards when useful and do not contradict `standards/README.md`.
4. Run `git diff --check` to catch whitespace issues.
5. Use `rg "^## Table of Contents"` to ensure old awesome-list heading style was not reintroduced.

## Writing style

- Be concise, factual, and implementation-oriented.
- Prefer Markdown links over bare URLs in curated indexes.
- Do not invent links, project status, or product claims. If uncertain, keep the entry unlinked and mark it for verification in a note.
