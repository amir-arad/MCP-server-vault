---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/src/postgres
name: PostgreSQL
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

# PostgreSQL

#category/database #status/official #purpose/development #tech/typescript

## Description

A reference MCP server that provides read-only database access with schema inspection capabilities for PostgreSQL databases. This server demonstrates safe database integration patterns.

## Features

- Read-only database access
- Schema inspection and metadata
- Query execution and results formatting
- Connection pooling
- Type mapping and conversion
- Query parameter validation
- Result set pagination

## Installation

```bash
npm install @modelcontextprotocol/postgres-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { PostgresServer } from "@modelcontextprotocol/postgres-server";

const server = new PostgresServer({
  connectionString: process.env.DATABASE_URL,
});
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- pg (node-postgres)
- TypeScript

## Related Servers

- Sqlite Server - For embedded database access
- Memory Server - For in-memory data storage
