--- 
type: server
repo_url: https://github.com/baryhuang/mcp-server-any-openapi
name: Any OpenAPI MCP Server
owner: baryhuang
stars: 7
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/api", "tech/openapi", "purpose/api-integration", "tech/docker"]
---

# Any OpenAPI MCP Server

#status/active #category/api #tech/openapi #purpose/api-integration #tech/docker

## Description

This server facilitates scalable discovery and execution of OpenAPI endpoints using semantic search and high-performance processing, overcoming limitations of large spec handling for streamlined API interactions. It uses in-memory semantic search to find relevant Api endpoints by natural language and returns the complete end-point docs in millionseconds.

## Features

- OpenAPI endpoint discovery
- Semantic search using optimized MiniLM-L3 model (43MB vs original 90MB)
- High-performance processing
- Large spec handling
- API interactions
- Endpoint execution
- Schema validation
- Request/response handling
- Use remote openapi json file as source, no local file system access, no updating required for API changes
- FastAPI-based server with async support
- Endpoint based chunking OpenAPI specs (handles 100KB+ documents), no loss of endpoint context
- In-memory FAISS vector search for instant endpoint discovery

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
- FastAPI

## Related Servers

- None currently listed