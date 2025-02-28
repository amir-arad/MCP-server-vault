---
type: server
repo_url: https://github.com/ztobs/cline-browser-use-mcp
name: Cline Browser Automation MCP Server
owner: ztobs
stars: 11
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/automation",
    "tech/python",
    "purpose/browser-automation",
    "purpose/web-scraping",
    "tech/selenium",
  ]
---

# Cline Browser Automation MCP Server

#status/active #category/automation #tech/python #purpose/browser-automation #purpose/web-scraping #tech/selenium

## Description

Enables browser automation using Python scripts, offering operations like taking webpage screenshots, retrieving HTML content, and executing JavaScript. This MCP server provides comprehensive browser control capabilities.

## Features

- Screenshot capture
- HTML extraction
- JavaScript execution
- Browser automation
- Element interaction
- Page navigation
- Cookie management
- Form handling
- Network monitoring
- Error recovery

## Installation

```bash
npm install @ztobs/cline-browser-use-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "browser-automation": {
      "command": "npx",
      "args": ["@ztobs/cline-browser-use-mcp"],
      "env": {
        "BROWSER_TYPE": "chrome",
        "HEADLESS": "true",
        "SCREENSHOT_PATH": "./screenshots",
        "TIMEOUT": "30000",
        "USER_AGENT": "custom-user-agent"
      }
    }
  }
}
```

## Dependencies

- Python >= 3.8
- Selenium WebDriver
- Chrome/Firefox browser
- Screenshot library
- HTML parser
- JavaScript executor

## Related Servers

- modelcontextprotocol-puppeteer-server
- hrmeetsingh-mcp-browser-automation
- browserbase-mcp-server-browserbase
