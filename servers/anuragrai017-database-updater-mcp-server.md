---
type: server
repo_url: https://github.com/AnuragRai017/database-updater-MCP-Server
name: Database Updater MCP Server
owner: AnuragRai017
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/database",
    "purpose/data-migration",
    "purpose/synchronization",
    "tech/csv",
    "tech/excel",
  ]
---

# Database Updater MCP Server

#status/active #category/database #purpose/data-migration #purpose/synchronization #tech/csv #tech/excel

## Description

Streamlines database updates from CSV and Excel files, supporting multiple database types for efficient data migration and synchronization tasks.

## Features

- CSV file processing
- Excel file handling
- Multi-database support
- Data migration
- Synchronization
- Schema mapping
- Data validation
- Error handling
- Progress tracking
- Rollback support

## Installation

```bash
npm install @anuragrai017/database-updater-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "db-updater": {
      "command": "npx",
      "args": ["@anuragrai017/database-updater-mcp"],
      "env": {
        "SOURCE_PATH": "./data-files",
        "DB_TYPE": "postgresql",
        "DB_URL": "your-db-url",
        "BATCH_SIZE": "1000",
        "VALIDATE_DATA": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Database drivers
- CSV parser
- Excel parser
- Data validator
- Migration engine

## Related Servers

- modelcontextprotocol-database-server
- fireproof-storage-mcp-database-server
- modelcontextprotocol-migration-server
