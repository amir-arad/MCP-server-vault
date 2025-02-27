---
type: server
repo_url: https://github.com/domdomegg/airtable-mcp-server
name: Airtable Server
owner: domdomegg
stars: 35
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/database", "integration/airtable", "purpose/data-management"]
---

# Airtable Server

#status/active #category/database #integration/airtable #purpose/data-management

## Description

A Model Context Protocol server that provides read and write access to Airtable databases. This server enables LLMs to inspect database schemas, then read and write records.

## Features

- Database schema inspection
- Record reading and writing
- Schema management
- Query execution
- Batch operations
- Field type handling
- View filtering
- Relationship management

## Installation

```bash
npm install @domdomegg/airtable-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "airtable": {
      "command": "npx",
      "args": ["@domdomegg/airtable-mcp-server"],
      "env": {
        "AIRTABLE_API_KEY": "your-api-key",
        "DEFAULT_BASE": "your-base-id",
        "CACHE_TTL": "300",
        "MAX_BATCH_SIZE": "10"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Airtable account
- API access token
- Base permissions

## Related Servers

- felores/airtable-mcp