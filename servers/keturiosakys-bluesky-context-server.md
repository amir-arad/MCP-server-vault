---
type: server
repo_url: https://github.com/keturiosakys/bluesky-context-server
name: Bluesky Context Server
owner: keturiosakys
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

A simple MCP server that allows Claude Desktop to query Bluesky instances.

## Features

- Bluesky instance querying
- Claude Desktop integration
- Data retrieval
- Context analysis
- Feed monitoring
- User lookup
- Content search
- Real-time updates

## Installation

```bash
npm install @keturiosakys/bluesky-context
```

## Usage

```javascript
{
  "mcpServers": {
    "bluesky-context": {
      "command": "npx",
      "args": ["@keturiosakys/bluesky-context"],
      "env": {
        "BLUESKY_SERVICE": "bsky.social",
        "BLUESKY_USERNAME": "your-username",
        "BLUESKY_APP_PASSWORD": "your-app-password",
        "QUERY_TIMEOUT": "30"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Bluesky account
- Claude Desktop
- API access

## Related Servers

- morinokami/mcp-server-bluesky
- laulauland/bluesky-context-server
- berlinbra/BlueSky-MCP
