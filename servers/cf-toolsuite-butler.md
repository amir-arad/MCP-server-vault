---
type: server
repo_url: https://github.com/cf-toolsuite/cf-kaizen/tree/HEAD/butler
name: Butler MCP Server
owner: cf-toolsuite
stars: 1
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/cloud",
    "integration/cloud-foundry",
    "purpose/maintenance",
  ]
---

# Butler MCP Server

#status/active #category/cloud #integration/cloud-foundry #purpose/maintenance

## Description

Cleanup stale apps and services on a Cloud Foundry foundation.

## Features

- Stale app cleanup
- Service maintenance
- Foundation management
- Resource optimization
- Automated cleanup
- Policy enforcement
- Usage tracking
- Health monitoring

## Installation

```bash
npm install @cf-toolsuite/butler-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "butler": {
      "command": "npx",
      "args": ["@cf-toolsuite/butler-mcp"],
      "env": {
        "CF_API": "https://api.your-cf.com",
        "CF_USERNAME": "your-username",
        "CF_PASSWORD": "your-password",
        "STALE_THRESHOLD": "30d"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Cloud Foundry CLI
- CF account
- Admin privileges

## Related Servers

- None currently listed
