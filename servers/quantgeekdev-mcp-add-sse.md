---
type: server
repo_url: https://github.com/QuantGeekDev/mcp-add-sse
name: Add SSE MCP Server
owner: QuantGeekDev
stars: 3
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/active",
    "category/development",
    "category/data-processing",
    "tech/typescript",
    "purpose/development",
  ]
---

# Add SSE MCP Server

#status/active #category/development #category/data-processing #tech/typescript #purpose/development

## Description

A Model Context Protocol server built with mcp-framework that allows users to create and manage custom tools for processing data, integrating with the Claude Desktop via CLI.

## Features

- Custom tool creation and management
- Data processing capabilities
- Claude Desktop integration
- CLI interface
- Server-Sent Events support
- Extensible framework

## Installation

```bash
npm install @quantgeekdev/mcp-add-sse
```

## Usage

```javascript
{
  "mcpServers": {
    "add-sse": {
      "command": "npx",
      "args": ["@quantgeekdev/mcp-add-sse"],
      "env": {
        "PORT": "3000",
        "MAX_CONNECTIONS": "100",
        "EVENT_TIMEOUT": "30000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript
- mcp-framework
- Claude Desktop

## Related Servers

- None currently listed
