---
type: server
repo_url: https://github.com/CamdenClark/anki-mcp-server
name: Anki MCP Server
owner: CamdenClark
stars: 7
last_updated: 2025-02-08
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/education", "integration/anki", "purpose/learning"]
---

# Anki MCP Server

#status/active #category/education #integration/anki #purpose/learning

## Description

Integrates with Anki flashcard decks via AnkiConnect to enable automated creation, retrieval, and management of study materials.

## Features

- AnkiConnect integration
- Flashcard creation
- Deck management
- Card retrieval
- Study material automation
- Note organization
- Tag management
- Media handling

## Installation

```bash
npm install @camdenclark/anki-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "anki": {
      "command": "npx",
      "args": ["@camdenclark/anki-mcp"],
      "env": {
        "ANKI_CONNECT_URL": "http://localhost:8765",
        "DEFAULT_DECK": "Default",
        "NOTE_TYPE": "Basic",
        "MEDIA_DIR": "./media"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Anki desktop app
- AnkiConnect plugin
- Local Anki instance

## Related Servers

- scorzeth/anki-mcp-server
- samefarrar/mcp-ankiconnect