---
type: server
repo_url: https://github.com/arben-adm/brave-mcp-search
name: Brave Search MCP Server
owner: arben-adm
stars: 2
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/search",
    "integration/brave",
    "purpose/web-search",
  ]
---

# Brave Search MCP Server

#status/active #category/search #integration/brave #purpose/web-search

## Description

Facilitates integration of Brave Search functionalities with AI assistants through the Model Context Protocol, enabling web and local searches using the Brave Search API.

## Features

- Web search integration
- Local search capability
- AI assistant support
- Search API access
- Result filtering
- Query optimization
- Content ranking
- Privacy protection

## Installation

```bash
npm install @arben-adm/brave-mcp-search
```

## Usage

```javascript
{
  "mcpServers": {
    "brave-search": {
      "command": "npx",
      "args": ["@arben-adm/brave-mcp-search"],
      "env": {
        "BRAVE_API_KEY": "your-api-key",
        "RESULTS_PER_PAGE": "10",
        "SAFE_SEARCH": "strict",
        "MARKET": "en-US"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Brave Search API key
- Internet connection
- Cache storage (optional)

## Related Servers

- modelcontextprotocol/servers/tree/main/src/brave-search
