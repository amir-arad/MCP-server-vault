---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/tree/main/src/fetch
name: Fetch MCP Server
owner: modelcontextprotocol
stars: 9794
last_updated: 2025-02-21
status: active
official: true
verified: true
sources: ["inbox/batch_011.md"]
tags: ["status/active", "status/official", "status/verified", "category/web", "purpose/content-fetching", "purpose/llm-optimization"]
---

# Fetch MCP Server

#status/active #status/official #status/verified #category/web #purpose/content-fetching #purpose/llm-optimization

## Description

Web content fetching and conversion for efficient LLM usage, providing optimized content processing and formatting for language model consumption.

## Features

- Web content fetching
- Content optimization
- LLM-friendly formatting
- Content conversion
- Resource handling
- Cache management
- Rate limiting
- Error handling
- Content cleaning
- Format validation

## Installation

```bash
npm install @modelcontextprotocol/fetch
```

## Usage

```javascript
{
  "mcpServers": {
    "fetch": {
      "command": "npx",
      "args": ["@modelcontextprotocol/fetch"],
      "env": {
        "MAX_CONTENT_SIZE": "1048576",
        "RATE_LIMIT": "10",
        "CACHE_TTL": "3600",
        "OUTPUT_FORMAT": "markdown"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Network connectivity
- Cache system
- Content processor
- Rate limiter

## Related Servers

- [Fetch MCP](https://github.com/zcaceres/fetch-mcp) - Community fetch implementation
- [Fetch](https://github.com/kazuph/mcp-fetch) - Alternative fetch implementation