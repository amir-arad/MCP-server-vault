--- 
type: server
repo_url: https://github.com/modelcontextprotocol/servers
name: Sqlite
owner: modelcontextprotocol
stars: 11500
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags:
  [
    "category/database",
    "status/official",
    "purpose/development",
    "tech/typescript",
  ]
---

# Sqlite

#category/database #status/official #purpose/development #tech/typescript

## Description

A reference MCP server that provides database interaction and business intelligence capabilities using SQLite. This server demonstrates embedded database integration patterns.

## Features

- Database creation and management
- Query execution and results formatting
- Schema manipulation
- Transaction handling
- Data import/export
- In-memory database support
- Query optimization

## Installation

```bash
npm install @modelcontextprotocol/sqlite-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { SqliteServer } from "@modelcontextprotocol/sqlite-server";

const server = new SqliteServer({
  database: ":memory:", // or path to file
});
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- sqlite3
- TypeScript

## Related Servers

- PostgreSQL Server - For full relational database capabilities
- Memory Server - For in-memory data storage