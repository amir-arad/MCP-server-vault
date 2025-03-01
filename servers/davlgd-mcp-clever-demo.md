--- 
type: server
repo_url: https://github.com/davlgd/mcp-clever-demo
name: Clever Cloud Demo MCP Server
owner: davlgd
stars: 1
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/cloud",
    "integration/clever-cloud",
    "purpose/deployment",
    "purpose/environment-management",
    "tech/paas",
  ]
---

# Clever Cloud Demo MCP Server

#status/active #category/cloud #integration/clever-cloud #purpose/deployment #purpose/environment-management #tech/paas

## Description

Integrates with Clever Cloud's tools and services to enable application deployment, environment management, and resource monitoring. This MCP server provides a demonstration of Clever Cloud platform capabilities.

## Features

- Application deployment
- Environment management
- Resource monitoring
- Service integration
- Configuration handling
- Log management
- Scaling controls
- Domain management
- SSL certificate handling
- Backup management

## Installation

To use this server in an MCP client such as Claude Desktop:

## Usage

```javascript
{
  "mcp-clever-demo": {
    "command": "npx",
    "args": [ "-y", "mcp-clever-demo" ]
  }
}
```

## Dependencies

- Node.js >= 16
- Clever Cloud account
- API credentials
- Git
- Environment manager
- Resource monitor

## Related Servers

- cf-toolsuite-butler
- cloudflare-mcp-server-cloudflare
- modelcontextprotocol-cloud-server