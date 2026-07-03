# Generative UI (GenUI)

Generative UI is the emerging layer where agents and models produce structured, interactive interfaces instead of only text. The space spans a spectrum — from frameworks that let a model compose screens out of a safe component catalog, to protocols that stream agent-authored UI to native renderers, to production systems that generate an entire page layout end to end, and experiments that render the interface itself as model-generated pixels. The references below are useful starting points for building chat-native, agent-driven, or model-composed UI.

## Contents

- [OpenUI](./OpenUI.md) - Generative UI from natural language (wandb/openui) and Thesys's OpenUI Lang framework.
- [json-render](./json-render.md) - Vercel Labs framework where models emit catalog-constrained JSON.
- [MCP Apps](./mcp-apps.md) - Official MCP extension for tool-owned interactive UI resources.
- [A2UI](https://github.com/a2ui-project/a2ui) - Declarative, Apache-2.0 protocol (created by Google with community contributions) for updatable, agent-generated UIs rendered with native components across platforms.
- [OpenAI Apps SDK](https://developers.openai.com/apps-sdk) - SDK for building apps and interactive widgets that render inside ChatGPT; see also [ChatKit widgets](https://developers.openai.com/api/docs/guides/chatkit-widgets).

## Related protocols

- [AG-UI](https://github.com/ag-ui-protocol/ag-ui) - Lightweight, event-based Agent-User Interaction protocol (originated by CopilotKit) for connecting agents to front-end applications; more an agent/frontend event protocol than a direct rendering format.

## Systems and experiments

Production systems and research prototypes that push generative UI beyond component catalogs — from generating an entire page layout to rendering the interface as model-generated pixels. These are references and case studies rather than frameworks you integrate.

- [GenPage](./GenPage.md) - Netflix's end-to-end generative model that constructs the personalized homepage autoregressively, replacing a multi-stage ranking pipeline with a single transformer that composes the whole page.
- [Flipbook](./Flipbook.md) - Experimental "visual browser" in which every page is a model-generated image and clicking anything generates the next image, with no HTML or DOM.

## Selection notes

- Use **OpenUI** or **json-render** when the primary problem is letting an AI compose screens from a safe, predefined component catalog.
- Use **MCP Apps** when the tool or server should own the UI resource and expose it over MCP to any compatible host.
- Use **A2UI** when the target is cross-platform, native rendering from agent-authored UI messages.
- Use **OpenAI Apps SDK / ChatKit widgets** when building specifically for ChatGPT apps or OpenAI-hosted chat experiences.
- Track **AG-UI** for agent-to-frontend event interoperability, distinct from renderer-first GenUI frameworks.
- Study **GenPage** as a production example of whole-page generative composition, where one model generates the full layout instead of ranking rows and items in separate stages.
- Track **Flipbook** as an experiment at the far end of the spectrum, where the interface is generated imagery rather than structured, interactive components.
