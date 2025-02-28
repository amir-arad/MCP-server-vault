---
type: server
repo_url: https://github.com/qpd-v/mcp-communicator-telegram
name: Telegram Communicator MCP Server
owner: qpd-v
stars: 8
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/communication",
    "integration/telegram",
    "purpose/messaging",
    "purpose/interaction",
    "tech/bot",
  ]
---

# Telegram Communicator MCP Server

#status/active #category/communication #integration/telegram #purpose/messaging #purpose/interaction #tech/bot

## Description

An MCP server that enables communication with users through Telegram. This server provides a tool to ask questions to users and receive their responses via a Telegram bot.

## Features

- Telegram integration
- Bot communication
- Question handling
- Response collection
- User interaction
- Message formatting
- Media support
- User management
- Chat history
- Notification system

## Installation

```bash
npm install @qpd-v/mcp-communicator-telegram
```

## Usage

```javascript
{
  "mcpServers": {
    "telegram": {
      "command": "npx",
      "args": ["@qpd-v/mcp-communicator-telegram"],
      "env": {
        "TELEGRAM_BOT_TOKEN": "your-bot-token",
        "ALLOWED_USERS": "*",
        "MESSAGE_TIMEOUT": "300",
        "HISTORY_ENABLED": "true",
        "MEDIA_SUPPORT": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Telegram Bot API
- Message handler
- User manager
- History tracker
- Media processor

## Related Servers

- modelcontextprotocol-slack-server
- modelcontextprotocol-communication-server
- apicolet-brevo-mcp
