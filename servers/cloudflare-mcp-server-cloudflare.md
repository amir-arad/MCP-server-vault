---
type: server
repo_url: https://github.com/cloudflare/mcp-server-cloudflare
name: Cloudflare MCP Server
owner: cloudflare
stars: 277
last_updated: 2025-02-21
status: active
official: true
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "status/official",
    "category/cloud",
    "integration/cloudflare",
    "purpose/infrastructure",
    "category/ai",
  ]
---

# Cloudflare MCP Server

#status/active #status/official #category/cloud #integration/cloudflare #purpose/infrastructure #category/ai

## Description

Lets you use Claude Desktop, or any MCP Client, to use natural language to accomplish things on your Cloudflare account. This official MCP server enables natural language control of Cloudflare services and configurations.

## Features

- Natural language control
- DNS management
- SSL/TLS configuration
- Security settings
- Cache control
- Worker deployment
- Analytics access
- Rule management
- Domain control
- Performance optimization

## Installation

```bash
npm install @cloudflare/mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "cloudflare": {
      "command": "npx",
      "args": ["@cloudflare/mcp-server"],
      "env": {
        "CF_API_TOKEN": "your-api-token",
        "CF_ACCOUNT_ID": "your-account-id",
        "ZONE_ID": "optional-zone-id",
        "AI_MODEL": "gpt-4",
        "LOG_LEVEL": "info"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Cloudflare API token
- AI model access
- Natural language processor
- API client
- Command parser

## Related Servers

- dynamicendpoints-cloudflare-github-backup-mcp
- cloudflare-mcp-server-cloudflare
- modelcontextprotocol-cloud-server
