# Debug Adapter Protocol (DAP)

An open, JSON-based protocol from Microsoft that standardizes communication between a development tool (editor or IDE) and a debugger, mediated by a reusable "debug adapter." It solves the M×N integration problem — without a shared protocol, every tool needs a custom integration for every debugger — much as the Language Server Protocol (LSP) does for language features. DAP grew out of Visual Studio Code's architecture and was published as a standalone protocol with its own website and repository in August 2018; its wire format (a `Content-Length` header followed by a JSON body) mirrors LSP, and its message set covers requests, responses, events, and reverse requests.

## Contents

- [microsoft.github.io/debug-adapter-protocol](https://microsoft.github.io/debug-adapter-protocol/) - Official site, overview, and documentation.
- [Specification](https://microsoft.github.io/debug-adapter-protocol/specification.html) - Current protocol specification, including the base protocol and all requests, responses, and events.
- [Overview](https://microsoft.github.io/debug-adapter-protocol/overview) - How the protocol works, the debug-session lifecycle, and its relationship to LSP.
- [Debug adapters registry](https://microsoft.github.io/debug-adapter-protocol/implementors/adapters/) - Directory of known debug adapters across languages and runtimes.
- [github.com/microsoft/debug-adapter-protocol](https://github.com/microsoft/debug-adapter-protocol) - Specification repository and source for the website.
- [debugAdapterProtocol.json](https://github.com/microsoft/debug-adapter-protocol/blob/main/debugAdapterProtocol.json) - Machine-readable JSON schema for the protocol.
- [microsoft/vscode-debugadapter-node](https://github.com/microsoft/vscode-debugadapter-node) - Reference Node.js SDK, published as the `@vscode/debugadapter` and `@vscode/debugprotocol` npm packages.
- [New home for the Debug Adapter Protocol](https://code.visualstudio.com/blogs/2018/08/07/debug-adapter-protocol-website/) - August 2018 announcement of the standalone protocol website.

## Footnotes

- The specification is versioned (for example, `1.71.0` as of this writing); the [change log](https://microsoft.github.io/debug-adapter-protocol/changelog.html) tracks revisions.
- DAP is the debugging counterpart to LSP; both originated with Visual Studio Code, and DAP's JSON wire format was inspired by the now-obsolete V8 Debugging Protocol.
- The specification and website are licensed under Creative Commons Attribution, and the associated code is licensed under MIT.
