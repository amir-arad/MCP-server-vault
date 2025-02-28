---
type: server
repo_url: https://github.com/ZubeidHendricks/azure-onenote-mcp-server
name: Azure OneNote MCP Server
owner: ZubeidHendricks
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/productivity", "integration/azure", "integration/onenote", "purpose/note-management", "tech/typescript", "integration/microsoft-graph"]
---

# Azure OneNote MCP Server

#status/active #category/productivity #integration/azure #integration/onenote #purpose/note-management #tech/typescript #integration/microsoft-graph

## Description

A Model Context Protocol (MCP) server implementation for Microsoft OneNote, enabling AI language models to interact with OneNote through a standardized interface. This server provides comprehensive notebook, section, and page management capabilities via the Microsoft Graph API.

## Features

- Notebook Management:
  - List all notebooks
  - Create new notebooks
  - Get notebook details
  - Delete notebooks
- Section Management:
  - List sections in a notebook
  - Create new sections
  - Get section details
  - Delete sections
- Page Management:
  - List pages in a section
  - Create new pages with HTML content
  - Read page content
  - Update page content
  - Delete pages
  - Search pages across notebooks

## Installation

```bash
# Install via Smithery (recommended)
npx -y @smithery/cli install @modelcontextprotocol/server-onenote --client claude

# Or manual installation
npm install -g mcp-server-onenote
```

## Usage

```javascript
{
  "mcpServers": {
    "onenote": {
      "command": "npx",
      "args": ["-y", "mcp-server-onenote"],
      "env": {
        "AZURE_TENANT_ID": "<YOUR_TENANT_ID>",
        "AZURE_CLIENT_ID": "<YOUR_CLIENT_ID>",
        "AZURE_CLIENT_SECRET": "<YOUR_CLIENT_SECRET>"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Azure account with app registration
- Microsoft Graph API permissions:
  - Notes.ReadWrite.All
  - Notes.Read.All
- OneNote access

## Related Servers

- stefanskiasan/azure-devops-mcp-server - Azure DevOps integration
- mashriram/azure_mcp_server - General Azure services integration
- dkmaker/mcp-azure-tablestorage - Azure Table Storage integration
- sirmews/apple-notes-mcp - Alternative notes integration for Apple Notes