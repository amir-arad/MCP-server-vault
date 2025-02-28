---
type: server
repo_url: https://github.com/olegshilin/mcp-eagle
name: Eagle MCP Server
owner: olegshilin
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/asset-management",
    "integration/eagle",
    "integration/claude",
    "purpose/creative-projects",
    "purpose/asset-organization",
  ]
---

# Eagle MCP Server

#status/active #category/asset-management #integration/eagle #integration/claude #purpose/creative-projects #purpose/asset-organization

## Description

Integrates Claude Desktop with the Eagle.cool app for asset management and creative project assistance through MCP-enabled interaction with Eagle's features.

## Features

- Asset management integration
- Creative project support
- Claude Desktop integration
- Asset organization
- Metadata management
- Asset search
- Collection management
- Tag organization
- Asset preview
- Export capabilities

## Installation

```bash
npm install @olegshilin/mcp-eagle
```

## Usage

```javascript
{
  "mcpServers": {
    "eagle": {
      "command": "npx",
      "args": ["@olegshilin/mcp-eagle"],
      "env": {
        "EAGLE_APP_PATH": "/Applications/Eagle.app",
        "EAGLE_LIBRARY_PATH": "~/Documents/Eagle",
        "CLAUDE_API_KEY": "your-claude-api-key"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Eagle.cool application
- Claude Desktop
- Claude API access
- File system access

## Related Servers

- None currently listed
