---
type: server
repo_url: https://github.com/kirill-markin/example-mcp-server
name: Example MCP Server
owner: kirill-markin
stars: 13
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/web",
    "purpose/website-fetching",
    "tech/stdio",
    "tech/sse",
    "integration/cursor",
    "tech/python",
    "purpose/template",
  ]
---

# Example MCP Server

#status/active #category/web #purpose/website-fetching #tech/stdio #tech/sse #integration/cursor #tech/python #purpose/template

## Description

A simple MCP server template that facilitates website fetching through a configurable server platform using stdio or SSE transport, allowing integration with tools like Cursor for streamlined access. It provides a ready-to-use template for extending Cursor IDE with custom tools.

## Features

- Website fetching
- Configurable platform
- Multiple transport options (stdio, sse)
- Stdio support
- SSE integration
- Cursor tool integration
- Error handling
- Request validation
- Response formatting
- Configuration management
- Heroku deployment
- Docker support
- Smithery installation

## Installation

```bash
npm install @kirill-markin/example-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "example": {
      "command": "npx",
      "args": ["@kirill-markin/example-mcp-server"],
      "env": {
        "TRANSPORT": "stdio",
        "TIMEOUT": "5000",
        "MAX_RETRIES": "3",
        "LOG_LEVEL": "info"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 18
- Python 3.7+
- Network connectivity
- Cursor (optional)
- Transport libraries
- Configuration system
- MCP Inspector

## Related Servers

- None currently listed
