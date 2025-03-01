---
type: server
repo_url: https://github.com/kazuph/mcp-browser-tabs
name: Browser Tabs MCP Server
owner: kazuph
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/browser",
    "tech/applescript",
    "tech/javascript",
    "purpose/tab-management",
    "tech/macos",
  ]
---

# Browser Tabs MCP Server

#status/active #category/browser #tech/applescript #purpose/tab-management #tech/macos

## Description

Enables interaction with Google Chrome tabs through the MCP protocol, allowing clients to retrieve information and control tabs on macOS using AppleScript.

## Features

- Chrome tab control
- Tab information retrieval
- AppleScript integration
- macOS support
- Tab management
- Window control
- Session handling
- State tracking

## Installation

```bash
npm install @kazuph/mcp-browser-tabs
```

## Usage

```javascript
{
  "mcpServers": {
    "browser-tabs": {
      "command": "npx",
      "args": ["@kazuph/mcp-browser-tabs"],
      "env": {
        "BROWSER": "Google Chrome",
        "MAX_TABS": "50",
        "REFRESH_INTERVAL": "1000",
        "ALLOW_CLOSE": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- macOS
- Google Chrome
- AppleScript permissions

## Related Servers

- hrmeetsingh/mcp-browser-automation
- JovaniPink/mcp-browser-use
- Saik0s/mcp-browser-use
