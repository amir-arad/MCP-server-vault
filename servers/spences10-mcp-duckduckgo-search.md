---
type: server
repo_url: https://github.com/spences10/mcp-duckduckgo-search
name: DuckDuckGo Search MCP Server
owner: spences10
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/search",
    "integration/duckduckgo",
    "purpose/web-search",
    "category/ai",
    "tech/llm",
    "tech/nodejs",
  ]
---

# DuckDuckGo Search MCP Server

#status/active #category/search #integration/duckduckgo #purpose/web-search #category/ai #tech/llm

## Description

Enables integration with DuckDuckGo search capabilities for LLMs, supporting comprehensive web search, regional filtering, result types, and safe browsing with caching and customizable search parameters.

## Features

- Web search integration
- Regional search filtering
- Safe browsing options
- Result type filtering
- Search parameter customization
- Result caching
- LLM integration
- Search analytics
- Custom timeout settings
- Error handling

## Installation

```bash
npm install @spences10/mcp-duckduckgo-search
```

## Usage

```javascript
{
  "mcpServers": {
    "duckduckgo-search": {
      "command": "npx",
      "args": ["@spences10/mcp-duckduckgo-search"],
      "env": {
        "REGION": "wt-wt",
        "SAFE_SEARCH": "on",
        "MAX_RESULTS": "10",
        "CACHE_TTL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- DuckDuckGo API
- Cache storage system
- LLM integration support
- HTTP client library

## Related Servers

- [DuckDuckGo MCP Server](https://github.com/qwang07/duck-duck-mcp) - Alternative DuckDuckGo implementation
