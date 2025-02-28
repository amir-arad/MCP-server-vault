---
type: server
repo_url: https://github.com/jakedahn/deno2-playwright-mcp-server
name: Deno Playwright MCP Server
owner: jakedahn
stars: 7
last_updated: 2025-02-05
status: active
official: false
verified: false
sources: ["inbox/batch_009.md"]
tags:
  [
    "status/active",
    "category/automation",
    "tech/deno",
    "tech/playwright",
    "purpose/web-automation",
    "purpose/data-extraction",
  ]
---

# Deno Playwright MCP Server

#status/active #category/automation #tech/deno #tech/playwright #purpose/web-automation #purpose/data-extraction

## Description

Integrates with Playwright and Deno to enable browser automation for web navigation, interaction, and data extraction tasks. This server combines Deno's runtime with Playwright's automation capabilities.

## Features

- Browser automation
- Web navigation
- Data extraction
- Element interaction
- Screenshot capture
- Network monitoring
- Page manipulation
- Event handling
- Error recovery
- Session management

## Installation

```bash
npm install @jakedahn/deno2-playwright-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "deno-playwright": {
      "command": "npx",
      "args": ["@jakedahn/deno2-playwright-mcp"],
      "env": {
        "BROWSER_TYPE": "chromium",
        "HEADLESS": "true",
        "TIMEOUT": "30000",
        "SCREENSHOT_DIR": "./screenshots",
        "USER_AGENT": "custom-agent"
      }
    }
  }
}
```

## Dependencies

- Deno >= 1.0
- Playwright
- Browser engines
- Screenshot tool
- Network monitor
- Event handler

## Related Servers

- modelcontextprotocol-puppeteer-server
- browserbase-mcp-server-browserbase
- hrmeetsingh-mcp-browser-automation
