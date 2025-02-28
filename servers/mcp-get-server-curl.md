---
type: server
repo_url: https://github.com/mcp-get/community-servers/tree/HEAD/src/server-curl
name: Curl MCP Server
owner: mcp-get
stars: 18
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/networking",
    "tech/http",
    "purpose/requests",
    "tech/curl",
    "purpose/web-access",
  ]
---

# Curl MCP Server

#status/active #category/networking #tech/http #purpose/requests #tech/curl #purpose/web-access

## Description

Make HTTP requests to any URL using curl-like interface. This server provides a familiar curl-like experience for making HTTP requests through the Model Context Protocol.

## Features

- HTTP requests
- URL handling
- Method selection
- Header management
- Request body
- Response parsing
- Cookie handling
- SSL/TLS support
- Proxy support
- Redirect handling

## Installation

```bash
npm install @mcp-get/server-curl
```

## Usage

```javascript
{
  "mcpServers": {
    "curl": {
      "command": "npx",
      "args": ["@mcp-get/server-curl"],
      "env": {
        "DEFAULT_TIMEOUT": "30000",
        "MAX_REDIRECTS": "5",
        "FOLLOW_REDIRECTS": "true",
        "VERIFY_SSL": "true",
        "USER_AGENT": "mcp-curl/1.0"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- HTTP client
- SSL/TLS support
- Cookie manager
- Request formatter
- Response parser

## Related Servers

- modelcontextprotocol-http-server
- modelcontextprotocol-network-server
- fetch-mcp-server
