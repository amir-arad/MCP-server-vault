---
type: server
repo_url: https://github.com/runekaagaard/mcp-alchemy
name: Alchemy MCP Server
owner: runekaagaard
stars: 28
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/database", "tech/sqlalchemy", "purpose/data-access", "integration/claude"]
---

# Alchemy MCP Server

#status/active #category/database #tech/sqlalchemy #purpose/data-access #integration/claude

## Description

Integrates Claude Desktop with SQL databases using SQLAlchemy to enable direct querying, analysis, and exploration of data across many database engines.

## Features

- SQLAlchemy integration
- Multi-database support
- Direct SQL querying
- Data analysis capabilities
- Schema exploration
- Query optimization
- Claude Desktop integration
- Connection management

## Installation

```bash
npm install @runekaagaard/mcp-alchemy
```

## Usage

```javascript
{
  "mcpServers": {
    "alchemy": {
      "command": "npx",
      "args": ["@runekaagaard/mcp-alchemy"],
      "env": {
        "DATABASE_URL": "your-database-url",
        "QUERY_TIMEOUT": "30",
        "MAX_ROWS": "1000",
        "ENABLE_CACHE": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Python >= 3.8
- SQLAlchemy
- Database drivers
- Claude Desktop

## Related Servers

- None currently listed