---
type: server
repo_url: https://github.com/TrackerXXX23/dev_memory_mcp
name: Development Memory MCP Server
owner: TrackerXXX23
stars: 1
last_updated: 2024-12-22
status: active
official: false
verified: false
sources: ["inbox/batch_009.md"]
tags:
  [
    "status/active",
    "category/development",
    "purpose/memory",
    "purpose/context",
    "purpose/persistence",
    "tech/storage",
  ]
---

# Development Memory MCP Server

#status/active #category/development #purpose/memory #purpose/context #purpose/persistence #tech/storage

## Description

Provides persistent cross-project memory storage and retrieval for maintaining development context and knowledge across sessions.

## Features

- Cross-project memory
- Context persistence
- Knowledge storage
- Session management
- Context retrieval
- Data organization
- Search functionality
- Version tracking
- Context linking
- Export capabilities

## Installation

```bash
npm install @trackerxxx23/dev-memory-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "dev-memory": {
      "command": "npx",
      "args": ["@trackerxxx23/dev-memory-mcp"],
      "env": {
        "STORAGE_PATH": "./dev-memory",
        "MAX_CONTEXTS": "100",
        "PERSISTENCE_MODE": "file",
        "SEARCH_ENABLED": "true",
        "BACKUP_INTERVAL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Storage system
- Search engine
- Context manager
- Version control
- Backup system

## Related Servers

- modelcontextprotocol-memory-server
- davidteren-claude-server
- modelcontextprotocol-context-server
