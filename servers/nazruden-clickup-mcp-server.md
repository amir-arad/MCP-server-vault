---
type: server
repo_url: https://github.com/Nazruden/clickup-mcp-server
name: ClickUp OAuth MCP Server
owner: Nazruden
stars: 4
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
    "tech/oauth",
    "category/ai",
  ]
---

# ClickUp OAuth MCP Server

#status/active #category/productivity #integration/clickup #purpose/task-management #tech/oauth #category/ai

## Description

This server integrates AI assistants with ClickUp workspaces, enabling task, team, list, and board management through a secure OAuth2 authentication process.

## Features

- OAuth2 authentication
- Task management
- Team organization
- List handling
- Board management
- Secure access
- Permission control
- Token management
- Workspace integration
- Event handling

## Installation

```bash
npm install @nazruden/clickup-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "clickup-oauth": {
      "command": "npx",
      "args": ["@nazruden/clickup-mcp"],
      "env": {
        "OAUTH_CLIENT_ID": "your-client-id",
        "OAUTH_CLIENT_SECRET": "your-client-secret",
        "REDIRECT_URI": "your-redirect-uri",
        "SCOPES": "team task workspace",
        "TOKEN_STORE": "./tokens"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- OAuth2 provider
- Token storage
- Permission handler
- Event system
- Cache manager

## Related Servers

- mikah13/mcp-clickup
- noahvanhart/mcp-server-clickup
- taazkareem/clickup-mcp-server
