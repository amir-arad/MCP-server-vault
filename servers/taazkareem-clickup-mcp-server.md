---
type: server
repo_url: https://github.com/TaazKareem/clickup-mcp-server
name: ClickUp AI Integration MCP Server
owner: TaazKareem
stars: 8
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
    "category/ai",
    "purpose/resource-management",
  ]
---

# ClickUp AI Integration MCP Server

#status/active #category/productivity #integration/clickup #purpose/task-management #category/ai #purpose/resource-management

## Description

Enables AI integrations with ClickUp tasks, supporting resource management, task operations, workspace organization, and AI-powered task recommendations through a standardized protocol.

## Features

- AI task recommendations
- Resource management
- Task operations
- Workspace organization
- Smart scheduling
- Priority suggestions
- Workload balancing
- Automated tagging
- Performance analytics
- Integration automation

## Installation

```bash
npm install @taazkareem/clickup-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "clickup-ai": {
      "command": "npx",
      "args": ["@taazkareem/clickup-mcp"],
      "env": {
        "CLICKUP_API_KEY": "your-api-key",
        "AI_MODEL": "gpt-4",
        "WORKSPACE_ID": "your-workspace-id",
        "UPDATE_INTERVAL": "300",
        "ENABLE_SUGGESTIONS": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- ClickUp API access
- AI model integration
- Task analyzer
- Resource tracker
- Recommendation engine

## Related Servers

- mikah13/mcp-clickup
- noahvanhart/mcp-server-clickup
- nazruden/clickup-mcp-server
