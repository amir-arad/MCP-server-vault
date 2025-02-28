---
type: server
repo_url: https://github.com/fireproof-storage/mcp-database-server
name: Fireproof Database MCP Server
owner: fireproof-storage
stars: 8
last_updated: 2025-02-09
status: active
official: true
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "status/official",
    "category/database",
    "tech/ledger",
    "purpose/sync",
    "purpose/storage",
  ]
---

# Fireproof Database MCP Server

#status/active #status/official #category/database #tech/ledger #purpose/sync #purpose/storage

## Description

Fireproof ledger database with multi-user sync. This server provides a secure, distributed database solution with built-in synchronization capabilities.

## Features

- Ledger database
- Multi-user sync
- Data integrity
- Transaction logging
- Conflict resolution
- Real-time updates
- User management
- Access control
- Audit trail
- Backup support

## Installation

```bash
npm install @fireproof-storage/database-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "fireproof-db": {
      "command": "npx",
      "args": ["@fireproof-storage/database-mcp"],
      "env": {
        "DB_PATH": "./fireproof-data",
        "SYNC_INTERVAL": "5000",
        "MAX_USERS": "100",
        "CONFLICT_STRATEGY": "last-write-wins",
        "BACKUP_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Ledger engine
- Sync manager
- User authenticator
- Conflict resolver
- Backup system

## Related Servers

- modelcontextprotocol-database-server
- neondatabase-mcp-server-neon
- motherduckdb-mcp-server-motherduck
