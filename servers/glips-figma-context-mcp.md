---
type: server
repo_url: https://github.com/GLips/Figma-Context-MCP
name: Figma Context MCP Server
owner: GLips
stars: 392
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
    "integration/cursor",
    "purpose/design-data",
    "purpose/code-generation",
    "tech/javascript",
  ]
---

# Figma Context MCP Server

#status/active #category/design #integration/figma #integration/cursor #purpose/design-data #purpose/code-generation

## Description

Enables Cursor to access Figma files through the Model Context Protocol, enhancing its ability to accurately interpret and utilize design data for code generation.

## Features

- Figma file access
- Design data interpretation
- Code generation support
- Design system integration
- Component analysis
- Style extraction
- Layout parsing
- Asset management
- Version tracking
- Context preservation

## Installation

```bash
npm install @glips/figma-context-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "figma-context": {
      "command": "npx",
      "args": ["@glips/figma-context-mcp"],
      "env": {
        "FIGMA_ACCESS_TOKEN": "your-access-token",
        "CURSOR_API_KEY": "your-cursor-key",
        "CACHE_TTL": "3600",
        "MAX_DEPTH": "5"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Figma API access
- Cursor integration
- Design parser
- Cache system

## Related Servers

- [Figma Server](https://github.com/TimHolden/figma-mcp-server) - Alternative Figma implementation
- [Figma MCP](https://github.com/MatthewDailey/figma-mcp) - Figma REST API integration
