--- 
type: server
repo_url: https://github.com/modelcontextprotocol/servers
name: Memory
owner: modelcontextprotocol
stars: 11500
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags:
  [
    "category/knowledge-base",
    "status/official",
    "purpose/development",
    "tech/typescript",
  ]
---

# Memory

#category/knowledge-base #status/official #purpose/development #tech/typescript

## Description

A reference MCP server that implements a knowledge graph-based persistent memory system. This server demonstrates how to maintain and query structured information across sessions.

## Features

- Knowledge graph data structure
- Persistent storage capabilities
- Query and traversal operations
- Relationship management
- Data versioning
- Memory context handling
- Cache management

## Installation

```bash
npm install @modelcontextprotocol/memory-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { MemoryServer } from "@modelcontextprotocol/memory-server";

const server = new MemoryServer({
  storage: "./memory-store",
});
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- TypeScript
- Graph database (e.g., Neo4j or custom implementation)

## Related Servers

- PostgreSQL Server - For relational data storage
- Sqlite Server - For embedded database storage