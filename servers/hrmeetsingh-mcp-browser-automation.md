---
type: server
repo_url: https://github.com/hrmeetsingh/mcp-browser-automation
name: Browser Automation MCP Server
owner: hrmeetsingh
stars: 3
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/automation",
    "tech/playwright",
    "purpose/browser-control",
    "integration/claude",
    "tech/javascript",
  ]
---

# Browser Automation MCP Server

#status/active #category/automation #tech/playwright #purpose/browser-control #integration/claude

## Description

Enables automation of browser tasks using Playwright by interacting via Claude Desktop for executing user-defined prompts and operations.

## Features

- Browser task automation
- Playwright integration
- Claude Desktop support
- Custom prompt execution
- Operation management
- Task scheduling
- Error handling
- Performance monitoring

## Installation

```bash
npm install @hrmeetsingh/mcp-browser-automation
```

## Usage

```javascript
{
  "mcpServers": {
    "browser-automation": {
      "command": "npx",
      "args": ["@hrmeetsingh/mcp-browser-automation"],
      "env": {
        "BROWSER_TYPE": "chromium",
        "HEADLESS": "true",
        "TIMEOUT": "30000",
        "SCREENSHOT_DIR": "./screenshots"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Playwright
- Claude Desktop
- Browser engines

## Related Servers

- kazuph/mcp-browser-tabs
- JovaniPink/mcp-browser-use
- Saik0s/mcp-browser-use
