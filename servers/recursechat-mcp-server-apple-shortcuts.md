---
type: server
repo_url: https://github.com/recursechat/mcp-server-apple-shortcuts
name: Apple Shortcuts MCP Server
owner: recursechat
stars: 56
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/automation", "integration/apple", "tech/macos", "purpose/workflow-automation"]
---

# Apple Shortcuts MCP Server

#status/active #category/automation #integration/apple #tech/macos #purpose/workflow-automation

## Description

An MCP Server Integration with Apple Shortcuts.

## Features

- Shortcuts integration
- Workflow automation
- Custom actions
- Shortcut execution
- Parameter passing
- Result handling
- Error management
- System integration

## Installation

```bash
npm install @recursechat/mcp-server-apple-shortcuts
```

## Usage

```javascript
{
  "mcpServers": {
    "apple-shortcuts": {
      "command": "npx",
      "args": ["@recursechat/mcp-server-apple-shortcuts"],
      "env": {
        "SHORTCUTS_PATH": "~/Library/Shortcuts",
        "DEFAULT_TIMEOUT": "30000",
        "ALLOW_SYSTEM_EVENTS": "true",
        "LOG_LEVEL": "info"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- macOS
- Apple Shortcuts app
- System Events permission

## Related Servers

- Dhravya/apple-mcp
- kennethreitz/mcp-applemusic
- joshrutkowski/applescript-mcp