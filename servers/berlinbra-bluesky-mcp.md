---
type: server
repo_url: https://github.com/berlinbra/BlueSky-MCP
name: BlueSky MCP Server
owner: berlinbra
stars: 1
last_updated: 2025-01-31
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

# BlueSky MCP Server

#status/active #category/social-media #integration/bluesky #purpose/social-networking

## Description

Facilitates interaction with the BlueSky social network via its official API, allowing users to retrieve detailed user profiles and following lists with authentication and error handling capabilities.

## Features

- User profile retrieval
- Following list management
- Authentication handling
- Error management
- API integration
- Profile analysis
- Data validation
- Rate limiting

## Installation

```bash
npm install @berlinbra/bluesky-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "bluesky": {
      "command": "npx",
      "args": ["@berlinbra/bluesky-mcp"],
      "env": {
        "BLUESKY_IDENTIFIER": "your-handle.bsky.social",
        "BLUESKY_APP_PASSWORD": "your-app-password",
        "RATE_LIMIT": "100",
        "CACHE_DURATION": "300"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- BlueSky account
- API credentials
- Network access

## Related Servers

- morinokami/mcp-server-bluesky
- keturiosakys/bluesky-context-server
- laulauland/bluesky-context-server
