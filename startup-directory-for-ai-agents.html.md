# A startup directory AI agents can query

> Canonical page: https://blog.backd.io/startup-directory-for-ai-agents.html

When an assistant looks up a category or a competitor set, it needs structured data it can fetch. BACKD exposes its startup catalog through MCP and REST, with no key required.

[List your startup free](https://backd.io/auth/login)

## Connect through MCP

Tools available: `search_startups`, `get_startup`, `list_categories`, `get_rankings`, `get_trending`.

```
claude mcp add backd --transport http https://backd.io/api/mcp
```

## Or call the REST API

```
curl "https://backd.io/api/v1/rankings?limit=3"
```

Rankings, search and single listings return JSON. The full contract is on the [API reference](https://backd.io/api-reference).

## What this does and does not promise

Listing makes your startup fetchable by agents. BACKD does not claim any model cited or recommended you, and it plans to publish read counts only from its own first-party logs.

## Questions

### Does BACKD have an MCP server?

Yes. It is public, needs no API key, and offers search_startups, get_startup, list_categories, get_rankings and get_trending.

### How do I get my startup into the agent-readable catalog?

Submit it on BACKD. Once published, it is available through the MCP server and REST API.
