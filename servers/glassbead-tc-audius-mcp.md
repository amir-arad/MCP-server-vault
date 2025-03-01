---
type: server
repo_url: https://github.com/glassBead-tc/audius-mcp
name: Audius MCP Server
owner: glassBead-tc
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "category/music",
    "integration/audius",
    "purpose/content-management",
    "tech/javascript",
  ]
---

# Audius MCP Server

#status/active #category/music #integration/audius #purpose/content-management

## Description

Enables interaction with the Audius music platform API, supporting user, track, and playlist operations through the Model Context Protocol.

## Features

- User profile management
- Track operations
- Playlist management
- API integration
- Music streaming
- Content discovery
- Metadata handling
- Search functionality

## Installation

```bash
npm install @glassbead-tc/audius-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "audius": {
      "command": "npx",
      "args": ["@glassbead-tc/audius-mcp"],
      "env": {
        "AUDIUS_APP_NAME": "your-app-name",
        "AUDIUS_API_KEY": "your-api-key",
        "DEFAULT_ENDPOINT": "https://api.audius.co",
        "CACHE_DURATION": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Audius API access
- API credentials
- Network connectivity

## Related Servers

- None currently listed
