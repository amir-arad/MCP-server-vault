---
type: server
repo_url: https://github.com/ALX99/db-mcp
name: Multi-Database MCP Server
owner: ALX99
stars: 0
last_updated: 2025-02-12
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/database",
    "tech/postgresql",
    "tech/mysql",
    "tech/sqlite",
    "purpose/query-execution",
  ]
---

# Multi-Database MCP Server

#status/active #category/database #tech/postgresql #tech/mysql #tech/sqlite #purpose/query-execution

## Description

Connects AI models to multiple database systems for executing queries and retrieving results across PostgreSQL, MySQL, and SQLite databases.

## Features

- Multi-database support
- Query execution
- Result retrieval
- Connection pooling
- Query validation
- Error handling
- Transaction support
- Schema inspection
- Result formatting
- Connection management

## Installation

```bash
npm install @alx99/db-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "multi-db": {
      "command": "npx",
      "args": ["@alx99/db-mcp"],
      "env": {
        "PG_CONNECTION": "postgresql://user:pass@host/db",
        "MYSQL_CONNECTION": "mysql://user:pass@host/db",
        "SQLITE_PATH": "./database.sqlite",
        "MAX_POOL_SIZE": "10",
        "TIMEOUT": "30000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- PostgreSQL client
- MySQL client
- SQLite3
- Query parser
- Connection pool
- Result formatter

## Related Servers

- modelcontextprotocol-postgres-server
- modelcontextprotocol-sqlite-server
- fireproof-storage-mcp-database-server
