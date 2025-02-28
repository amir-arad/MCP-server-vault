---
type: server
repo_url: https://github.com/scorzeth/anki-mcp-server
name: Anki MCP Server
owner: scorzeth
stars: 17
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/education", "integration/anki", "purpose/learning", "category/ai"]
---

# Anki MCP Server

#status/active #category/education #integration/anki #purpose/learning #category/ai

## Description

Integrates with Anki to enable AI-driven flashcard creation, retrieval, and review processes for enhanced spaced repetition learning.

## Features

- AI-driven flashcard creation
- Spaced repetition optimization
- Smart review scheduling
- Content generation
- Learning pattern analysis
- Progress tracking
- Deck organization
- Performance analytics

## Installation

```bash
npm install @scorzeth/anki-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "anki": {
      "command": "npx",
      "args": ["@scorzeth/anki-mcp"],
      "env": {
        "ANKI_CONNECT_URL": "http://localhost:8765",
        "AI_MODEL": "gpt-4",
        "LEARNING_STYLE": "adaptive",
        "REVIEW_INTERVAL": "optimal"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Anki desktop app
- AnkiConnect plugin
- AI model access (optional)

## Related Servers

- CamdenClark/anki-mcp-server
- samefarrar/mcp-ankiconnect