---
type: server
repo_url: https://github.com/jkawamoto/mcp-bear
name: Bear MCP Server
owner: jkawamoto
stars: 4
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
    "tech/javascript",
  ]
---

# Bear MCP Server

#status/active #category/productivity #integration/bear #purpose/note-management #tech/macos

## Description

Facilitates interaction with Bear note-taking software, allowing users to perform actions like opening notes, creating notes, and searching through Bear's X-callback-url Scheme.

## Features

- Note creation
- Note opening
- Search functionality
- X-callback-url support
- Tag management
- Content organization
- Note linking
- Export options

## Installation

```bash
npm install @jkawamoto/mcp-bear
```

## Usage

```javascript
{
  "mcpServers": {
    "bear": {
      "command": "npx",
      "args": ["@jkawamoto/mcp-bear"],
      "env": {
        "BEAR_TOKEN": "your-bear-token",
        "DEFAULT_TAG": "inbox",
        "SEARCH_LIMIT": "50",
        "EXPORT_FORMAT": "markdown"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- macOS
- Bear app
- X-callback-url support

## Related Servers

- akseyh/bear-mcp-server
