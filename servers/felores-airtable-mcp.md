---
type: server
repo_url: https://github.com/felores/airtable-mcp
name: Airtable MCP Server
owner: felores
stars: 13
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/active",
    "category/database",
    "integration/airtable",
    "purpose/data-management",
    "tech/javascript",
    "tech/typescript",
  ]
---

# Airtable MCP Server

#status/active #category/database #integration/airtable #purpose/data-management

## Description

Airtable MCP server enables AI assistants to programmatically manage Airtable bases, tables, fields, and records through a simplified interface to the Airtable API.

## Features

- Airtable base management
- Table operations
- Field configuration
- Record CRUD operations
- Query capabilities
- Batch processing
- Schema management
- View customization

## Installation

```bash
npm install @felores/airtable-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "airtable": {
      "command": "npx",
      "args": ["@felores/airtable-mcp"],
      "env": {
        "AIRTABLE_API_KEY": "your-api-key",
        "BASE_ID": "your-base-id",
        "MAX_RECORDS_PER_REQUEST": "100",
        "RATE_LIMIT_PER_SEC": "5"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Airtable account
- Airtable API key
- Base access permissions

## Related Servers

- domdomegg/airtable-mcp-server
