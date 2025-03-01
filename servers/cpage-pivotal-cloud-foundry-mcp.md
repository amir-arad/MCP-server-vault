---
type: server
repo_url: https://github.com/cpage-pivotal/cloud-foundry-mcp
name: Cloud Foundry MCP Server
owner: cpage-pivotal
stars: 2
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/cloud",
    "integration/cloud-foundry",
    "purpose/application-management",
    "purpose/service-management",
    "tech/paas",
  ]
---

# Cloud Foundry MCP Server

#status/active #category/cloud #integration/cloud-foundry #purpose/application-management #purpose/service-management #tech/paas

## Description

Integrates with Cloud Foundry foundations to enable management of applications, services, and resources. This MCP server provides comprehensive control over Cloud Foundry deployments and operations.

## Features

- Application management
- Service provisioning
- Resource allocation
- Route management
- Log streaming
- Environment control
- Scale operations
- Health monitoring
- Backup management
- Security controls

## Installation

```bash
npm install @cpage-pivotal/cloud-foundry-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "cloud-foundry": {
      "command": "npx",
      "args": ["@cpage-pivotal/cloud-foundry-mcp"],
      "env": {
        "CF_API_URL": "https://api.your-cf.com",
        "CF_USERNAME": "your-username",
        "CF_PASSWORD": "your-password",
        "ORG_NAME": "your-org",
        "SPACE_NAME": "your-space"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Cloud Foundry CLI
- CF API access
- UAA client
- Service broker
- Resource manager

## Related Servers

- cf-toolsuite-butler
- cloudflare-mcp-server-cloudflare
- modelcontextprotocol-cloud-server
