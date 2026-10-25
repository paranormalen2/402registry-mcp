# 402registry MCP server

Remote MCP server for **402registry** (https://402registry.com). Checks whether AI agents and AI crawlers can actually see a website: a plain HTTP fetch with no JavaScript, the way GPTBot, ClaudeBot, PerplexityBot and OAI-SearchBot fetch pages. $0.01 per check over the x402 protocol (USDC on Base), no account, no API key. A passing check earns a dated badge and a free listing in a public catalog.

This repository holds the listing metadata for MCP catalogs. The server itself is hosted; there is nothing to
install or run locally.

## Connect

- Endpoint (Streamable HTTP): `https://402registry.com/mcp`
- No account, no API key.

Claude Code:

```bash
claude mcp add --transport http 402registry https://402registry.com/mcp
```

Any other client: add a remote (Streamable HTTP) server with the URL above.

## Tools

| Tool | What it does |
|---|---|
| `lookup_site` | The last dated verdict for a website, if it was ever checked and listed: verdict, score, date and badge. Free. |
| `get_pricing` | Every product for sale — the check (one payment, one check) and the catalog snapshot — with its price, the query parameters the paid request needs, and the exact x402 v2 payment requirements. |
| `get_docs` | The whole machine guide as JSON: quickstart, what each verdict means, packs, the rules every check runs, and every public route. |
| `get_service_status` | Whether the service is selling right now, in which mode and on which network, and if not, why not. |

## Links

- Website: https://402registry.com
- For language models: https://402registry.com/llms.txt
- Official MCP Registry entry: `com.402registry/402registry`
