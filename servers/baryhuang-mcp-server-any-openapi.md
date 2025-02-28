---
type: server
repo_url: https://github.com/baryhuang/mcp-server-any-openapi
name: Any OpenAPI MCP Server
owner: baryhuang
stars: 5
last_updated: 2025-02-13
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/api", "tech/openapi", "purpose/api-integration"]
---

# Any OpenAPI MCP Server

#status/active #category/api #tech/openapi #purpose/api-integration

## Description

This server facilitates scalable discovery and execution of OpenAPI endpoints using semantic search and high-performance processing, overcoming limitations of large spec handling for streamlined API interactions.

## Features

- OpenAPI endpoint discovery
- Semantic search
- High-performance processing
- Large spec handling
- API interactions
- Endpoint execution
- Schema validation
- Request/response handling

## Installation

```bash
npm install @baryhuang/mcp-server-any-openapi
```

## Usage

```javascript
{
  "mcpServers": {
    "any-openapi": {
      "command": "npx",
      "args": ["@baryhuang/mcp-server-any-openapi"],
      "env": {
        "SPEC_URL": "https://api.example.com/openapi.json",
        "CACHE_TTL": "3600",
        "MAX_SPEC_SIZE": "10MB",
        "SEMANTIC_THRESHOLD": "0.8"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- OpenAPI specifications
- Semantic search engine
- Cache storage (optional)

## Related Servers

- None currently listed