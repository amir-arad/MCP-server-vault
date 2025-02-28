---
type: server
repo_url: https://github.com/KS-GEN-AI/confluence-mcp-server
name: Confluence Query MCP Server
owner: KS-GEN-AI
stars: 0
last_updated: 2025-01-06
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/confluence",
    "purpose/search",
    "tech/cql",
    "purpose/content-retrieval",
  ]
---

# Confluence Query MCP Server

#status/active #category/productivity #integration/confluence #purpose/search #tech/cql #purpose/content-retrieval

## Description

Integrates with Confluence's API to execute CQL queries and retrieve page content, enabling efficient search and access of wiki information.

## Features

- CQL query execution
- Content retrieval
- Search functionality
- Page access
- Query optimization
- Result formatting
- Content caching
- Permission handling
- Error management
- Query validation

## Installation

```bash
npm install @ks-gen-ai/confluence-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "confluence-query": {
      "command": "npx",
      "args": ["@ks-gen-ai/confluence-mcp"],
      "env": {
        "CONFLUENCE_URL": "your-confluence-url",
        "API_TOKEN": "your-api-token",
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
- Confluence API access
- CQL parser
- Query executor
- Content formatter
- Cache system

## Related Servers

- mouhamadalmounayar/mcp-confluence
- aaronsb/confluence-cloud-mcp
- zereight/confluence-mcp
