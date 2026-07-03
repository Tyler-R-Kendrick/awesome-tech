# LangSmith

LangChain's framework-agnostic platform for observing, evaluating, and deploying LLM agents. LangSmith captures runtime behavior as **traces** — nested records of every model call, tool call, retrieval, and step in an agent run — and layers evaluation, monitoring, prompt management, and deployment on top of that trace data. It works with any stack: applications built on LangChain and LangGraph are instrumented automatically, and non-LangChain apps (OpenAI SDK, Anthropic SDK, Vercel AI SDK, LlamaIndex, or custom code) connect through native SDK wrappers or OpenTelemetry, so LangSmith can sit alongside an existing telemetry pipeline rather than replacing it.

The platform spans four areas. **Observability** gives trace-level debugging, failure analysis, and production dashboards for cost, latency (P50/P99), error rates, and qualitative scores, with alerting via webhooks or PagerDuty. **Evaluation** runs LLM-as-judge, code-based, and multi-turn evaluators over offline datasets or as online evaluators on live traffic, with side-by-side experiment comparison and human annotation queues. **Prompt management** versions prompts with full history. **Deployment** standardizes shipping agents with human-in-the-loop approvals, background execution, and multi-agent coordination. Two built-in assistants help interpret data: **Polly** summarizes and pinpoints problems inside large traces, and the **Insights Agent** clusters traces to reveal usage patterns and common failure modes. LangSmith is offered as SaaS (US or EU data residency), hybrid, and fully self-hosted, with enterprise controls such as SSO/SAML, SCIM, RBAC, and audit logs.

## Contents

- [LangSmith platform](https://www.langchain.com/langsmith-platform) - Product overview of the observability, evaluation, and deployment platform.
- [LangSmith documentation](https://docs.langchain.com/langsmith) - Official documentation home.
- [Observability docs](https://docs.langchain.com/langsmith/observability) - Tracing, dashboards, and production monitoring guide.
- [smith.langchain.com](https://smith.langchain.com/) - The hosted application.

## Footnotes

- LangSmith is framework-agnostic: LangChain and LangGraph apps are traced automatically, while other frameworks connect via SDK wrappers or [OpenTelemetry](./README.md); it is not limited to LangChain-built applications.
- The platform has expanded beyond observability into a broader agent-engineering stack. [LangSmith Engine](./langsmith-engine.md) closes the loop from traces to fixes, and [LangSmith Context Hub](../../documentation/context-hub.md) manages the instructions and skills agents run with; LangSmith Fleet adds no-code agent creation.
- Documentation moved from `docs.smith.langchain.com` to `docs.langchain.com/langsmith`; older links may redirect.
- Relates to the tracing standards tracked in this folder — LangSmith ingests OpenTelemetry GenAI telemetry and interoperates with OpenInference-style trace data.
