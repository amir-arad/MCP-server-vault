---
type: server
repo_url: https://github.com/ClickHouse/mcp-clickhouse
name: ClickHouse MCP Server
owner: ClickHouse
stars: 60
last_updated: 2025-03-01
status: active
official: true
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "status/official",
    "category/database",
    "integration/clickhouse",
    "purpose/analytics",
    "tech/sql",
  ]
---

# ClickHouse MCP Server

#status/active #status/official #category/database #integration/clickhouse #purpose/analytics #tech/sql

## Description

ClickHouse database integration with schema inspection and query capabilities. This official MCP server provides comprehensive access to ClickHouse's columnar database features for analytics and data processing.

## Features

- Schema inspection
- Query execution
- Performance monitoring
- Table management
- Column operations
- Data ingestion
- Query optimization
- Result streaming
- Metadata handling
- Security controls

## Installation

```bash
npm install @clickhouse/mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "clickhouse": {
      "command": "npx",
      "args": ["@clickhouse/mcp-server"],
      "env": {
        "CLICKHOUSE_HOST": "localhost",
        "CLICKHOUSE_PORT": "8123",
        "CLICKHOUSE_USER": "default",
        "CLICKHOUSE_PASSWORD": "your-password",
        "MAX_ROWS": "1000000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- ClickHouse database
- SQL parser
- Query executor
- Connection pool
- Result formatter

## Related Servers

- modelcontextprotocol-postgres-server
- modelcontextprotocol-sqlite-server
- tinybirdco-mcp-tinybird
