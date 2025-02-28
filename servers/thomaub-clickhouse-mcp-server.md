---
type: server
repo_url: https://github.com/ThomAub/clickhouse_mcp_server
name: ClickHouse Integration MCP Server
owner: ThomAub
stars: 1
last_updated: 2024-12-18
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/database",
    "integration/clickhouse",
    "purpose/data-analysis",
    "purpose/analytics",
    "tech/sql",
  ]
---

# ClickHouse Integration MCP Server

#status/active #category/database #integration/clickhouse #purpose/data-analysis #purpose/analytics #tech/sql

## Description

Integrates with ClickHouse databases to enable data analysis, querying, and exploration for large-scale analytical workloads.

## Features

- Database connectivity
- Query execution
- Data analysis
- Schema exploration
- Performance monitoring
- Query optimization
- Result formatting
- Batch processing
- Error handling
- Analytics support

## Installation

```bash
npm install @thomaub/clickhouse-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "clickhouse": {
      "command": "npx",
      "args": ["@thomaub/clickhouse-mcp"],
      "env": {
        "CLICKHOUSE_HOST": "localhost",
        "CLICKHOUSE_PORT": "8123",
        "CLICKHOUSE_USER": "default",
        "CLICKHOUSE_PASSWORD": "your-password",
        "MAX_QUERY_SIZE": "1000000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- ClickHouse database
- SQL parser
- Query executor
- Result formatter
- Connection manager

## Related Servers

- clickhouse/mcp-clickhouse
- iskakaushik-mcp-clickhouse
- tinybirdco-mcp-tinybird
