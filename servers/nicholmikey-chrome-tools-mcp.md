---
type: server
repo_url: https://github.com/nicholmikey/chrome-tools-MCP
name: Chrome Tools MCP Server
owner: nicholmikey
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/browser",
    "integration/chrome",
    "purpose/automation",
    "tech/devtools-protocol",
    "purpose/debugging",
  ]
---

# Chrome Tools MCP Server

#status/active #category/browser #integration/chrome #purpose/automation #tech/devtools-protocol #purpose/debugging

## Description

Integrates with Chrome's DevTools Protocol to enable remote control of browser tabs, including JavaScript execution, screenshot capture, and network traffic monitoring.

## Features

- Remote browser control
- JavaScript execution
- Screenshot capture
- Network monitoring
- Tab management
- Console logging
- DOM manipulation
- Performance profiling
- Resource tracking
- Security testing

## Installation

```bash
npm install @nicholmikey/chrome-tools-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "chrome-tools": {
      "command": "npx",
      "args": ["@nicholmikey/chrome-tools-mcp"],
      "env": {
        "CHROME_PATH": "path/to/chrome",
        "DEVTOOLS_PORT": "9222",
        "HEADLESS": "true",
        "MAX_TABS": "10",
        "DEBUG_MODE": "false"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Google Chrome
- Chrome DevTools Protocol
- WebSocket support
- Screenshot library
- Network analyzer

## Related Servers

- modelcontextprotocol-puppeteer-server
- cmann50-mcp-chrome-google-search
- browserbase-mcp-server-browserbase
