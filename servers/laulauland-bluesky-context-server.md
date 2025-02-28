---
type: server
repo_url: https://github.com/laulauland/bluesky-context-server
name: Bluesky Context Server
owner: laulauland
stars: 10
last_updated: 2025-02-06
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/social-media",
    "integration/bluesky",
    "purpose/query",
    "category/context",
  ]
---

# Bluesky Context Server

#status/active #category/social-media #integration/bluesky #purpose/query #category/context

## Description

A simple MCP server that can enable MCP clients to query Bluesky instances.

## Features

- Bluesky instance querying
- MCP client integration
- Data retrieval
- Instance monitoring
- User data access
- Content search
- Feed management
- API interaction

## Installation

```bash
npm install @laulauland/bluesky-context
```

## Usage

```javascript
{
  "mcpServers": {
    "bluesky-context": {
      "command": "npx",
      "args": ["@laulauland/bluesky-context"],
      "env": {
        "BLUESKY_HOST": "bsky.social",
        "BLUESKY_HANDLE": "your-handle",
        "BLUESKY_APP_PASSWORD": "your-app-password",
        "CACHE_TTL": "300"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Bluesky account
- API credentials
- Network access

## Related Servers

- morinokami/mcp-server-bluesky
- keturiosakys/bluesky-context-server
- berlinbra/BlueSky-MCP
