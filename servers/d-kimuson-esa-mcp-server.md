---
type: server
repo_url: https://github.com/d-kimuson/esa-mcp-server
name: Esa MCP Server
owner: d-kimuson
stars: 1
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/documentation",
    "integration/esa",
    "purpose/article-management",
    "purpose/search",
    "tech/api",
  ]
---

# Esa MCP Server

#status/active #category/documentation #integration/esa #purpose/article-management #purpose/search #tech/api

## Description

Enables interaction with esa.io's API through the Model Context Protocol, supporting article search and retrieval with a compliant MCP interface.

## Features

- esa.io の記事検索
- 記事の詳細取得（単一・複数）
- MCP 準拠のインターフェース提供

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
