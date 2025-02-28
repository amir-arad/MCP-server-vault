---
type: server
repo_url: https://github.com/alexgoller/mcp-server-agenda
name: Agenda MCP Server
owner: alexgoller
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/agenda",
    "purpose/note-management",
    "tech/macos",
  ]
---

# Agenda MCP Server

#status/active #category/productivity #integration/agenda #purpose/note-management #tech/macos

## Description

Integrates with Agenda note-taking app on macOS to enable creating notes, managing projects, and opening existing notes using x-callback-urls.

## Features

- Note creation and management
- Project organization
- x-callback-url integration
- macOS integration
- Agenda app automation
- Note linking and referencing

## Installation

```bash
npm install @alexgoller/mcp-server-agenda
```

## Usage

```javascript
{
  "mcpServers": {
    "agenda": {
      "command": "npx",
      "args": ["@alexgoller/mcp-server-agenda"],
      "env": {
        "AGENDA_CALLBACK_URL": "agenda://",
        "DEFAULT_PROJECT": "Inbox",
        "NOTE_FORMAT": "markdown"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- macOS
- Agenda app
- x-callback-url support

## Related Servers

- None currently listed
