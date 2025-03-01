---
type: server
repo_url: https://github.com/identimoji/mcp-server-emojikey
name: Emojikey MCP Server
owner: identimoji
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/personalization",
    "integration/supabase",
    "purpose/interaction-styles",
    "category/llm",
    "tech/emoji",
    "tech/javascript",
  ]
---

# Emojikey MCP Server

#status/active #category/personalization #integration/supabase #purpose/interaction-styles #category/llm #tech/emoji

## Description

Integrates with Supabase to persist and retrieve LLM interaction styles using emojikeys, enabling consistent personalized experiences across conversations.

## Features

- Emoji-based interaction styles
- Style persistence
- Style retrieval
- LLM integration
- Supabase integration
- Style customization
- User preferences
- Cross-session consistency
- Style management
- Emoji mapping

## Installation

```bash
npm install @identimoji/mcp-server-emojikey
```

## Usage

```javascript
{
  "mcpServers": {
    "emojikey": {
      "command": "npx",
      "args": ["@identimoji/mcp-server-emojikey"],
      "env": {
        "SUPABASE_URL": "your-project-url",
        "SUPABASE_KEY": "your-api-key",
        "DEFAULT_STYLE": "🤖",
        "CACHE_TTL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Supabase account
- Supabase client
- LLM integration
- Database access

## Related Servers

- None currently listed
