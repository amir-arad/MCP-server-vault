---
type: server
repo_url: https://github.com/r3-yamauchi/mcp-server-blastengine-mailer
name: Blastengine Mailer MCP Server
owner: r3-yamauchi
stars: 0
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/communication",
    "integration/blastengine",
    "purpose/email-automation",
  ]
---

# Blastengine Mailer MCP Server

#status/active #category/communication #integration/blastengine #purpose/email-automation

## Description

Integrates with Blastengine to enable sending emails via API, supporting automated notification and marketing campaign functionalities.

## Features

- Email sending automation
- Marketing campaign support
- Notification system
- Template management
- Campaign tracking
- Analytics integration
- List management
- Delivery monitoring

## Installation

```bash
npm install @r3-yamauchi/blastengine-mailer-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "blastengine": {
      "command": "npx",
      "args": ["@r3-yamauchi/blastengine-mailer-mcp"],
      "env": {
        "BLASTENGINE_API_KEY": "your-api-key",
        "BLASTENGINE_USER_ID": "your-user-id",
        "DEFAULT_FROM": "noreply@example.com",
        "TEMPLATE_PATH": "./templates"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Blastengine account
- API credentials
- Email templates

## Related Servers

- None currently listed
