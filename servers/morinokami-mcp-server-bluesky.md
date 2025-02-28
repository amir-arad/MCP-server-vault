---
type: server
repo_url: https://github.com/morinokami/mcp-server-bluesky
name: Bluesky MCP Server
owner: morinokami
stars: 1
last_updated: 2025-01-13
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/social-media",
    "integration/bluesky",
    "purpose/social-networking",
  ]
---

# Bluesky MCP Server

#status/active #category/social-media #integration/bluesky #purpose/social-networking

## Description

Integrates with Bluesky's social network API to enable profile management, posting, following, and engagement actions.

## Features

- Profile management
- Post creation
- Following management
- Engagement tracking
- Content discovery
- Feed management
- User interactions
- Content moderation

## Installation

```bash
npm install @morinokami/mcp-server-bluesky
```

## Usage

```javascript
{
  "mcpServers": {
    "bluesky": {
      "command": "npx",
      "args": ["@morinokami/mcp-server-bluesky"],
      "env": {
        "BLUESKY_IDENTIFIER": "your-handle.bsky.social",
        "BLUESKY_PASSWORD": "your-app-password",
        "DEFAULT_FEED": "following",
        "POST_LIMIT": "50"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Bluesky account
- API access
- Network connectivity

## Related Servers

- keturiosakys/bluesky-context-server
- laulauland/bluesky-context-server
- berlinbra/BlueSky-MCP
