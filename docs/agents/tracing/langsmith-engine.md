# LangSmith Engine

A deep agent inside [LangSmith](./langsmith.md) that closes the loop from observability to improvement: instead of a human reading traces, spotting patterns, and hand-writing fixes, Engine does that continuously. It has access to production trace data, evaluator feedback, and — when connected to the repository — the agent's source code, and it clusters recurring production failures into named **issues** rather than surfacing one trace at a time. For each issue it diagnoses a likely root cause against the code and proposes fixes for human review.

Engine watches several signal types to decide what is worth fixing: explicit errors (tool-call failures, timeouts), online evaluator failures, trace anomalies (latency spikes, token blowouts, unexpected step counts), negative user feedback, and unexpected behaviors such as users asking for things the agent was not built to handle. When it opens an issue, it can propose three artifacts: a **pull request** with targeted code or prompt changes, a **scoped online evaluator** to catch that specific regression going forward, and **failing traces added to an offline eval dataset** as ground-truth examples. The developer stays in the loop — Engine drafts and proposes; it does not merge autonomously. It launched in public beta in May 2026.

## Contents

- [Introducing LangSmith Engine](https://www.langchain.com/blog/introducing-langsmith-engine) - Announcement describing the deep agent, monitored signals, and proposed fixes.
- [LangSmith platform](https://www.langchain.com/langsmith-platform) - The platform Engine is part of.
- [smith.langchain.com](https://smith.langchain.com/) - The hosted application where Engine runs.

## Footnotes

- Engine is a capability of [LangSmith](./langsmith.md) and depends on its trace and evaluator data; it is not a standalone product.
- It bridges this tracing scope with [agent optimization](../optimization/README.md) and [evals](../evals/README.md): it consumes traces (observability) and emits PRs, evaluators, and eval datasets (optimization and evaluation).
- Public beta as of May 2026; treat availability, scope, and behavior as subject to change and verify against the announcement before relying on specifics.
