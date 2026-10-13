# Conduit — Filings & Fundamentals, for Gemini CLI

A [Gemini CLI](https://geminicli.com) extension that wires the hosted
**Conduit — Filings & Fundamentals** MCP server into your terminal.

Conduit gives your agent direct, read-only access to U.S. SEC EDGAR — the
primary source for public-company filings and financials: company identity
and filing history, 10-K / 10-Q facts (revenue, profits, EPS, assets, cash,
debt), key ratios, revenue by business segment, side-by-side peer
comparisons, all-filer rankings, filing full-text search, and insider
filings and amendments. 24 read-only tools in all, refreshed within 48 hours
of SEC publication and returned as reported in the filings.

## Install

```bash
gemini extensions install https://github.com/nrupala/conduit-gemini-extension
```

On install, Gemini CLI prompts for your **Conduit API key** (stored as
`CONDUIT_API_KEY`). Get a key at [pipavia.com](https://pipavia.com) — a free
tier is available; Pro and Team tiers raise the daily quota.

## What this repo is

This is a thin wrapper: it contains no server code. The extension manifest
(`gemini-extension.json`) points Gemini CLI at the hosted Conduit MCP server
(`https://mcp.pipavia.com/mcp`, Streamable HTTP) and sends your key as an
`Authorization: Bearer <key>` header on each call. The server also supports
OAuth 2.1 sign-in for clients that use it directly.

- Documentation: https://pipavia.com/docs
- Privacy policy: https://pipavia.com/privacy
- Terms: https://pipavia.com/terms
- Support: info@pipavia.com

## License

Apache-2.0. See `LICENSE`.

---
Owned by Nrupal Akolkar · Built with Muse by Meta
