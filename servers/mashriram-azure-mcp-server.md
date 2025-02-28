---
type: server
repo_url: https://github.com/mashriram/azure_mcp_server
name: Azure MCP Server
owner: mashriram
stars: 0
last_updated: 2025-02-13
status: active
official: false
verified: false
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/cloud", "integration/azure", "integration/blob-storage", "integration/cosmos-db"]
---

# Azure MCP Server

#status/active #category/cloud #integration/azure #integration/blob-storage #integration/cosmos-db

## Description

This server implements the Model Context Protocol for seamless interaction with Azure Blob Storage and Cosmos DB, enabling automatic logging and audit tracking of operations.

## Features

- Blob Storage integration
- Cosmos DB operations
- Automatic logging
- Audit tracking
- Operation monitoring
- Data management
- Access control
- Performance optimization

## Installation

```bash
npm install @mashriram/azure-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "azure": {
      "command": "npx",
      "args": ["@mashriram/azure-mcp"],
      "env": {
        "AZURE_STORAGE_CONNECTION_STRING": "your-connection-string",
        "COSMOS_DB_ENDPOINT": "your-cosmos-endpoint",
        "COSMOS_DB_KEY": "your-cosmos-key",
        "LOG_LEVEL": "info"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Azure subscription
- Storage account
- Cosmos DB instance

## Related Servers

- stefanskiasan/azure-devops-mcp-server
- ZubeidHendricks/azure-onenote-mcp-server
- dkmaker/mcp-azure-tablestorage