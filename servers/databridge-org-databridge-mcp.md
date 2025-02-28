---
type: server
repo_url: https://github.com/databridge-org/databridge-mcp
name: DataBridge MCP Server
owner: databridge-org
stars: 0
last_updated: 2025-02-19
status: active
official: true
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "status/official",
    "category/data",
    "purpose/ingestion",
    "purpose/retrieval",
    "category/context",
  ]
---

# DataBridge MCP Server

#status/active #status/official #category/data #purpose/ingestion #purpose/retrieval #category/context

## Description

Integrates with DataBridge to enable ingestion and retrieval of contextual information from a local database, supporting persistent storage for AI applications.

## Features

- Data ingestion
- Context retrieval
- Local storage
- Persistence layer
- Context management
- Query capabilities
- Data organization
- Access control
- Backup support
- Search functionality

## Installation

```bash
npm install @databridge-org/databridge-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "databridge": {
      "command": "npx",
      "args": ["@databridge-org/databridge-mcp"],
      "env": {
        "DB_PATH": "./databridge-store",
        "MAX_CONTEXT_SIZE": "1000000",
        "INDEX_ENABLED": "true",
        "BACKUP_INTERVAL": "3600",
        "COMPRESSION": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Local database
- Context engine
- Search indexer
- Backup manager
- Query processor

## Related Servers

- modelcontextprotocol-memory-server
- fireproof-storage-mcp-database-server
- modelcontextprotocol-context-server
