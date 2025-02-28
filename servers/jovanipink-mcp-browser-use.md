---
type: server
repo_url: https://github.com/JovaniPink/mcp-browser-use
name: Browser Use MCP Server
owner: JovaniPink
stars: 9
last_updated: 2025-02-17
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/automation",
    "purpose/browser-control",
    "category/ai",
    "purpose/web-interaction",
  ]
---

# Browser Use MCP Server

#status/active #category/automation #purpose/browser-control #category/ai #purpose/web-interaction

## Description

Enables AI agents to interact with web browsers using natural language, featuring automated browsing, form filling, vision-based element detection, and structured JSON responses for systematic browser control.

## Features

- Natural language control
- Automated browsing
- Form filling
- Element detection
- Vision-based interaction
- JSON response format
- Browser automation
- AI agent integration

## Installation

```bash
npm install @jovanipink/mcp-browser-use
```

## Usage

```javascript
{
  "mcpServers": {
    "browser-use": {
      "command": "npx",
      "args": ["@jovanipink/mcp-browser-use"],
      "env": {
        "BROWSER_TYPE": "chrome",
        "VISION_MODEL": "default",
        "TIMEOUT": "30000",
        "HEADLESS": "false"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Browser engine
- Vision models
- AI frameworks

## Related Servers

- adamdude828/mcp-browser-use
- Saik0s/mcp-browser-use
- hrmeetsingh/mcp-browser-automation
