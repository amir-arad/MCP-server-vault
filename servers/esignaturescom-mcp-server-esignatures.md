---
type: server
repo_url: https://github.com/esignaturescom/mcp-server-esignatures
name: eSignatures MCP Server
owner: esignaturescom
stars: 2
last_updated: 2025-02-12
status: active
official: true
verified: false
sources: ["inbox/batch_011.md"]
tags: ["status/active", "status/official", "category/document-management", "purpose/esignature", "purpose/contract-management", "purpose/template-management"]
---

# eSignatures MCP Server

#status/active #status/official #category/document-management #purpose/esignature #purpose/contract-management #purpose/template-management

## Description

Facilitates contract and template management for eSignatures, enabling users to create, send, update, and manage contracts and templates with customizable options through a user-friendly interface.

## Features

- Contract management
- Template management
- Electronic signatures
- Document customization
- Workflow automation
- Status tracking
- Audit trails
- User management
- Template versioning
- Security compliance

## Installation

```bash
npm install @esignatures/mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "esignatures": {
      "command": "npx",
      "args": ["@esignatures/mcp-server"],
      "env": {
        "ESIGNATURES_API_KEY": "your-api-key",
        "WEBHOOK_URL": "your-webhook-url",
        "TEMPLATE_DIR": "./templates",
        "STORAGE_PATH": "./storage"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- eSignatures API access
- Storage system
- PDF processing libraries
- Network connectivity

## Related Servers

- None currently listed