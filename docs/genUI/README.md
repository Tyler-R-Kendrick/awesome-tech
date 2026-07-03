# Generative UI (GenUI)

Generative UI is the emerging layer where agents and models produce structured, interactive interfaces instead of only text. The projects below are useful reference points for building chat-native, agent-driven, or model-composed UI.

## Contents

- [OpenUI](./OpenUI.md) - Generative UI from natural language (wandb/openui) and Thesys's OpenUI Lang framework.
- [json-render](./json-render.md) - Vercel Labs framework where models emit catalog-constrained JSON.
- [MCP Apps](./mcp-apps.md) - Official MCP extension for tool-owned interactive UI resources.
- [A2UI](https://github.com/a2ui-project/a2ui) - Declarative, Apache-2.0 protocol (created by Google with community contributions) for updatable, agent-generated UIs rendered with native components across platforms.
- [OpenAI Apps SDK](https://developers.openai.com/apps-sdk) - SDK for building apps and interactive widgets that render inside ChatGPT; see also [ChatKit widgets](https://developers.openai.com/api/docs/guides/chatkit-widgets).

## Related protocols

- [AG-UI](https://github.com/ag-ui-protocol/ag-ui) - Lightweight, event-based Agent-User Interaction protocol (originated by CopilotKit) for connecting agents to front-end applications; more an agent/frontend event protocol than a direct rendering format.

## Selection notes

- Use **OpenUI** or **json-render** when the primary problem is letting an AI compose screens from a safe, predefined component catalog.
- Use **MCP Apps** when the tool or server should own the UI resource and expose it over MCP to any compatible host.
- Use **A2UI** when the target is cross-platform, native rendering from agent-authored UI messages.
- Use **OpenAI Apps SDK / ChatKit widgets** when building specifically for ChatGPT apps or OpenAI-hosted chat experiences.
- Track **AG-UI** for agent-to-frontend event interoperability, distinct from renderer-first GenUI frameworks.
