---
type: server
repo_url: https://github.com/tinybirdco/mcp-tinybird
name: Tinybird
owner: tinybirdco
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags:
  [
    "status/active",
    "status/official",
    "category/database",
    "category/analytics",
  ]
---

# Tinybird

#status/active #status/official #category/database #category/analytics

## Description

Interact with Tinybird serverless ClickHouse platform. This MCP server provides seamless integration with Tinybird's real-time analytics platform powered by ClickHouse.

## Features

- Real-time data ingestion
- SQL query execution
- Data pipe management
- API endpoint creation
- Real-time analytics
- Data transformation
- Query optimization
- Schema management
- Access control
- Performance monitoring

## Installation

```bash
npm install @tinybird/mcp-server
```

## Usage

```javascript
import { TinybirdServer } from "@tinybird/mcp-server";

const server = new TinybirdServer({
  apiKey: "your-tinybird-api-key",
  region: "eu",
});

// Ingest data in real-time
await server.ingest({
  datasource: "events",
  data: [
    {
      timestamp: new Date().toISOString(),
      event_type: "page_view",
      user_id: "123",
      page: "/home",
    },
  ],
  format: "json",
});

// Execute SQL query
const results = await server.query({
  sql: `
    SELECT 
      toStartOfHour(timestamp) as hour,
      event_type,
      count() as events
    FROM events
    WHERE timestamp >= now() - interval 24 hour
    GROUP BY hour, event_type
    ORDER BY hour DESC
  `,
});

// Create data pipe
await server.createPipe({
  name: "hourly_stats",
  description: "Aggregate hourly statistics",
  sql: `
    SELECT
      toStartOfHour(timestamp) as hour,
      countState() as events,
      uniqState(user_id) as users
    FROM events
    GROUP BY hour
  `,
  materialized: true,
  schedule: "0 * * * *", // Every hour
});

// Create API endpoint
await server.createEndpoint({
  name: "get_stats",
  sql: `
    SELECT *
    FROM hourly_stats
    WHERE hour >= {start_date:DateTime}
    AND hour <= {end_date:DateTime}
  `,
  parameters: [
    {
      name: "start_date",
      type: "DateTime",
      required: true,
    },
    {
      name: "end_date",
      type: "DateTime",
      required: true,
    },
  ],
});
```

## Dependencies

- Node.js >= 14.x
- Tinybird account
- Tinybird API key
- Active workspace

## Related Servers

- None currently listed
