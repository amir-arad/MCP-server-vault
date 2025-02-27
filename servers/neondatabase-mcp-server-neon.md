---
type: server
repo_url: https://github.com/neondatabase/mcp-server-neon
name: Neon
owner: neondatabase
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/database"]
---

#status/active #status/official #category/database

# Neon

## Description

Interact with the Neon serverless Postgres platform. This MCP server provides seamless integration with Neon's serverless PostgreSQL service, enabling scalable and efficient database operations.

## Features

- Serverless PostgreSQL operations
- Auto-scaling capabilities
- Connection management
- Query execution
- Database branching
- Backup and restore
- Performance monitoring
- Resource optimization
- Cost management
- Security controls

## Installation

```bash
npm install @neondatabase/mcp-server
```

## Usage

```javascript
import { NeonServer } from "@neondatabase/mcp-server";

const server = new NeonServer({
  apiKey: "your-neon-api-key",
  projectId: "your-project-id",
});

// Execute SQL query
const results = await server.query({
  sql: `
    SELECT 
      users.name,
      COUNT(orders.id) as order_count
    FROM users
    LEFT JOIN orders ON users.id = orders.user_id
    GROUP BY users.id, users.name
    HAVING COUNT(orders.id) > 5
  `,
});

// Create database branch
const branch = await server.createBranch({
  name: "feature-test",
  parentBranch: "main",
  options: {
    computeProvisioning: "auto",
    autoscaling: true,
  },
});

// Monitor performance
const metrics = await server.getMetrics({
  timeRange: {
    from: "now-1h",
    to: "now",
  },
  metrics: [
    "cpu_usage",
    "memory_usage",
    "active_connections",
    "query_duration",
  ],
});
```

## Dependencies

- Node.js >= 14.x
- Neon account
- Neon API key
- Project on Neon platform

## Related Servers

- None currently listed
