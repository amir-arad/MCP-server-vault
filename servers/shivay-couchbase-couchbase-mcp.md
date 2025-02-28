---
type: server
repo_url: https://github.com/shivay-couchbase/couchbase-mcp
name: Couchbase Vector Search MCP Server
owner: shivay-couchbase
stars: 0
last_updated: 2025-01-03
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/database",
    "integration/couchbase",
    "purpose/vector-search",
    "tech/semantic",
    "category/demo",
  ]
---

# Couchbase Vector Search MCP Server

#status/active #category/database #integration/couchbase #purpose/vector-search #tech/semantic #category/demo

## Description

Integrates Couchbase vector search for semantic similarity queries on Star Wars planet data. This server demonstrates vector search capabilities using a themed dataset.

## Features

- Vector search
- Semantic queries
- Similarity matching
- Data indexing
- Query optimization
- Result ranking
- Dataset management
- Search filtering
- Performance tuning
- Example queries

## Installation

```bash
npm install @shivay-couchbase/couchbase-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "couchbase-vector": {
      "command": "npx",
      "args": ["@shivay-couchbase/couchbase-mcp"],
      "env": {
        "COUCHBASE_URL": "your-couchbase-url",
        "COUCHBASE_USER": "your-username",
        "COUCHBASE_PASSWORD": "your-password",
        "BUCKET_NAME": "starwars",
        "VECTOR_DIM": "384"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Couchbase server
- Vector engine
- Search indexer
- Query processor
- Dataset loader

## Related Servers

- modelcontextprotocol-vector-server
- qdrant-mcp-server-qdrant
- modelcontextprotocol-search-server
