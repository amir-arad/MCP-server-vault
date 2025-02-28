---
type: server
repo_url: https://github.com/joshrutkowski/applescript-mcp
name: AppleScript MCP Server
owner: joshrutkowski
stars: 76
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/automation", "integration/apple", "tech/applescript", "tech/typescript", "purpose/system-control", "platform/macos"]
---

# AppleScript MCP Server

#status/active #category/automation #integration/apple #tech/applescript #tech/typescript #purpose/system-control #platform/macos

## Description

A Model Context Protocol server that enables LLM applications to interact with macOS through AppleScript. This server provides a standardized interface for AI applications to control system functions, manage files, handle notifications, and more.

## Features

- Calendar management (events, reminders)
- Clipboard operations (copy, paste, clear)
- Finder integration (file selection, search, preview)
- System notifications (send, toggle Do Not Disturb)
- System controls (volume, dark mode, app management)
- iTerm terminal integration
- Application automation
- UI scripting
- Window management
- Process control
- File operations

## Installation

```bash
# Install dependencies
npm install

# Build the server
npm run build
```

## Usage

```javascript
{
  "mcpServers": {
    "applescript": {
      "command": "npx",
      "args": ["@joshrutkowski/applescript-mcp"],
      "env": {
        "SCRIPT_PATH": "./scripts",
        "TIMEOUT": "5000",
        "ALLOW_UI_SCRIPTING": "true",
        "SANDBOX_MODE": "false"
      }
    }
  }
}
```

## Dependencies

- macOS 10.15 or later
- Node.js 18 or later
- AppleScript permissions
- System Events access
- TypeScript (for development)

## Related Servers

- Dhravya/apple-mcp - Alternative Apple integration
- kennethreitz/mcp-applemusic - Apple Music integration
- recursechat/mcp-server-apple-shortcuts - Apple Shortcuts integration
- sirmews/apple-notes-mcp - Apple Notes integration
- rafalwilinski/mcp-apple-notes - Another Apple Notes integration