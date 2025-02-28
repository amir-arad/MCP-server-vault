---
type: server
repo_url: https://github.com/ComposioHQ/composio-mcp-server
name: Composio MCP Server
owner: ComposioHQ
stars: 6
last_updated: 2025-02-21
status: active
official: true
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "status/official",
    "category/integration",
    "integration/gmail",
    "integration/linear",
    "purpose/application-access",
  ]
---

# Composio MCP Server

#status/active #status/official #category/integration #integration/gmail #integration/linear #purpose/application-access

## Description

A server implementation that provides MCP-compatible access to Composio applications like Gmail and Linear, allowing interaction through a structured interface for language models.

## Features

- Gmail integration
- Linear integration
- Structured interfaces
- Application access
- Authentication handling
- Data synchronization
- Action automation
- Event handling
- Status tracking
- Error management

## Installation

```bash
npm install @composiohq/composio-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "composio": {
      "command": "npx",
      "args": ["@composiohq/composio-mcp"],
      "env": {
        "GMAIL_OAUTH_TOKEN": "your-gmail-token",
        "LINEAR_API_KEY": "your-linear-key",
        "SYNC_INTERVAL": "300",
        "CACHE_ENABLED": "true",
        "MAX_BATCH_SIZE": "50"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Gmail OAuth tokens
- Linear API access
- Authentication system
- Data processor
- Event handler

## Related Servers

- modelcontextprotocol-gmail-server
- roychri-mcp-server-asana
- sooperset-mcp-atlassian
