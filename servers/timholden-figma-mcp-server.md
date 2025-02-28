---
type: server
repo_url: https://github.com/TimHolden/figma-mcp-server
name: Figma MCP Server
owner: TimHolden
stars: 35
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_012.md"]
tags:
  [
    "status/active",
    "category/design",
    "integration/figma",
    "purpose/file-management",
    "purpose/component-management",
    "purpose/variable-management",
  ]
---

# Figma MCP Server

#status/active #category/design #integration/figma #purpose/file-management #purpose/component-management #purpose/variable-management

## Description

Enables seamless interaction with Figma via the Model Context Protocol, allowing LLM applications to access, manipulate, and track Figma files, components, and variables.

## Features

- Figma file access
- Component management
- Variable tracking
- File manipulation
- Version control
- Asset management
- Team collaboration
- Design system integration
- Change tracking
- Permission handling

## Installation

```bash
npm install @timholden/figma-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "figma": {
      "command": "npx",
      "args": ["@timholden/figma-mcp-server"],
      "env": {
        "FIGMA_ACCESS_TOKEN": "your-access-token",
        "PROJECT_ID": "your-project-id",
        "AUTO_SYNC": "true",
        "SYNC_INTERVAL": "300"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Figma API access
- File system access
- Cache system
- Sync manager

## Related Servers

- [Figma Context MCP](https://github.com/GLips/Figma-Context-MCP) - Cursor integration for Figma
- [Figma MCP](https://github.com/MatthewDailey/figma-mcp) - Figma REST API integration
