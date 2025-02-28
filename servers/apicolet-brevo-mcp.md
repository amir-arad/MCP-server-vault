---
type: server
repo_url: https://github.com/apicolet/brevo-mcp
name: Brevo MCP Server
owner: apicolet
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/communication",
    "integration/brevo",
    "purpose/email-management",
    "tech/typescript",
  ]
---

# Brevo MCP Server

#status/active #category/communication #integration/brevo #purpose/email-management #tech/typescript

## Description

A TypeScript server enabling integration with the Brevo (Sendinblue) API for managing contacts, sending emails, and tracking email events in multi-channel applications like Claude Desktop.

## Features

- Contact management
- Email sending
- Event tracking
- Multi-channel support
- TypeScript implementation
- API integration
- Analytics tracking
- Campaign management

## Installation

```bash
npm install @apicolet/brevo-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "brevo": {
      "command": "npx",
      "args": ["@apicolet/brevo-mcp"],
      "env": {
        "BREVO_API_KEY": "your-api-key",
        "DEFAULT_SENDER": "noreply@example.com",
        "TRACKING_ENABLED": "true",
        "TEMPLATE_DIR": "./templates"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- TypeScript >= 4.5
- Brevo account
- API credentials

## Related Servers

- None currently listed
