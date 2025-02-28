---
type: server
repo_url: https://github.com/lucas-deangelis/arango-mcp-server
name: Arango MCP Server
owner: lucas-deangelis
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags:
  [
    "status/active",
    "category/database",
    "integration/arangodb",
    "purpose/data-management",
    "tech/aql",
  ]
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

### Tools

#### Query Tools

- `readQuery`
  - Execute read-only query on the database
  - Input:
    - `databaseName` (string): The database to query
    - `aql` (string): The read-only AQL query to execute
  - Returns: Query results as array of objects
- `readWriteQuery`
  - Execute query on the database
  - Input:
    - `databaseName` (string): The database to query
    - `aql` (string): The AQL query to execute
  - Returns: Query results as array of objects
- `listDatabases`
  - List all the databases on the ArangoDB server
  - Returns: Array of the databases names
- `listCollections`
  - List all the collections in an ArangoDB database
  - Input:
    - `databaseName` (string): The name of the database
  - Returns: Array of objects `{ "name": "<collectionName>" }`

## Usage

To connect to an arangodb instance running on localhost:2434, to the database "account", add the following to your `claude_desktop_config.json`, assuming the path to this project is `/home/yourcoolname/arango-mcp-server`:

```json
{
  "mcpServers": {
    "arangodb-account": {
      "command": "npx",
      "args": [
        "-y",
        "arango-mcp-server",
        "http://localhost:8529",
        "root",
        "root"
      ]
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
