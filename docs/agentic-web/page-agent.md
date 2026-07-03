# PageAgent

An open-source, in-page GUI agent from Alibaba that lets users drive a website through natural language. Described as "the GUI agent living in your webpage," PageAgent embeds as plain JavaScript in a web app, reads the live DOM as text, and operates the existing interface — finding elements, clicking, and filling forms — without a browser extension, a headless browser, or a server-side automation stack. It is a developer-embeddable library rather than a research system, and there is no associated paper or benchmark.

## Contents

- [alibaba/page-agent](https://github.com/alibaba/page-agent) - Source repository (TypeScript), under the MIT License.
- [PageAgent documentation](https://alibaba.github.io/page-agent/) - Official project site and docs.
- [page-agent on npm](https://www.npmjs.com/package/page-agent) - Published package for embedding the agent in a web app.

## How it works

- **In-page, client-side.** PageAgent runs as JavaScript inside the page, executing in the user's own browser session and inheriting existing cookies, authentication, and UI validation instead of re-driving the site from the outside. The core use case needs no browser extension, headless browser, or Python backend.
- **Text-based DOM, not vision.** Rather than screenshots and multimodal models, PageAgent operates on the DOM as text, so a strong text-only LLM suffices — no visual recognition or special permissions required.
- **DOM serialization.** A `PageController` compresses the live DOM into a flattened text representation of the page's interactive elements — referenced by numeric index rather than CSS selectors — so even smaller models can locate and act on controls precisely; the project describes this step as DOM "dehydration."
- **ReAct-style agent loop.** The agent iterates Observe → Think → Act: it extracts current DOM state, asks the LLM for the next action, then dispatches a real DOM event (click, type, etc.), repeating until the task completes. Its DOM-processing and prompting are credited to the open-source `browser-use` project, re-implemented to live inside the page.
- **Model-agnostic.** It works with any OpenAI-compatible endpoint (bring-your-own LLM); Alibaba's Qwen via DashScope is the default example, with documented support spanning Claude, GPT, DeepSeek, Gemini, and local Ollama models, plus a free test endpoint for evaluation.
- **Optional extras.** A Chrome extension (`MultiPageAgent`) handles tasks that span multiple tabs, and a beta MCP server lets external clients (for example Claude Desktop or Cursor) drive the in-page agent over the [Model Context Protocol](../standards/mcp.md).

## Positioning

- Built for web developers and web applications first: the intended integration is a publisher adding an agent to their own site, framed as client-side web enhancement rather than server-side scraping or browser automation.
- Contrasts with headless-browser tools (Playwright, Puppeteer), which drive an external browser from a server, and with vision-based GUI agents, which rely on screenshots and multimodal models — PageAgent stays inside the page and relies on structured DOM text.

## Use cases

Documented uses include in-app copilots for SaaS, ERP, CRM, and admin dashboards, automated form filling, accessibility assistance, and multi-page or multi-step task automation, collapsing long click-through workflows into a single natural-language instruction.

## Footnotes

- License is MIT; the project is TypeScript-first, published on npm as `page-agent` (v1.11.0 as of this writing), and actively maintained. There are no formal benchmark results (no WebArena, Mind2Web, or WebVoyager numbers).
- PageAgent sits on the UI-control side of the agentic web (operating a site's own interface), complementary to content-access projects such as [NLWeb](./nlweb.md).
