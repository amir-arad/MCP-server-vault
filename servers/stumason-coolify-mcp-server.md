---
type: server
repo_url: https://github.com/StuMason/coolify-mcp-server
name: Coolify MCP Server
owner: StuMason
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/deployment",
    "integration/coolify",
    "purpose/application-management",
    "purpose/resource-management",
    "tech/javascript",
    "tech/api",
    "tech/typescript"
  ]
---

# Coolify MCP Server

#status/active #category/deployment #integration/coolify #purpose/application-management #purpose/resource-management #tech/javascript #tech/typescript #tech/api

## Description

A TypeScript-based MCP server that provides a standardized interface to interact with Coolify's API, enabling comprehensive management of applications and resources. The server supports operations like listing, starting, stopping, restarting, and deploying applications through a well-documented API interface.

## Features

- Resource listing and management
- Application lifecycle control
- Deployment automation
- Status monitoring
- Operation execution
- Configuration management
- Health checks
- Version tracking
- Environment control
- Service scaling

## Installation

```bash
# Via npm
npm install @stumason/coolify-mcp

# Build from source
git clone https://github.com/StuMason/coolify-mcp-server.git
cd coolify-mcp-server
npm install
npm run build
```

## Usage

```javascript
{
  "mcpServers": {
    "coolify": {
      "command": "node",
      "args": ["/path/to/build/index.js"],
      "env": {
        "COOLIFY_ACCESS_TOKEN": "your-api-key",
        "COOLIFY_BASE_URL": "https://your-coolify-url",
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
- TypeScript runtime
- Coolify API access
- Operation manager
- Status monitor
- Log handler
- Configuration system
- MCP Inspector (for debugging)

## Related Servers

- modelcontextprotocol-deployment-server
- cf-toolsuite-butler
- cloudflare-mcp-server-cloudflare