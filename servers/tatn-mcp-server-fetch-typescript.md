---
type: server
repo_url: https://github.com/tatn/mcp-server-fetch-typescript
name: Fetch TypeScript MCP Server
owner: tatn
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_012.md"]
tags:
  [
    "status/active",
    "category/web",
    "tech/typescript",
    "purpose/content-fetching",
    "purpose/conversion",
    "tech/web-content",
  ]
---

# Fetch TypeScript MCP Server

#status/active #category/web #tech/typescript #purpose/content-fetching #purpose/conversion #tech/web-content

## Description

A Model Context Protocol server that provides web content fetching and conversion capabilities, implemented in TypeScript for type safety and modern JavaScript features.

## Features

- Web content fetching
- Content conversion
- Type-safe implementation
- Error handling
- Response formatting
- Cache management
- Format validation
- Content cleaning
- Rate limiting
- TypeScript support

## Installation

```bash
npm install @tatn/mcp-server-fetch-typescript
```

## Usage

```javascript
{
  "mcpServers": {
    "fetch-typescript": {
      "command": "npx",
      "args": ["@tatn/mcp-server-fetch-typescript"],
      "env": {
        "DEFAULT_FORMAT": "markdown",
        "CACHE_TTL": "3600",
        "MAX_RETRIES": "3",
        "TIMEOUT": "30000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- TypeScript >= 4.5
- Axios
- Cheerio
- Cache system

## Related Servers

- [Fetch](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch) - Official fetch implementation
- [Fetch Python](https://github.com/tatn/mcp-server-fetch-python) - Python version
