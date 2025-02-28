---
type: server
repo_url: https://github.com/chatmcp/mcp-server-chatsum
name: Chatsum MCP Server
owner: chatmcp
stars: 449
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/ai",
    "purpose/summarization",
    "category/chat",
    "purpose/content-processing",
  ]
---

# Chatsum MCP Server

#status/active #category/ai #purpose/summarization #category/chat #purpose/content-processing

## Description

Summarizes your chat messages. This MCP server provides intelligent chat message summarization capabilities, helping users extract key information and insights from conversations.

## Features

- Chat message summarization
- Key points extraction
- Topic identification
- Conversation analysis
- Length customization
- Format options
- Batch processing
- Real-time summarization
- Multi-language support
- Context preservation

## Installation

```bash
npm install @chatmcp/mcp-server-chatsum
```

## Usage

```javascript
{
  "mcpServers": {
    "chatsum": {
      "command": "npx",
      "args": ["@chatmcp/mcp-server-chatsum"],
      "env": {
        "MODEL_TYPE": "gpt-4",
        "MAX_TOKEN_LENGTH": "4096",
        "MIN_SUMMARY_LENGTH": "100",
        "LANGUAGE": "en",
        "PRESERVE_CONTEXT": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- GPT model access
- NLP libraries
- Text processing tools
- Language detection
- Summarization algorithms

## Related Servers

- mcpso/mcp-server-chatsum
- rebots-online-mcp-chat-analysis-server
- shin-t-o-mcp-access
