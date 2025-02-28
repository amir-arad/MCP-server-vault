---
type: server
repo_url: https://github.com/liuyoshio/mcp-compass
name: MCP Compass Server
owner: liuyoshio
stars: 11
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/discovery",
    "purpose/recommendation",
    "purpose/search",
    "category/ai",
    "purpose/understanding",
  ]
---

# MCP Compass Server

#status/active #category/discovery #purpose/recommendation #purpose/search #category/ai #purpose/understanding

## Description

MCP Compass is a discovery and recommendation service that assists AI assistants in finding and understanding Model Context Protocol servers through natural language queries.

## Features

- Server discovery
- Recommendation engine
- Natural language queries
- Server understanding
- Capability matching
- Usage suggestions
- Documentation access
- Relevance ranking
- Server comparison
- Integration guidance

## Installation

```bash
npm install @liuyoshio/mcp-compass
```

## Usage

```javascript
{
  "mcpServers": {
    "compass": {
      "command": "npx",
      "args": ["@liuyoshio/mcp-compass"],
      "env": {
        "INDEX_UPDATE": "3600",
        "MAX_RESULTS": "10",
        "EMBEDDING_MODEL": "all-MiniLM-L6-v2",
        "CACHE_TTL": "86400",
        "SIMILARITY_THRESHOLD": "0.8"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Vector database
- Search engine
- NLP processor
- Recommendation system
- Documentation parser

## Related Servers

- chatmcp/mcp-server-collector
- modelcontextprotocol-discovery-server
- modelcontextprotocol-registry-server
