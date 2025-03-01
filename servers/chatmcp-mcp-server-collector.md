---
type: server
repo_url: https://github.com/chatmcp/mcp-server-collector
name: MCP Server Collector
owner: chatmcp
stars: 18
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/discovery",
    "purpose/collection",
    "purpose/indexing",
    "tech/mcp",
    "purpose/aggregation",
  ]
---

# MCP Server Collector

#status/active #category/discovery #purpose/collection #purpose/indexing #tech/mcp #purpose/aggregation

## Description

A MCP Server used to collect MCP Servers over the internet. This server discovers, indexes, and aggregates information about available MCP servers across the web.

## Features

- Server discovery
- Information collection
- Server indexing
- Metadata aggregation
- Availability monitoring
- Version tracking
- API documentation
- Status checking
- Category organization
- Search functionality

## Installation

```bash
npm install @chatmcp/mcp-server-collector
```

## Usage

```javascript
{
  "mcpServers": {
    "collector": {
      "command": "npx",
      "args": ["@chatmcp/mcp-server-collector"],
      "env": {
        "SCAN_INTERVAL": "3600",
        "MAX_DEPTH": "3",
        "TIMEOUT": "30000",
        "VERIFY_SERVERS": "true",
        "INDEX_PATH": "./index"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Network scanner
- Metadata parser
- Index database
- Status checker
- Search engine

## Related Servers

- liuyoshio/mcp-compass
- modelcontextprotocol-discovery-server
- modelcontextprotocol-registry-server
