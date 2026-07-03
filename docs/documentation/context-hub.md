# LangSmith Context Hub

A central, version-controlled store in [LangSmith](../agents/tracing/langsmith.md) for the files that define how agents behave — the **context** an agent reads and follows, such as system instructions, `AGENTS.md` files, skills, policies, examples, writing guidelines, and domain knowledge. Much of this content doesn't fit naturally in a code repository, yet many agent failures come from missing, stale, or poorly managed context. Context Hub gives teams a home to store, version, promote, and collaborate on that context separately from the application code, so agents load approved, environment-appropriate context in production.

A context is a versioned bundle of instructions and tools, and comes in two types: an **agent** (a full bundle including an `AGENTS.md` file and tools) and a **skill** (a reusable capability including a `SKILL.md` file). Every saved change creates a **commit** in the commit history, so teams can browse, compare, and revert prior versions without losing work, and any commit can be given a human-readable **tag**. Commits are promoted through environment tags — `staging` and `production` — so an agent pulls the right context for the environment it runs in. An SDK manages contexts programmatically (push, pull, list, and delete), letting agent code fetch a specific commit or tag for reproducible runs.

## Contents

- [Introducing Context Hub](https://www.langchain.com/blog/introducing-context-hub) - Announcement of the versioned context store and its motivation.
- [Use the Context Hub](https://docs.langchain.com/langsmith/use-the-context-hub) - Documentation for context types, commits, tags, and the SDK.
- [smith.langchain.com/context](https://smith.langchain.com/context) - The Context Hub in the hosted application.

## Footnotes

- Context Hub curates and manages the same agent-facing file formats tracked in this repository: [AGENTS.md](./agents-md.md) for agent bundles and the [Agent Skills](../agents/skills/README.md) `SKILL.md` format for reusable capabilities.
- It operationalizes [context engineering](../prompt-engineering/context-engineering/README.md) — versioning, promoting, and governing the instructions and knowledge in an agent's context window rather than treating them as ad-hoc prompt strings.
- Part of the [LangSmith](../agents/tracing/langsmith.md) platform; documented here as a content/knowledge-management tool, distinct from the wire protocols under [standards](../standards/README.md).
- Environment promotion supports `staging` and `production` tags; confirm the current tag set and SDK surface against the official documentation, as the feature is new.
