---
type: server
repo_url: https://github.com/mikah13/mcp-clickup
name: ClickUp MCP Server
owner: mikah13
stars: 1
last_updated: 2025-02-18
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/clickup",
    "purpose/task-management",
    "purpose/project-management",
    "tech/api",
  ]
---

# ClickUp MCP Server

#status/active #category/productivity #integration/clickup #purpose/task-management #purpose/project-management #tech/api

## Description

MCP Server for the ClickUp API, providing integration capabilities for task and project management within the ClickUp platform.

## Features

- Task management
- Project tracking
- Team collaboration
- Status updates
- Due date handling
- Priority management
- Custom field support
- Comment integration
- Attachment handling
- Notification system

## Installation

```bash
npm install @mikah13/mcp-clickup
```

## Usage

```javascript
{
  "mcpServers": {
    "clickup": {
      "command": "npx",
      "args": ["@mikah13/mcp-clickup"],
      "env": {
        "CLICKUP_API_TOKEN": "your-api-token",
        "WORKSPACE_ID": "your-workspace-id",
        "DEFAULT_SPACE": "your-space-id",
        "CACHE_TTL": "3600",
        "DEBUG_MODE": "false"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- ClickUp account
- API token
- Cache system
- HTTP client
- JSON parser

## Related Servers

- noahvanhart/mcp-server-clickup
- nazruden/clickup-mcp-server
- taazkareem/clickup-mcp-server
