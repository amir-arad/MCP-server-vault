---
type: server
repo_url: https://github.com/Dhravya/apple-mcp
name: Apple MCP Server
owner: Dhravya
stars: 227
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/integration", "integration/apple", "purpose/app-control", "tech/macos"]
---

# Apple MCP Server

#status/active #category/integration #integration/apple #purpose/app-control #tech/macos

## Description

Enables interaction with Apple apps like Messages, Notes, and Contacts through the MCP protocol to send messages, search, and open app content using natural language.

## Features

- Messages app integration
- Notes app access
- Contacts management
- Natural language control
- App content search
- Message sending
- Contact lookup
- Note creation/editing

## Installation

```bash
npm install @dhravya/apple-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "apple": {
      "command": "npx",
      "args": ["@dhravya/apple-mcp"],
      "env": {
        "APPLE_ID": "your-apple-id",
        "APP_PASSWORD": "your-app-specific-password",
        "ALLOWED_APPS": "messages,notes,contacts",
        "DEFAULT_LANGUAGE": "en-US"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- macOS
- Apple ID
- App-specific password

## Related Servers

- RafalWilinski/mcp-apple-notes
- sirmews/apple-notes-mcp
- turlockmike/apple-notifier-mcp
- recursechat/mcp-server-apple-shortcuts
- kennethreitz/mcp-applemusic
- joshrutkowski/applescript-mcp