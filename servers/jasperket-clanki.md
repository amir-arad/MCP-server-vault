---
type: server
repo_url: https://github.com/jasperket/clanki
name: Clanki MCP Server
owner: jasperket
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/education",
    "integration/anki",
    "purpose/learning",
    "purpose/flashcards",
    "tech/javascript",
    "tech/typescript",
  ]
---

# Clanki MCP Server

#status/active #category/education #integration/anki #purpose/learning #purpose/flashcards #tech/javascript

## Description

Integrates with Anki flashcards to provide card creation and deck management capabilities. This MCP server enables automated flashcard management and learning optimization through the Anki platform.

## Features

- Card creation
- Deck management
- Study scheduling
- Progress tracking
- Template customization
- Media handling
- Tag organization
- Review statistics
- Sync support
- Backup management

## Installation

```bash
npm install @jasperket/clanki
```

## Usage

```javascript
{
  "mcpServers": {
    "clanki": {
      "command": "npx",
      "args": ["@jasperket/clanki"],
      "env": {
        "ANKI_CONNECT_URL": "http://localhost:8765",
        "DEFAULT_DECK": "Default",
        "MEDIA_PATH": "./media",
        "SYNC_ON_CHANGE": "true",
        "BACKUP_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Anki desktop app
- AnkiConnect plugin
- Media processor
- Sync manager
- Backup system

## Related Servers

- scorzeth-anki-mcp-server
- samefarrar-mcp-ankiconnect
- camdenclark-anki-mcp-server
