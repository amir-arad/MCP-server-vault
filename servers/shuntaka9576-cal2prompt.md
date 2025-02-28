---
type: server
repo_url: https://github.com/shuntaka9576/cal2prompt
name: Cal2Prompt MCP Server
owner: shuntaka9576
stars: 2
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "purpose/scheduling",
    "purpose/task-management",
    "integration/calendar",
  ]
---

# Cal2Prompt MCP Server

#status/active #category/productivity #purpose/scheduling #purpose/task-management #integration/calendar

## Description

Integrates with calendar APIs to fetch event data and generate context-aware prompts, enabling automated scheduling assistance and task management.

## Features

- Calendar integration
- Event data fetching
- Context-aware prompts
- Scheduling assistance
- Task management
- Automated prompts
- Event analysis
- Time optimization

## Installation

```bash
npm install @shuntaka9576/cal2prompt
```

## Usage

```javascript
{
  "mcpServers": {
    "cal2prompt": {
      "command": "npx",
      "args": ["@shuntaka9576/cal2prompt"],
      "env": {
        "CALENDAR_PROVIDER": "google",
        "CALENDAR_ID": "primary",
        "PROMPT_TEMPLATE": "./templates/default.txt",
        "LOOKAHEAD_DAYS": "7"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Calendar API access
- Authentication tokens
- Template system

## Related Servers

- GongRzhe/Calendar-Autoauth-MCP-Server
