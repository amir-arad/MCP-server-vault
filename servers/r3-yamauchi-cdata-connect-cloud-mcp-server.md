---
type: server
repo_url: https://github.com/r3-yamauchi/cdata-connect-cloud-mcp-server
name: CData Connect Cloud MCP Server
owner: r3-yamauchi
stars: 0
last_updated: 2025-02-18
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/database",
    "integration/cdata",
    "purpose/data-integration",
    "tech/sql",
    "purpose/analytics",
  ]
---

# CData Connect Cloud MCP Server

#status/active #category/database #integration/cdata #purpose/data-integration #tech/sql #purpose/analytics

## Description

Integrates with CData Connect Cloud to enable SQL query execution across diverse data sources, facilitating seamless data integration for analytics and workflows.

## Features

- SQL query execution
- Multi-source data integration
- Real-time data access
- Cross-database joins
- Query optimization
- Connection pooling
- Data type mapping
- Security management
- Query monitoring
- Performance analytics

## Installation

```bash
npm install @r3-yamauchi/cdata-connect-cloud-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "cdata-connect": {
      "command": "npx",
      "args": ["@r3-yamauchi/cdata-connect-cloud-mcp"],
      "env": {
        "CDATA_CLOUD_URL": "your-cdata-cloud-url",
        "CDATA_API_KEY": "your-api-key",
        "CDATA_SECRET": "your-api-secret",
        "MAX_CONNECTIONS": "10"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- CData Connect Cloud account
- API credentials
- SQL client library
- Connection manager

## Related Servers

- modelcontextprotocol-postgres-server
- modelcontextprotocol-sqlite-server
- monochromegane-mcp-bigquery-server
