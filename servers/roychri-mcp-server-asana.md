---
type: server
repo_url: https://github.com/roychri/mcp-server-asana
name: Asana MCP Server
owner: roychri
stars: 10
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/asana",
    "purpose/task-management",
    "tech/nodejs",
  ]
---

# Asana MCP Server

#status/active #category/productivity #integration/asana #purpose/task-management

## Description

Perform Asana operations from an MCP Client such as Anthropic's Claude Desktop Application, and many more.

## Features

- Task management
- Project organization
- Team collaboration
- Workflow automation
- Due date tracking
- Assignment handling
- Comment integration
- Status updates

## Installation

```bash
npm install @roychri/mcp-server-asana
```

## Usage

```javascript
{
  "mcpServers": {
    "asana": {
      "command": "npx",
      "args": ["@roychri/mcp-server-asana"],
      "env": {
        "ASANA_ACCESS_TOKEN": "your-access-token",
        "DEFAULT_WORKSPACE": "your-workspace-id",
        "DEFAULT_PROJECT": "your-project-id",
        "SYNC_INTERVAL": "300"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Asana account
- Access token
- Workspace permissions

## Related Servers

- None currently listed
