---
type: server
repo_url: https://github.com/turlockmike/apple-notifier-mcp
name: Apple Notifier MCP Server
owner: turlockmike
stars: 3
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags:
  [
    "status/active",
    "category/notifications",
    "integration/apple",
    "tech/macos",
    "purpose/system-interaction",
  ]
---

To install Apple Notifier MCP Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/apple-notifier-mcp):

```bash
npx -y @smithery/cli install apple-notifier-mcp --client claude
```

# Apple Notifier MCP Server

#status/active #category/notifications #integration/apple #tech/macos #purpose/system-interaction

## Description

A simple MCP server that can send notifications on mac devices.

## Features

- macOS notifications
- Custom notification titles
- Message formatting
- Sound options
- Action buttons
- Notification scheduling
- Priority levels
- Notification center integration

## Installation

```bash
npm install @turlockmike/apple-notifier-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "apple-notifier": {
      "command": "npx",
      "args": ["@turlockmike/apple-notifier-mcp"],
      "env": {
        "DEFAULT_TITLE": "MCP Notification",
        "DEFAULT_SOUND": "default",
        "NOTIFICATION_TIMEOUT": "5000",
        "ALLOW_ACTIONS": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- macOS
- Notification Center access
- Terminal-notifier

## Related Servers

- Dhravya/apple-mcp
- RafalWilinski/mcp-apple-notes
- sirmews/apple-notes-mcp
