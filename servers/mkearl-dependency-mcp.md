---
type: server
repo_url: https://github.com/mkearl/dependency-mcp
name: Dependency Management MCP Server
owner: mkearl
stars: 5
last_updated: 2025-01-02
status: active
official: false
verified: false
sources: ["inbox/batch_009.md"]
tags:
  [
    "status/active",
    "category/development",
    "purpose/dependency-management",
    "purpose/analysis",
    "tech/caching",
    "purpose/tracking",
  ]
---

# Dependency Management MCP Server

#status/active #category/development #purpose/dependency-management #purpose/analysis #tech/caching #purpose/tracking

## Description

Manage and analyze project dependencies, offering caching and flexible configuration for efficient tracking across complex software ecosystems.

## Features

- Dependency tracking
- Analysis tools
- Cache management
- Configuration options
- Version control
- Update checking
- Conflict detection
- Security scanning
- Report generation
- Ecosystem support

## Installation

```bash
npm install @mkearl/dependency-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "dependency-mgmt": {
      "command": "npx",
      "args": ["@mkearl/dependency-mcp"],
      "env": {
        "CACHE_PATH": "./dep-cache",
        "CACHE_TTL": "86400",
        "SCAN_INTERVAL": "3600",
        "ECOSYSTEMS": "npm,pip,maven",
        "SECURITY_CHECK": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Package managers
- Cache system
- Analysis tools
- Security scanner
- Report generator

## Related Servers

- daipendency/daipendency-mcp
- modelcontextprotocol-dependency-server
- modelcontextprotocol-security-server
