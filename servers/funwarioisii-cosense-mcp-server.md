---
type: server
repo_url: https://github.com/funwarioisii/cosense-mcp-server
name: Cosense Integration MCP Server
owner: funwarioisii
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/project-management",
    "integration/cosense",
    "purpose/data-access",
    "purpose/collaboration",
    "purpose/workflow",
    "tech/javascript",
    "tech/typescript",
    "tech/bun"
  ]
---

# Cosense Integration MCP Server

#status/active #category/project-management #integration/cosense #purpose/data-access #purpose/collaboration #purpose/workflow #tech/javascript #tech/typescript #tech/bun

## Description

A TypeScript/JavaScript-based MCP server that provides seamless integration with Cosense's project management platform. The server enables access and interaction with project data, supporting both public and private projects through SID authentication.

## Features

- Project data access and management
- Page content retrieval
- Workflow integration
- Collaboration tools
- Project tracking
- Task organization
- Team coordination
- Progress monitoring
- Resource allocation
- Reporting capabilities
- Private project support via SID

## Installation

```bash
# Via npm
npm install @funwarioisii/cosense-mcp

# Build from source
git clone https://github.com/funwarioisii/cosense-mcp-server.git
cd cosense-mcp-server
npm install
npm run build
```

## Usage

```javascript
{
  "mcpServers": {
    "cosense": {
      "command": "npx",
      "args": ["@funwarioisii/cosense-mcp"],
      "env": {
        "COSENSE_API_URL": "your-cosense-url",
        "API_KEY": "your-api-key",
        "PROJECT_ID": "default-project",
        "COSENSE_SID": "your-sid",  // Optional, for private projects
        "UPDATE_INTERVAL": "300",
        "CACHE_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript runtime
- Bun package manager
- Cosense account
- API credentials
- Data processor
- Cache system
- Event handler
- MCP Inspector (for debugging)

## Related Servers

- yosider/cosense-mcp-server
- modelcontextprotocol-project-server
- roychri-mcp-server-asana