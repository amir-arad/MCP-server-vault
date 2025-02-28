---
type: server
repo_url: https://github.com/mlobo2012/Claude_Desktop_API_USE_VIA_MCP
name: Claude Desktop API MCP Server
owner: mlobo2012
stars: 2
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/ai",
    "integration/claude",
    "purpose/api-access",
    "purpose/conversation-management",
    "tech/typescript",
  ]
---

# Claude Desktop API MCP Server

#status/active #category/ai #integration/claude #purpose/api-access #purpose/conversation-management #tech/typescript

## Description

Integrates Claude API features, enabling direct API access, extended context windows, and advanced conversation management. Helpful to bypass standard daily limits of Claude.ai.

## Features

- Direct API integration
- Extended context windows
- Conversation management
- Session handling
- Rate limit management
- Context preservation
- History tracking
- Response streaming
- Error handling
- Usage analytics

## Installation

```bash
npm install @mlobo2012/claude-desktop-api-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "claude-api": {
      "command": "npx",
      "args": ["@mlobo2012/claude-desktop-api-mcp"],
      "env": {
        "CLAUDE_API_KEY": "your-api-key",
        "MAX_CONTEXT_LENGTH": "100000",
        "PRESERVE_HISTORY": "true",
        "STREAM_RESPONSES": "true",
        "RATE_LIMIT": "50"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Claude API key
- TypeScript runtime
- WebSocket support
- Storage backend
- Rate limiter

## Related Servers

- pyroprompts-any-chat-completions-mcp
- dmontgomery40-deepseek-mcp-server
- kivo360-anthropic-mcp-code-analyzer
