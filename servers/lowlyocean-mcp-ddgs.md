---
type: server
repo_url: https://github.com/lowlyocean/mcp-ddgs
name: DuckDuckGo Search MCP Server
owner: lowlyocean
stars: 0
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/search",
    "integration/duckduckgo",
    "purpose/web-search",
    "purpose/data-structure",
    "tech/api",
  ]
---

# DuckDuckGo Search MCP Server

#status/active #category/search #integration/duckduckgo #purpose/web-search #purpose/data-structure #tech/api

## Description

Integrates with DuckDuckGo to enable web search functionality, returning results as structured data for easy incorporation into AI workflows.

## Features

- Web search
- Structured results
- Data formatting
- Search filtering
- Result ranking
- Query optimization
- Region support
- Safe search
- Result caching
- Error handling

## Installation

```bash
npm install @lowlyocean/mcp-ddgs
```

## Usage

```javascript
{
  "mcpServers": {
    "ddg-search": {
      "command": "npx",
      "args": ["@lowlyocean/mcp-ddgs"],
      "env": {
        "REGION": "wt-wt",
        "SAFE_SEARCH": "moderate",
        "MAX_RESULTS": "25",
        "CACHE_TTL": "3600",
        "TIMEOUT": "10000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- DuckDuckGo API
- Result parser
- Cache system
- Query builder
- Data formatter

## Related Servers

- modelcontextprotocol-brave-search
- kagisearch-kagimcp
- meilisearch-meilisearch-mcp
