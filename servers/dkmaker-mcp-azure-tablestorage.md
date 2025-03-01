--- 
type: server
repo_url: https://github.com/dkmaker/mcp-azure-tablestorage
name: Azure Table Storage MCP Server
owner: dkmaker
stars: 4
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "category/storage",
    "integration/azure",
    "integration/table-storage",
    "purpose/data-management",
    "tech/javascript",
    "tech/typescript",
  ]
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

- Node.js >= 16
- Azure subscription
- Storage account
- Table access rights