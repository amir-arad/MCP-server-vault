---
type: server
repo_url: https://github.com/motherduckdb/mcp-server-motherduck
name: MotherDuck
owner: motherduckdb
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/database"]
---

#status/active #status/official #category/database

# MotherDuck

## Description

Query and analyze data with MotherDuck and local DuckDB. This MCP server provides seamless integration with MotherDuck's cloud service and local DuckDB instances, enabling powerful data analysis capabilities.

## Features

- SQL query execution
- Local DuckDB integration
- Cloud data synchronization
- Advanced analytics functions
- Data import/export capabilities
- Query optimization
- Real-time data analysis
- Distributed query processing
- Data caching
- Performance monitoring

## Installation

```bash
npm install @motherduck/mcp-server
```

## Usage

```javascript
import { MotherDuckServer } from "@motherduck/mcp-server";

const server = new MotherDuckServer({
  apiKey: "your-motherduck-api-key",
  databaseUrl: "md:your-database",
});

// Execute a SQL query
const results = await server.query({
  sql: `
    SELECT 
      category,
      COUNT(*) as count,
      AVG(price) as avg_price
    FROM products
    GROUP BY category
    ORDER BY count DESC
  `,
});

// Import data from a file
await server.importData({
  table: "sales",
  source: "./sales_data.csv",
  format: "csv",
  options: {
    delimiter: ",",
    header: true,
  },
});

// Create a materialized view
await server.createMaterializedView({
  name: "daily_sales",
  query: `
    SELECT 
      DATE_TRUNC('day', timestamp) as date,
      SUM(amount) as total_sales
    FROM sales
    GROUP BY 1
  `,
  refreshSchedule: "0 0 * * *", // Daily refresh at midnight
});
```

## Dependencies

- Node.js >= 14.x
- MotherDuck account
- MotherDuck API key
- Local DuckDB installation (optional)

## Related Servers

- None currently listed
