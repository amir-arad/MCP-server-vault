---
type: server
repo_url: https://github.com/LostInBrittany/clever-doc-mcp-server
name: Clever Cloud Documentation MCP Server
owner: LostInBrittany
stars: 0
last_updated: 2025-01-29
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/documentation",
    "integration/clever-cloud",
    "purpose/knowledge-base",
    "purpose/query",
    "tech/typescript",
  ]
---

# Clever Cloud Documentation MCP Server

#status/active #category/documentation #integration/clever-cloud #purpose/knowledge-base #purpose/query #tech/typescript

## Description

The MCP server provides access to Clever Cloud's documentation, allowing users to query and interact with it through Model Context Protocol clients like Claude Desktop.

## Features

- Documentation access
- Content querying
- Search functionality
- Version tracking
- Topic navigation
- Example code retrieval
- API documentation
- Tutorial access
- Content indexing
- Update notifications

## Installation

```bash
npm install @lostinbrittany/clever-doc-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "clever-docs": {
      "command": "npx",
      "args": ["@lostinbrittany/clever-doc-mcp"],
      "env": {
        "DOC_SOURCE": "https://api.clever-cloud.com/docs",
        "CACHE_TTL": "3600",
        "MAX_RESULTS": "10",
        "SEARCH_DEPTH": "3",
        "INDEX_UPDATE": "daily"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Documentation indexer
- Search engine
- Cache system
- Content parser
- Version tracker

## Related Servers

- davlgd-mcp-clever-demo
- modelcontextprotocol-docs-server
- mendableai-firecrawl-mcp-server
