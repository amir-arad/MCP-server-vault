---
type: server
repo_url: https://github.com/J-Gal02/clicksend-mcp
name: ClickSend MCP Server
owner: J-Gal02
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/communication",
    "integration/clicksend",
    "purpose/sms",
    "purpose/text-to-speech",
    "tech/api",
    "tech/javascript",
  ]
---

# ClickSend MCP Server

#status/active #category/communication #integration/clicksend #purpose/sms #purpose/text-to-speech #tech/api

## Description

This server enables AI models to send SMS messages and initiate Text-to-Speech calls programmatically using ClickSend's API with built-in rate limiting and input validation.

## Features

- SMS messaging
- Text-to-Speech calls
- Rate limiting
- Input validation
- Message scheduling
- Delivery tracking
- Contact management
- Template support
- Error handling
- Usage analytics

## Installation

```bash
npm install @j-gal02/clicksend-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "clicksend": {
      "command": "npx",
      "args": ["@j-gal02/clicksend-mcp"],
      "env": {
        "CLICKSEND_USERNAME": "your-username",
        "CLICKSEND_API_KEY": "your-api-key",
        "RATE_LIMIT": "100",
        "MAX_BATCH_SIZE": "1000",
        "DEFAULT_COUNTRY": "US"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- ClickSend account
- API credentials
- Rate limiter
- Input validator
- Message formatter

## Related Servers

- apicolet-brevo-mcp
- r3-yamauchi-mcp-server-blastengine-mailer
- modelcontextprotocol-sms-server
