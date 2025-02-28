---
type: server
repo_url: https://github.com/lucas-deangelis/arango-mcp-server
name: Arango MCP Server
owner: lucas-deangelis
stars: 2
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/database", "integration/arangodb", "purpose/data-management", "tech/aql"]
---

# Arango MCP Server

#status/active #category/database #integration/arangodb #purpose/data-management #tech/aql

## Description

Integrates ArangoDB databases into workflows, enabling dynamic querying and analysis of document-oriented and graph data via AQL and document retrieval.

## Features

- ArangoDB integration
- AQL query support
- Document retrieval
- Graph data analysis
- Dynamic querying
- Collection management
- Index operations
- Transaction handling

## Installation

```bash
npm install @lucas-deangelis/arango-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "arango": {
      "command": "npx",
      "args": ["@lucas-deangelis/arango-mcp"],
      "env": {
        "ARANGO_URL": "http://localhost:8529",
        "ARANGO_DB": "your-database",
        "ARANGO_USERNAME": "root",
        "ARANGO_PASSWORD": "your-password"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- ArangoDB instance
- Database credentials
- AQL knowledge

## Related Servers

- ravenwits/mcp-server-arangodb