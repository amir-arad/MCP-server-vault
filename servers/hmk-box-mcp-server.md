---
type: server
repo_url: https://github.com/hmk/box-mcp-server
name: Box MCP Server
owner: hmk
stars: 2
last_updated: 2025-02-11
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/storage",
    "integration/box",
    "purpose/document-management",
  ]
---

# Box MCP Server

#status/active #category/storage #integration/box #purpose/document-management

## Description

The Box MCP Server facilitates searching and reading PDF and Word files in Box using Developer Token authentication.

## Features

- PDF file access
- Word file access
- Document search
- Content reading
- Token authentication
- File management
- Content indexing
- Access control

## Installation

```bash
npm install @hmk/box-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "box": {
      "command": "npx",
      "args": ["@hmk/box-mcp"],
      "env": {
        "BOX_DEVELOPER_TOKEN": "your-developer-token",
        "DEFAULT_FOLDER_ID": "0",
        "SEARCH_LIMIT": "100",
        "SUPPORTED_TYPES": "pdf,docx"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Box account
- Developer token
- PDF/Word readers

## Related Servers

- None currently listed
