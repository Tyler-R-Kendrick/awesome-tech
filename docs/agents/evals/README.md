# Agent Evals

A curated index of tools and frameworks for evaluating agent behavior, quality, and governance.

## Contents

- [Harbor](https://github.com/harbor-framework/harbor) - Framework for evaluating and optimizing agents and language models in containerized, sandboxed environments; runs thousands of trials in parallel on local Docker or cloud providers, evaluates any agent that installs in a container, and generates rollouts for reinforcement learning and post-training. Serves as the official harness for Terminal-Bench 2.0.
- agentevals.io: AgentV - CLI and SDK for evaluating agent behavior.
- ASSERT - Microsoft agent-governance-toolkit resource for agent evaluation and governance checks.

## Footnotes

- Harbor is built by Mike Merrill and Alex Shaw, the team behind [Terminal-Bench](https://www.tbench.ai/), and was announced with [Terminal-Bench 2.0](https://www.tbench.ai/news/announcement-2-0) in November 2025. It re-implements the Terminal-Bench harness to add cloud-deployed containers, a framework-agnostic agent abstraction, and interfaces for reinforcement learning, supervised fine-tuning, and prompt optimization. The project is Apache-2.0 licensed and its canonical repository lives under the `harbor-framework` organization.
- Install with `uv tool install harbor` (PyPI package `harbor`) and run a benchmark with, for example, `harbor run -d terminal-bench@2.0 --agent claude-code`. Harbor defines each task as a container plus a deterministic verifier and oracle solution, ships adapters for 20+ benchmarks, and can evaluate agents such as Claude Code, OpenHands, Codex CLI, Aider, Goose, Gemini CLI, and Mini SWE Agent under a shared protocol.
- Parallel execution runs on local Docker or cloud sandbox providers such as Daytona, Modal, E2B, Runloop, and Google Kubernetes Engine. A web-based results viewer browses jobs and inspects each trial's trajectory, tool calls, token usage, and rewards, and the [Harbor Hub](https://hub.harborframework.com) hosts shared benchmarks and leaderboards. See the [documentation](https://www.harborframework.com/docs) and the [cookbook](https://github.com/harbor-framework/harbor-cookbook).
- Because Harbor drives evaluation, RL rollouts, and prompt optimization from one containerized task definition, it links this scope to [agent optimization](../optimization/README.md); external benchmarks such as SkillsBench and CompileBench have been ported to the Harbor task format.
