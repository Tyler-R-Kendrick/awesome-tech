# Repository Standards

Repo-wide standards for maintaining this repository as an awesome-style knowledge index that remains compatible with required knowledge formats and indexing workflows.

## Contents

- [Required Standards](#required-standards) - Required knowledge formats for repository documents.
- [Awesome-Index Structure](#awesome-index-structure) - Markdown structure used by repository indexes.
- [Enforcement](#enforcement) - Checks and expectations for repository changes.
- [Indexing Requirement](#indexing-requirement) - Required parsing and indexing workflow.

## Required Standards

All repository documents **must** follow:

1. **LLM Wiki 2.0 (LangChain standard)**
2. **Open Knowledge format (Google standard)**

## Awesome-Index Structure

- Use `## Contents` for index navigation; do not use `## Table of Contents` in awesome indexes.
- Root and category indexes should start with a `#` title and a concise scope description.
- Keep Contents shallow and focused on the most important sections or resources.
- Prefer verified Markdown links with short descriptions for curated resources.
- Descriptions should be neutral, concise, and end with a period.
- Place secondary notes in `## Footnotes` only when needed, and keep that section out of Contents.

## Enforcement

- New and updated documentation must conform to both required standards above.
- Pull requests should describe how changes satisfy both standards.
- Category folders must keep a `README.md` that acts as a curated contents index.
- Every folder scope should include an `AGENTS.md` file with standards and focus-area guidance.
- Run `git diff --check` and `rg "^## Table of Contents"` before committing documentation changes.

## Indexing Requirement

All repository ingestion/indexing work must use:

- **LlamaParse Cloud Index v2**
- Getting started guide: <https://developers.llamaindex.ai/llamaparse/cloud-index-v2/getting_started/>
