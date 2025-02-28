---
type: server
repo_url: https://github.com/akseyh/bear-mcp-server
name: Bear MCP Server
owner: akseyh
stars: 12
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/bear",
    "purpose/note-management",
    "tech/macos",
  ]
---

# Bear MCP Server

#status/active #category/productivity #integration/bear #purpose/note-management #tech/macos

## Description

Allows the AI to read from your Bear Notes.

## Features

- Note reading
- Content access
- Search functionality
- Tag filtering
- Note metadata
- Content parsing
- Data synchronization
- Access control

## Installation

```bash
npm install @akseyh/bear-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "bear": {
      "command": "npx",
      "args": ["@akseyh/bear-mcp"],
      "env": {
        "BEAR_DATABASE_PATH": "~/Library/Group Containers/9K33E3U3T4.net.shinyfrog.bear/Application Data/database.sqlite",
        "READ_ONLY": "true",
        "CACHE_DURATION": "300",
        "MAX_RESULTS": "100"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- macOS
- Bear app
- SQLite access

## Related Servers

- jkawamoto/mcp-bear
