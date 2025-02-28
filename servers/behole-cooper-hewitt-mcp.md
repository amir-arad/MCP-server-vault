---
type: server
repo_url: https://github.com/behole/cooper-hewitt-mcp
name: Cooper Hewitt MCP Server
owner: behole
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/museum",
    "integration/cooper-hewitt",
    "purpose/art",
    "purpose/collection-access",
    "category/cultural",
    "tech/typescript",
    "tech/javascript",
    "tech/python"
  ]
---

# Cooper Hewitt MCP Server

#status/active #category/museum #integration/cooper-hewitt #purpose/art #purpose/collection-access #category/cultural #tech/typescript #tech/javascript #tech/python

## Description

A TypeScript-based MCP server that provides programmatic access to the Cooper Hewitt Smithsonian Design Museum's digital collections and resources through their API. The server enables searching and retrieving detailed information about museum objects with support for pagination and advanced filtering.

## Features

- Collection search and browsing
- Object metadata retrieval
- Image access and handling
- Exhibition data access
- Advanced search filtering
- Category navigation
- Pagination support
- Data export capabilities
- Multi-language support
- Caching system

## Installation

```bash
# Via npm
npm install @behole/cooper-hewitt-mcp

# Build from source
git clone https://github.com/behole/cooper-hewitt-mcp.git
cd cooper-hewitt-mcp
npm install
```

## Usage

```javascript
{
  "mcpServers": {
    "cooper-hewitt": {
      "command": "npx",
      "args": ["@behole/cooper-hewitt-mcp"],
      "env": {
        "CH_API_KEY": "your-api-key",
        "DEFAULT_LANG": "en",
        "MAX_RESULTS": "100",
        "INCLUDE_IMAGES": "true",
        "CACHE_TTL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript runtime
- Cooper Hewitt API key
- Image processor
- Search engine
- Cache system
- Data formatter
- Python (for some utilities)

## Related Servers

- modelcontextprotocol-museum-server
- modelcontextprotocol-cultural-server
- modelcontextprotocol-art-server