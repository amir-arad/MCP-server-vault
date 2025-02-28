---
type: server
repo_url: https://github.com/KS-GEN-AI/confluence-mcp-server
name: Confluence Query MCP Server
owner: KS-GEN-AI
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/confluence",
    "purpose/search",
    "tech/cql",
    "purpose/content-retrieval",
    "tech/javascript",
    "tech/typescript",
    "tech/nodejs"
  ]
---

# Confluence Query MCP Server

#status/active #category/productivity #integration/confluence #purpose/search #tech/cql #purpose/content-retrieval #tech/javascript #tech/typescript #tech/nodejs

## Description

A TypeScript-based MCP server that integrates with Confluence's API to execute CQL queries and retrieve page content, enabling efficient search and access of wiki information. The server provides a standardized interface for AI assistants to interact with Confluence content.

## Features

- CQL query execution with customizable limits
- Content retrieval and formatting
- Advanced search functionality
- Page content access and parsing
- Query optimization and validation
- Result formatting and processing
- Content caching for performance
- Permission handling and security
- Error management and logging
- Cross-platform support (Windows/Mac)

## Installation

```bash
npm install @ks-gen-ai/confluence-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "confluence-query": {
      "command": "node",
      "args": ["/path/to/build/index.js"],
      "env": {
        "CONFLUENCE_URL": "your-confluence-url",
        "CONFLUENCE_API_MAIL": "your-email",
        "CONFLUENCE_API_KEY": "your-api-token",
        "MAX_RESULTS": "100",
        "CACHE_TTL": "3600",
        "DEFAULT_SPACE": "your-space"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript runtime
- Confluence API access
- CQL parser and executor
- Query optimizer
- Content formatter
- Cache system
- MCP Inspector (for debugging)

## Related Servers

- mouhamadalmounayar/mcp-confluence
- aaronsb/confluence-cloud-mcp
- zereight/confluence-mcp