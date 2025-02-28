---
type: server
repo_url: https://github.com/dkmaker/mcp-azure-tablestorage
name: Azure Table Storage MCP Server
owner: dkmaker
stars: 4
last_updated: 2025-01-13
status: active
official: false
verified: false
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/storage", "integration/azure", "integration/table-storage", "purpose/data-management"]
---

# Azure Table Storage MCP Server

#status/active #category/storage #integration/azure #integration/table-storage #purpose/data-management

## Description

Enables interaction with Azure Table Storage directly through Cline. This tool allows you to query and manage data in Azure Storage Tables.

## Features

- Table Storage access
- Data querying
- Record management
- Table operations
- Entity manipulation
- Batch processing
- Query optimization
- Schema handling

## Installation

```bash
npm install @dkmaker/mcp-azure-tablestorage
```

## Usage

```javascript
{
  "mcpServers": {
    "azure-table": {
      "command": "npx",
      "args": ["@dkmaker/mcp-azure-tablestorage"],
      "env": {
        "AZURE_STORAGE_CONNECTION_STRING": "your-connection-string",
        "DEFAULT_TABLE": "your-table-name",
        "BATCH_SIZE": "100",
        "QUERY_TIMEOUT": "30"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Azure subscription
- Storage account
- Table access rights

## Related Servers

- stefanskiasan/azure-devops-mcp-server
- mashriram/azure_mcp_server
- ZubeidHendricks/azure-onenote-mcp-server