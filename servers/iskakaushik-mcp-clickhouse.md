---
type: server
repo_url: https://github.com/iskakaushik/mcp-clickhouse
name: ClickHouse Community MCP Server
owner: iskakaushik
stars: 3
last_updated: 2025-01-06
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "status/community",
    "category/database",
    "integration/clickhouse",
    "purpose/analytics",
    "tech/sql",
  ]
---

# ClickHouse Community MCP Server

#status/active #status/community #category/database #integration/clickhouse #purpose/analytics #tech/sql

## Description

An MCP server for ClickHouse. This community implementation provides integration with ClickHouse database systems, offering core functionality for database operations and analytics.

## Features

- Database connectivity
- Query execution
- Schema management
- Data insertion
- Result formatting
- Error handling
- Connection pooling
- Basic monitoring
- Type conversion
- Query validation

## Installation

```bash
npm install @iskakaushik/mcp-clickhouse
```

## Usage

```javascript
{
  "mcpServers": {
    "clickhouse": {
      "command": "npx",
      "args": ["@iskakaushik/mcp-clickhouse"],
      "env": {
        "CLICKHOUSE_URL": "http://localhost:8123",
        "CLICKHOUSE_DB": "default",
        "CLICKHOUSE_USER": "default",
        "CLICKHOUSE_PASSWORD": "your-password",
        "MAX_ROWS": "10000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- ClickHouse database
- HTTP client
- Query builder
- Result parser
- Connection manager

## Related Servers

- clickhouse/mcp-clickhouse
- modelcontextprotocol-postgres-server
- tinybirdco-mcp-tinybird
