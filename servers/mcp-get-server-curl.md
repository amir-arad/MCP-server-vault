---
type: server
repo_url: https://github.com/mcp-get/community-servers/tree/HEAD/src/server-curl
name: Curl MCP Server
owner: mcp-get
stars: 20
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/networking",
    "tech/http",
    "purpose/requests",
    "tech/curl",
    "purpose/web-access",
    "tech/typescript",
    "tech/nodejs",
    "purpose/api",
    "category/tools"
  ]
---

# Curl MCP Server

#status/active #category/networking #tech/http #purpose/requests #tech/curl #purpose/web-access #tech/typescript #tech/nodejs #purpose/api #category/tools

## Description

A TypeScript/Node.js-based MCP server that provides a curl-like interface for making HTTP requests. The server enables AI models to interact with web APIs and services through a familiar curl-like experience, supporting all common HTTP methods with customizable headers, request bodies, and timeout configurations.

## Features

- HTTP request capabilities
- Multiple HTTP methods (GET, POST, PUT, DELETE, etc.)
- Custom header support
- Request body handling
- Configurable timeouts
- Response parsing
- Status code handling
- Cookie management
- SSL/TLS support
- Proxy compatibility
- Redirect handling
- Error management
- Comprehensive response data

## Installation

```bash
# Using mcp-get
npx @michaellatman/mcp-get@latest install @mcp-get-community/server-curl

# Or build from source
git clone https://github.com/mcp-get/community-servers.git
cd community-servers/src/server-curl
npm install
npm run build
```

## Usage

```javascript
// Configuration
{
  "mcpServers": {
    "@mcp-get-community/server-curl": {
      "runtime": "node",
      "command": "npx",
      "args": ["-y", "@mcp-get-community/server-curl"],
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

// Example Request
{
  "url": "https://api.example.com/data",
  "method": "POST",
  "headers": {
    "Content-Type": "application/json",
    "Authorization": "Bearer token123"
  },
  "body": "{\"key\": \"value\"}",
  "timeout": 5000
}
```

## Dependencies

- Node.js >= 16
- TypeScript runtime
- HTTP client library
- SSL/TLS support
- Cookie manager
- Request formatter
- Response parser
- Error handler
- Proxy manager
- Timeout controller

## Related Servers

- modelcontextprotocol-http-server
- modelcontextprotocol-network-server
- fetch-mcp-server
- zcaceres/fetch-mcp