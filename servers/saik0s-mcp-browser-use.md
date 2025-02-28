---
type: server
repo_url: https://github.com/Saik0s/mcp-browser-use
name: Browser Use MCP Server
owner: Saik0s
stars: 98
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/automation",
    "purpose/browser-control",
    "tech/browser-use",
    "purpose/agent-interaction",
    "tech/python",
  ]
---

# Browser Use MCP Server

#status/active #category/automation #purpose/browser-control #tech/browser-use #purpose/agent-interaction

## Description

Facilitates browser automation with custom capabilities and agent-based interactions, integrated through the browser-use library.

## Features

- Browser automation
- Custom capabilities
- Agent interactions
- Browser control
- Task automation
- Event handling
- State management
- Performance monitoring

## Installation

```bash
npm install @saik0s/mcp-browser-use
```

## Usage

```javascript
{
  "mcpServers": {
    "browser-use": {
      "command": "npx",
      "args": ["@saik0s/mcp-browser-use"],
      "env": {
        "BROWSER_ENGINE": "chromium",
        "AGENT_CONFIG": "./agent.json",
        "AUTOMATION_DELAY": "100",
        "DEBUG_MODE": "false"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- browser-use library
- Browser engine
- Agent configuration

## Related Servers

- adamdude828/mcp-browser-use
- JovaniPink/mcp-browser-use
- hrmeetsingh/mcp-browser-automation
