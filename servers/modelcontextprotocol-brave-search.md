---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search
name: Brave Search MCP Server
owner: modelcontextprotocol
stars: 9794
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "status/official",
    "category/search",
    "integration/brave",
    "purpose/web-search",
  ]
---

# Brave Search MCP Server

#status/active #status/official #category/search #integration/brave #purpose/web-search

## Description

Web and local search using Brave's Search API.

## Features

- Web search functionality
- Local search capability
- API integration
- Result filtering
- Search customization
- Privacy protection
- Query optimization
- Result ranking

## Installation

```bash
npm install @modelcontextprotocol/brave-search
```

## Usage

```javascript
{
  "mcpServers": {
    "brave-search": {
      "command": "npx",
      "args": ["@modelcontextprotocol/brave-search"],
      "env": {
        "BRAVE_API_KEY": "your-api-key",
        "MAX_RESULTS": "10",
        "SEARCH_TYPE": "web",
        "SAFE_SEARCH": "moderate"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Brave Search API key
- Internet connection
- Cache system (optional)

## Related Servers

- arben-adm/brave-mcp-search
