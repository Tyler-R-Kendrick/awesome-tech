# Agentic Web

The agentic web is the layer that makes existing websites first-class participants in the agent ecosystem — not by generating new interfaces, but by making a site's own content answerable and its own UI operable through natural language. The references here approach that goal from two complementary directions: exposing a site's data to agents for natural-language querying, and embedding agents that drive the site's interface.

## Contents

- [NLWeb](./nlweb.md) - Content access, server-side: Microsoft's open project for conversational, natural-language interfaces over a site's content; every instance is also an MCP server.
- [PageAgent](./page-agent.md) - UI control, client-side (in-page): Alibaba's JavaScript GUI agent that operates a site's own interface through natural language via the DOM.

## Two directions

- **Content access — make a site's data answerable.** Expose structured content so people and agents can query it in natural language and receive structured answers. [NLWeb](./nlweb.md) takes this path, reusing Schema.org/RSS data and serving it over an MCP-compatible `ask` endpoint.
- **UI control — make a site's interface operable.** Embed an agent that perceives and acts on the page's own controls so a user can complete tasks by describing them. [PageAgent](./page-agent.md) takes this path, serializing the live DOM to text and dispatching real events client-side.

## Selection notes

- Use **NLWeb** when the goal is a conversational, queryable interface over your published content, and when you want that content discoverable by agents through MCP.
- Use **PageAgent** when the goal is letting users operate your existing UI (forms, dashboards, multi-step workflows) by describing tasks, entirely within the browser session.
- Both connect to the [Model Context Protocol](../standards/mcp.md): NLWeb serves an MCP endpoint for its content, and PageAgent ships a beta MCP server for external control. This scope is distinct from [Generative UI](../genUI/README.md), which is about generating interfaces rather than querying or operating existing ones.
