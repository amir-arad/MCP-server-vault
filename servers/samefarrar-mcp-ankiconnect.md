---
type: server
repo_url: https://github.com/samefarrar/mcp-ankiconnect
name: AnkiConnect MCP Server
owner: samefarrar
stars: 3
last_updated: 2025-02-07
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/education", "integration/anki", "purpose/learning"]
---

# AnkiConnect MCP Server

#status/active #category/education #integration/anki #purpose/learning

## Description

Integrates Anki flashcard functionality, enabling natural language interactions for spaced repetition learning within conversations.

## Features

- Natural language interactions
- Spaced repetition learning
- Conversational flashcards
- Dynamic card creation
- Review scheduling
- Progress tracking
- Learning analytics
- Multi-deck support

## Installation

```bash
npm install @samefarrar/mcp-ankiconnect
```

## Usage

```javascript
{
  "mcpServers": {
    "ankiconnect": {
      "command": "npx",
      "args": ["@samefarrar/mcp-ankiconnect"],
      "env": {
        "ANKI_CONNECT_URL": "http://localhost:8765",
        "DEFAULT_DECK": "Main",
        "LANGUAGE_MODEL": "default",
        "SYNC_INTERVAL": "300"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Anki desktop app
- AnkiConnect plugin
- Natural language processing

## Related Servers

- CamdenClark/anki-mcp-server
- scorzeth/anki-mcp-server