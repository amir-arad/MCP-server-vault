---
type: server
repo_url: https://github.com/seansoreilly/abs
name: Australian Bureau of Statistics MCP Server
owner: seansoreilly
stars: 3
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/active",
    "category/data-analysis",
    "integration/abs",
    "purpose/statistics",
    "tech/nodejs",
  ]
---

# Australian Bureau of Statistics MCP Server

#status/active #category/data-analysis #integration/abs #purpose/statistics

## Description

An MCP server that provides access to the Australian Bureau of Statistics (ABS) Data API, enabling AI assistants to query and analyze ABS statistical data.

## Features

- Direct access to ABS Data API
- Statistical data querying
- Data analysis capabilities
- Structured data responses
- Historical data access

## Installation

```bash
npm install @seansoreilly/abs-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "abs": {
      "command": "npx",
      "args": ["@seansoreilly/abs-mcp"],
      "env": {
        "ABS_API_KEY": "your-abs-api-key"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- ABS Data API access key

## Related Servers

- None currently listed
