---
type: server
repo_url: https://github.com/hmk/attio-mcp-server
name: Attio MCP Server
owner: hmk
stars: 2
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/crm", "integration/attio", "purpose/data-management"]
---

# Attio MCP Server

#status/active #category/crm #integration/attio #purpose/data-management

## Description

Facilitates interaction with the Attio CRM by allowing MCP clients to read and write company records and notes through the Attio API.

## Features

- Company record management
- Note creation and editing
- CRM data access
- Record searching
- Data synchronization
- Contact management
- Field customization
- API integration

## Installation

```bash
npm install @hmk/attio-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "attio": {
      "command": "npx",
      "args": ["@hmk/attio-mcp"],
      "env": {
        "ATTIO_API_KEY": "your-api-key",
        "WORKSPACE_ID": "your-workspace-id",
        "CACHE_TTL": "3600",
        "BATCH_SIZE": "50"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Attio account
- API credentials
- Workspace access

## Related Servers

- None currently listed