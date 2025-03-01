--- 
type: server
repo_url: https://github.com/da1y/mcp-server-elasticsearch
name: Elasticsearch MCP Server
owner: da1y
stars: 1
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags: ["status/active", "category/search", "integration/elasticsearch", "purpose/indexing", "purpose/search", "tech/full-text-search"]
---

# Elasticsearch MCP Server

#status/active #category/search #integration/elasticsearch #purpose/indexing #purpose/search #tech/full-text-search

## Description

Integrates with Elasticsearch to enable index management, document indexing, and powerful search capabilities across large datasets.

## Features

- Index management
- Document indexing
- Full-text search
- Query optimization
- Index configuration
- Mapping management
- Aggregation support
- Cluster monitoring
- Document versioning
- Search analytics

## Installation

```bash
npm install @da1y/mcp-server-elasticsearch
```

## Usage

```javascript
{
  "mcpServers": {
    "elasticsearch": {
      "command": "npx",
      "args": ["@da1y/mcp-server-elasticsearch"],
      "env": {
        "ES_NODE": "http://localhost:9200",
        "ES_USERNAME": "elastic",
        "ES_PASSWORD": "your-password",
        "INDEX_PREFIX": "mcp-"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Elasticsearch >= 7.x
- Elasticsearch client
- Memory for indexing
- Storage space