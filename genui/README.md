# Generative UI (GenUI)

Generative UI is the emerging layer where agents and models produce structured, interactive interfaces instead of only text. The projects below are useful reference points for building chat-native, agent-driven, or model-composed UI.

## Core projects and specs

| Project | What it is | Notes |
| --- | --- | --- |
| [OpenUI](https://github.com/thesysdev/openui) | Full-stack generative UI framework with a compact streaming language, React runtime, component libraries, and chat interfaces. | Useful when the model should compose UI from a constrained component vocabulary while keeping rendering streaming-first and framework-friendly. |
| [json-render](https://github.com/vercel-labs/json-render) | Vercel Labs generative UI framework where models emit JSON constrained to a component catalog. | Good reference for schema/catalog-driven UI generation and progressive rendering from structured model output. |
| [MCP Apps](https://github.com/modelcontextprotocol/ext-apps) | Official MCP extension for returning interactive UI resources from MCP tools. | Important for tool-owned UI that renders inline in compliant agent/chat hosts. See also the [`mcp-ui`](https://github.com/MCP-UI-Org/mcp-ui) SDK implementation. |
| [A2UI](https://github.com/a2ui-project/a2ui) | Agent-to-User Interface format and renderer set for updatable, agent-generated UIs. | Focuses on agents sending declarative UI messages that clients render with native components across platforms. |
| [OpenAI Apps SDK](https://developers.openai.com/apps-sdk/) and [ChatKit widgets](https://developers.openai.com/api/docs/guides/chatkit-widgets) | OpenAI's SDK and widget system for building interactive ChatGPT apps and embeddable chat experiences. | This is the OpenAI “chat SDK widget thing”: Apps SDK connects MCP-style tools/resources to ChatGPT apps, while ChatKit widgets are the customizable UI containers and components for ChatKit chat experiences. |

## Related protocols

| Project | What it is | Why it is adjacent |
| --- | --- | --- |
| [AG-UI](https://github.com/ag-ui-protocol/ag-ui) | Event-based Agent-User Interaction protocol for connecting agents to user-facing applications. | Worth tracking, but it is more of an agent/frontend event protocol than a direct generative UI rendering format, so it is listed as related rather than core. |

## Selection notes

- Use **OpenUI** or **json-render** when the primary problem is letting an AI compose screens from a safe, predefined component catalog.
- Use **MCP Apps** when the tool/server should own the UI resource and expose it through MCP to any compatible host.
- Use **A2UI** when the target is cross-platform, native rendering from agent-authored UI messages.
- Use **OpenAI Apps SDK / ChatKit widgets** when building specifically for ChatGPT apps or OpenAI-hosted/embedded chat experiences.
- Track **AG-UI** for agent-to-frontend event interoperability, but do not treat it as the same category as renderer-first GenUI frameworks.
