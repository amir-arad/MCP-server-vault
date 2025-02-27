---
type: server
repo_url: https://github.com/neo4j-contrib/mcp-neo4j/
name: Neo4j
owner: neo4j-contrib
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/database"]
---

#status/active #status/official #category/database

# Neo4j

## Description

Neo4j graph database server (schema + read/write-cypher) and separate graph database backed memory. This MCP server provides comprehensive integration with Neo4j's graph database capabilities, enabling powerful graph data operations and analysis.

## Features

- Graph database operations
- Cypher query execution
- Schema management
- Graph data modeling
- CRUD operations
- Transaction management
- Graph traversal
- Memory-backed storage
- Real-time graph updates
- Query optimization

## Installation

```bash
npm install @neo4j/mcp-server
```

## Usage

```javascript
import { Neo4jServer } from "@neo4j/mcp-server";

const server = new Neo4jServer({
  uri: "neo4j://localhost:7687",
  username: "neo4j",
  password: "your-password",
});

// Execute Cypher query
const results = await server.query({
  cypher: `
    MATCH (p:Person)-[:FOLLOWS]->(f:Person)
    WHERE p.name = $name
    RETURN f.name as follower, f.age as age
  `,
  params: {
    name: "John Doe",
  },
});

// Create graph schema
await server.createSchema({
  nodes: [
    {
      label: "Person",
      properties: {
        name: "STRING",
        age: "INTEGER",
        email: "STRING",
      },
      constraints: [
        {
          type: "UNIQUE",
          properties: ["email"],
        },
      ],
    },
  ],
  relationships: [
    {
      type: "FOLLOWS",
      properties: {
        since: "DATETIME",
      },
    },
  ],
});

// Use graph memory backend
const memoryGraph = await server.createMemoryGraph({
  name: "temp-graph",
  config: {
    maxNodes: 1000000,
    maxRelationships: 5000000,
  },
});
```

## Dependencies

- Node.js >= 14.x
- Neo4j database instance
- Neo4j authentication credentials

## Related Servers

- None currently listed
