---
type: server
repo_url: https://github.com/GongRzhe/Calendar-Autoauth-MCP-Server
name: Calendar Autoauth MCP Server
owner: GongRzhe
stars: 2
last_updated: 2025-02-14
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/google",
    "purpose/calendar-management",
    "integration/claude",
  ]
---

# Calendar Autoauth MCP Server

#status/active #category/productivity #integration/google #purpose/calendar-management #integration/claude

## Description

Server for Google Calendar integration in Claude Desktop with auto authentication support. This server enables AI assistants to manage Google Calendar events through natural language interactions.

## Features

- Google Calendar integration
- Auto authentication
- Natural language support
- Event management
- AI assistant integration
- Calendar operations
- Authentication handling
- Event scheduling

## Installation

```bash
npm install @gongrzhe/calendar-autoauth-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "calendar-autoauth": {
      "command": "npx",
      "args": ["@gongrzhe/calendar-autoauth-mcp"],
      "env": {
        "GOOGLE_CLIENT_ID": "your-client-id",
        "GOOGLE_CLIENT_SECRET": "your-client-secret",
        "DEFAULT_CALENDAR": "primary",
        "AUTH_PORT": "3000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Google Cloud account
- OAuth credentials
- Claude Desktop

## Related Servers

- shuntaka9576/cal2prompt
