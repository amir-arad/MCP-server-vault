---
type: server
repo_url: https://github.com/d-kimuson/esa-mcp-server
name: Esa MCP Server
owner: d-kimuson
stars: 1
last_updated: 2025-01-25
status: active
official: false
verified: false
sources: ["inbox/batch_011.md"]
tags: ["status/active", "category/documentation", "integration/esa", "purpose/article-management", "purpose/search", "tech/api"]
---

# Esa MCP Server

#status/active #category/documentation #integration/esa #purpose/article-management #purpose/search #tech/api

## Description

Enables interaction with esa.io's API through the Model Context Protocol, supporting article search and retrieval with a compliant MCP interface.

## Features

- Article search functionality
- Content retrieval
- API integration
- MCP compliance
- Document management
- Search filtering
- Content organization
- Team collaboration
- Version tracking
- Access control

## Installation

```bash
npm install @d-kimuson/esa-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "esa": {
      "command": "npx",
      "args": ["@d-kimuson/esa-mcp-server"],
      "env": {
        "ESA_ACCESS_TOKEN": "your-access-token",
        "ESA_TEAM": "your-team-name",
        "CACHE_TTL": "3600",
        "MAX_RESULTS": "100"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- esa.io account
- API access token
- Team permissions
- Network connectivity

## Related Servers

- None currently listed