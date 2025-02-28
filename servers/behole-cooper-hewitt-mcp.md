---
type: server
repo_url: https://github.com/behole/cooper-hewitt-mcp
name: Cooper Hewitt MCP Server
owner: behole
stars: 2
last_updated: 2025-01-30
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/museum",
    "integration/cooper-hewitt",
    "purpose/art",
    "purpose/collection-access",
    "category/cultural",
  ]
---

# Cooper Hewitt MCP Server

#status/active #category/museum #integration/cooper-hewitt #purpose/art #purpose/collection-access #category/cultural

## Description

Interact with the Cooper Hewitt API with MCP. This server provides access to the Cooper Hewitt Smithsonian Design Museum's digital collections and resources.

## Features

- Collection access
- Object search
- Metadata retrieval
- Image access
- Exhibition data
- Collection browsing
- Object details
- Search filtering
- Category navigation
- Data export

## Installation

```bash
npm install @behole/cooper-hewitt-mcp
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
- Cooper Hewitt API key
- Image processor
- Search engine
- Cache system
- Data formatter

## Related Servers

- modelcontextprotocol-museum-server
- modelcontextprotocol-cultural-server
- modelcontextprotocol-art-server
