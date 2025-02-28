---
type: server
repo_url: https://github.com/ZeparHyfar/mcp-datetime
name: DateTime Formatting MCP Server
owner: ZeparHyfar
stars: 2
last_updated: 2025-02-13
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/utility",
    "purpose/datetime",
    "purpose/formatting",
    "integration/claude",
    "tech/time",
  ]
---

# DateTime Formatting MCP Server

#status/active #category/utility #purpose/datetime #purpose/formatting #integration/claude #tech/time

## Description

A datetime formatting service implemented as an MCP server for the Claude Desktop Application. Supports generation of datetime strings in various formats.

## Features

- DateTime formatting
- Format customization
- Timezone support
- Locale handling
- Format validation
- String generation
- Pattern matching
- Error handling
- Format conversion
- Timezone conversion

## Installation

```bash
npm install @zeparhyfar/mcp-datetime
```

## Usage

```javascript
{
  "mcpServers": {
    "datetime": {
      "command": "npx",
      "args": ["@zeparhyfar/mcp-datetime"],
      "env": {
        "DEFAULT_FORMAT": "YYYY-MM-DD HH:mm:ss",
        "DEFAULT_TIMEZONE": "UTC",
        "DEFAULT_LOCALE": "en-US",
        "CACHE_ENABLED": "true",
        "STRICT_PARSING": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- DateTime library
- Timezone database
- Locale data
- Format parser
- Validation engine

## Related Servers

- bossjones/datetime-mcp-server
- modelcontextprotocol-time-server
- modelcontextprotocol-utility-server
