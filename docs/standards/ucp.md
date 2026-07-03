# Universal Commerce Protocol (UCP)

Google's open-source standard for agent-driven commerce (detailed publicly January 2026, with a "Universal Cart" expansion at Google I/O 2026) that provides a common language and functional primitives so agents, businesses, payment and credential providers, and consumer surfaces interoperate across the full commerce journey — discovery, checkout, payment, and order management — instead of building unique per-agent integrations. It is designed to be compatible with A2A, AP2, and MCP: roughly, AP2 handles the payment and authorization layer while UCP handles the broader commerce, checkout, and order layer on top. It was co-developed with retailers including Shopify, Etsy, Wayfair, Target, and Walmart.

## Contents

- [Under the Hood: Universal Commerce Protocol (UCP)](https://developers.googleblog.com/under-the-hood-universal-commerce-protocol-ucp/) - Google Developers technical overview.
- [github.com/universal-commerce-protocol/ucp](https://github.com/universal-commerce-protocol/ucp) - Specification, schemas, and SDKs (Apache-2.0).
- [Universal Cart in Google Shopping](https://blog.google/products-and-platforms/products/shopping/google-shopping-cart/) - Google I/O 2026 expansion announcement.

## Footnotes

- Google's UCP is distinct from the separate, similarly themed Agentic Commerce Protocol (ACP) from OpenAI and Stripe; the generic phrase "agentic commerce protocol" is used loosely in press for both.
- UCP pairs with Google's [Agent Payments Protocol (AP2)](./ap2.md) for the payment layer.
- `ucp.dev` is referenced by Google's blog and the GitHub repository as the official site; it is not independently verified here.
