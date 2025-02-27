---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/src/memory
name: Memory
owner: modelcontextprotocol
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
related_tags: ["category/knowledge-base", "status/official", "purpose/development", "tech/typescript"]
---

# Memory

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
import { Server } from '@modelcontextprotocol/sdk/server';
import { MemoryServer } from '@modelcontextprotocol/memory-server';

const server = new MemoryServer({
  storage: './memory-store'
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