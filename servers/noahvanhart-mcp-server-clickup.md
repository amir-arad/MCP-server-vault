---
type: server
repo_url: https://github.com/noahvanhart/mcp-server-clickup
name: ClickUp Integration MCP Server
owner: noahvanhart
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/clickup",
    "purpose/task-management",
    "purpose/workflow",
    "tech/api",
  ]
---

# ClickUp Integration MCP Server

#status/active #category/productivity #integration/clickup #purpose/task-management #purpose/workflow #tech/api

## Description

Integrates with ClickUp to enable task management, project tracking, and workflow optimization within the platform's ecosystem. This MCP server provides comprehensive access to ClickUp's features for automated project management.

## Features

- Task management
- Project tracking
- Workflow optimization
- Team collaboration
- Time tracking
- Custom field handling
- Automation rules
- Report generation
- Goal tracking
- Integration management

## Installation

```bash
npm install @noahvanhart/mcp-server-clickup
```

## Usage

```javascript
{
  "mcpServers": {
    "clickup": {
      "command": "npx",
      "args": ["@noahvanhart/mcp-server-clickup"],
      "env": {
        "CLICKUP_TOKEN": "your-api-token",
        "WORKSPACE_ID": "your-workspace-id",
        "DEFAULT_LIST": "your-list-id",
        "WEBHOOK_URL": "your-webhook-url",
        "LOG_LEVEL": "info"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- ClickUp account
- API token
- Webhook support
- Event handler
- Data validator

## Related Servers

- mikah13/mcp-clickup
- nazruden/clickup-mcp-server
- taazkareem/clickup-mcp-server
