---
type: server
repo_url: https://github.com/ravenwits/mcp-server-arangodb
name: ArangoDB MCP Server
owner: ravenwits
stars: 5
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags:
  [
    "status/active",
    "category/database",
    "integration/arangodb",
    "tech/typescript",
    "purpose/data-management",
  ]
---

# ArangoDB MCP Server

#status/active #category/database #integration/arangodb #tech/typescript #purpose/data-management

## Description

A TypeScript-based server to interact with ArangoDB using the Model Context Protocol, enabling database operations and integration with tools like Claude and VSCode extensions for streamlined data management.

## Features

- TypeScript implementation
- ArangoDB operations
- Claude integration
- VSCode extension support
- Data management
- Query building
- Schema validation
- Connection pooling

## Installation

```bash
npm install @ravenwits/mcp-server-arangodb
```

## Usage

```javascript
{
  "mcpServers": {
    "arangodb": {
      "command": "npx",
      "args": ["@ravenwits/mcp-server-arangodb"],
      "env": {
        "ARANGO_URL": "http://localhost:8529",
        "ARANGO_DATABASE": "your-database",
        "ARANGO_USER": "root",
        "ARANGO_PASSWORD": "your-password",
        "CONNECTION_POOL_SIZE": "5"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript >= 4.5
- ArangoDB instance
- Database credentials

## Related Servers

- lucas-deangelis/arango-mcp-server
