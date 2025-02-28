---
type: server
repo_url: https://github.com/v-3/discordmcp
name: Discord MCP Server
owner: v-3
stars: 16
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/communication",
    "integration/discord",
    "purpose/messaging",
    "tech/api",
    "category/ai",
  ]
---

To install Discord MCP Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@v-3/discordmcp):

```bash
npx -y @smithery/cli install @v-3/discordmcp --client claude
```

# Discord MCP Server

#status/active #category/communication #integration/discord #purpose/messaging #tech/api #category/ai

## Description

Enables LLMs to interact with Discord channels by sending and reading messages through Discord's API, with a focus on maintaining user control and security.

## Features

- Discord channel message reading
- Message sending capabilities
- User control and security features
- Discord API integration
- Channel management
- Message history access
- Real-time message monitoring
- Secure authentication handling
- Rate limit management
- Error handling and logging

## Installation

```bash
npm install @v-3/discordmcp
```

## Usage

```javascript
{
  "mcpServers": {
    "discord": {
      "command": "npx",
      "args": ["@v-3/discordmcp"],
      "env": {
        "DISCORD_TOKEN": "your-discord-bot-token",
        "DISCORD_CLIENT_ID": "your-client-id",
        "DISCORD_GUILD_ID": "your-guild-id"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Discord Bot Token
- Discord Developer Application
- Discord Server (Guild) permissions

## Related Servers

- None currently listed
