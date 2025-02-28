---
type: server
repo_url: https://github.com/shivay-couchbase/couchbase-mcp
name: Couchbase Vector Search MCP Server
owner: shivay-couchbase
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/database",
    "integration/couchbase",
    "purpose/vector-search",
    "tech/semantic",
    "category/demo",
    "tech/typescript",
    "tech/javascript",
    "tech/vector-db"
  ]
---

# Couchbase Vector Search MCP Server

#status/active #category/database #integration/couchbase #purpose/vector-search #tech/semantic #category/demo #tech/typescript #tech/javascript #tech/vector-db

## Description

A TypeScript/JavaScript-based MCP server that demonstrates semantic search capabilities using Couchbase's vector search functionality. The server provides a standardized interface for querying and finding similar Star Wars planets based on vector embeddings, showcasing practical applications of vector search in a themed dataset.

## Features

- Vector-based semantic search
- Similarity matching with embeddings
- Efficient vector indexing
- Query optimization
- Result ranking and scoring
- Dataset management
- Search filtering
- Performance tuning
- Connection pooling
- Error handling
- Type-safe implementation
- Example queries and data

## Installation

```bash
# Install dependencies
npm install @shivay-couchbase/couchbase-mcp

# Or build from source
git clone https://github.com/shivay-couchbase/couchbase-mcp.git
cd couchbase-mcp
npm install
npm run build
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
        "VECTOR_DIM": "384",
        "TIMEOUT": "5000",
        "MAX_CONNECTIONS": "10"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript runtime
- Couchbase server with vector search capability
- Vector engine
- Search indexer
- Query processor
- Dataset loader
- Connection manager
- Error handler

## Related Servers

- modelcontextprotocol-vector-server
- qdrant-mcp-server-qdrant
- modelcontextprotocol-search-server