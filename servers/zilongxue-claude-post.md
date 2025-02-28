---
type: server
repo_url: https://github.com/ZilongXue/claude-post
name: ClaudePost MCP Server
owner: ZilongXue
stars: 19
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/communication",
    "integration/gmail",
    "purpose/email-management",
    "tech/typescript",
    "category/ai",
  ]
---

# ClaudePost MCP Server

#status/active #category/communication #integration/gmail #purpose/email-management #tech/typescript #category/ai

## Description

ClaudePost enables seamless email management for Gmail, offering secure features like email search, reading, and sending. This MCP server provides AI-assisted email management capabilities through Gmail integration.

## Features

- Email search functionality
- Email reading
- Email composition
- Secure authentication
- Attachment handling
- Label management
- Thread organization
- Draft management
- Contact integration
- Filter creation

## Installation

```bash
npm install @zilongxue/claude-post
```

## Usage

```javascript
{
  "mcpServers": {
    "claude-post": {
      "command": "npx",
      "args": ["@zilongxue/claude-post"],
      "env": {
        "GMAIL_CLIENT_ID": "your-client-id",
        "GMAIL_CLIENT_SECRET": "your-client-secret",
        "OAUTH_REFRESH_TOKEN": "your-refresh-token",
        "MAX_RESULTS": "100",
        "CACHE_DURATION": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Gmail API access
- OAuth 2.0 credentials
- Email parser
- MIME handler
- Cache system

## Related Servers

- apicolet-brevo-mcp
- r3-yamauchi-mcp-server-blastengine-mailer
- modelcontextprotocol-gmail-server
