---
type: server
repo_url: https://github.com/turlockmike/apple-notifier-mcp
name: Apple Notifier MCP Server
owner: turlockmike
stars: 1
last_updated: 2024-12-23
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/notifications", "integration/apple", "tech/macos", "purpose/system-interaction"]
---

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