---
type: server
repo_url: https://github.com/StuMason/coolify-mcp-server
name: Coolify MCP Server
owner: StuMason
stars: 0
last_updated: 2025-02-17
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/deployment",
    "integration/coolify",
    "purpose/application-management",
    "purpose/resource-management",
    "tech/api",
  ]
---

# Coolify MCP Server

#status/active #category/deployment #integration/coolify #purpose/application-management #purpose/resource-management #tech/api

## Description

Enables interaction with Coolify applications and resources through the Coolify API via a standardized interface, supporting application management operations such as listing, starting, stopping, restarting, and deploying.

## Features

- Application management
- Resource control
- Deployment handling
- Status monitoring
- Operation execution
- Configuration management
- Log access
- Environment control
- Service scaling
- Health checks

## Installation

```bash
npm install @stumason/coolify-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "coolify": {
      "command": "npx",
      "args": ["@stumason/coolify-mcp"],
      "env": {
        "COOLIFY_API_URL": "your-coolify-url",
        "COOLIFY_API_KEY": "your-api-key",
        "DEFAULT_PROJECT": "your-project",
        "AUTO_RESTART": "true",
        "LOG_LEVEL": "info"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Coolify API access
- Operation manager
- Status monitor
- Log handler
- Configuration system

## Related Servers

- modelcontextprotocol-deployment-server
- cf-toolsuite-butler
- cloudflare-mcp-server-cloudflare
