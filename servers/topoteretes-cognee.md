---
type: server
repo_url: https://github.com/topoteretes/cognee
name: Cognee MCP Server
owner: topoteretes
stars: 1268
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/memory",
    "category/ai",
    "tech/graph-database",
    "tech/vector-store",
    "purpose/data-ingestion",
  ]
---

# Cognee MCP Server

#status/active #category/memory #category/ai #tech/graph-database #tech/vector-store #purpose/data-ingestion

## Description

Memory manager for AI apps and Agents using various graph and vector stores and allowing ingestion from 30+ data sources. This server provides comprehensive memory management and knowledge integration capabilities.

## Features

- Memory management
- Graph database support
- Vector store integration
- Multi-source ingestion
- Data processing
- Query optimization
- GraphRAG support
- Customizable pipelines
- Search capabilities
- Knowledge persistence

## Installation

```bash
npm install @topoteretes/cognee-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "cognee": {
      "command": "npx",
      "args": ["@topoteretes/cognee-mcp"],
      "env": {
        "GRAPH_DB_URL": "your-graph-db-url",
        "VECTOR_STORE": "your-vector-store",
        "DATA_SOURCES": "github,notion,confluence",
        "BATCH_SIZE": "1000",
        "PROCESSING_THREADS": "4"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Graph database
- Vector store
- Data processors
- Source connectors
- Query engine

## Related Servers

- modelcontextprotocol-memory-server
- davidvc/code-knowledge-mcptool
- needle-ai-needle-mcp
