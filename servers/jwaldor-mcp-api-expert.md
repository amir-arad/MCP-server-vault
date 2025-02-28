---
type: server
repo_url: https://github.com/jwaldor/mcp-api-expert
name: API Expert MCP Server
owner: jwaldor
stars: 5
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/api", "purpose/integration", "tech/rest"]
---

# API Expert MCP Server

#status/active #category/api #purpose/integration #tech/rest

## Description

Integrates any REST API by dynamically connecting to APIs using provided documentation and keys, enabling rapid prototyping of applications with real-time external data. All you have to do is provide API documentation and API keys in a message.

## Features

- Dynamic API integration
- Documentation parsing
- Key management
- Rapid prototyping
- Real-time data access
- Request validation
- Response formatting
- Error handling

## Setup with Claude Desktop

1.  Install the package globally:

```bash
npm i -g mcp-api-connect
```

2.  Run the setup command:

```bash
mcpapiconnect install
```

3.  Restart Claude

## Usage

```javascript
{
  "mcpServers": {
    "api-expert": {
      "command": "npx",
      "args": ["@jwaldor/mcp-api-expert"],
      "env": {
        "API_DOCS_URL": "https://api.example.com/docs",
        "API_KEY": "your-api-key",
        "CACHE_DURATION": "3600",
        "VALIDATION_LEVEL": "strict"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- API documentation
- Authentication credentials
- OpenAPI/Swagger support

## Related Servers

- None currently listed
