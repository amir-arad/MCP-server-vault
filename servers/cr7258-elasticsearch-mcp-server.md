---
type: server
repo_url: https://github.com/cr7258/elasticsearch-mcp-server
name: Elasticsearch MCP Server
owner: cr7258
stars: 10
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/search",
    "integration/elasticsearch",
    "purpose/cluster-management",
    "purpose/search",
    "purpose/indexing",
  ]
---

# Elasticsearch MCP Server

#status/active #category/search #integration/elasticsearch #purpose/cluster-management #purpose/search #purpose/indexing

## Description

Facilitates interaction with Elasticsearch clusters by allowing users to perform index operations, document searches, and cluster management via a Model Context Protocol server and natural language commands.

## Features

- Cluster management
- Index operations
- Document searching
- Natural language commands
- Cluster monitoring
- Index optimization
- Shard management
- Backup operations
- Security configuration
- Performance tuning

## Installation

```bash
npm install @cr7258/elasticsearch-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "elasticsearch": {
      "command": "npx",
      "args": ["@cr7258/elasticsearch-mcp-server"],
      "env": {
        "ES_HOSTS": "http://localhost:9200",
        "ES_USERNAME": "elastic",
        "ES_PASSWORD": "your-password",
        "CLUSTER_NAME": "my-cluster"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Elasticsearch >= 7.x
- Elasticsearch client
- Natural language processing libraries
- Cluster access permissions

## Related Servers

- [Elasticsearch MCP Server](https://github.com/da1y/mcp-server-elasticsearch) - Alternative Elasticsearch implementation
