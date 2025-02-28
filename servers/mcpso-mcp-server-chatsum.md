---
type: server
repo_url: https://github.com/mcpso/mcp-server-chatsum
name: Chatsum MCP Server by mcpso
owner: mcpso
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
    "purpose/query",
    "purpose/content-processing",
  ]
---

# Chatsum MCP Server by mcpso

#status/active #category/ai #purpose/summarization #category/chat #purpose/query #purpose/content-processing

## Description

Query and Summarize chat messages with LLM. This MCP server, developed by mcpso, provides advanced capabilities for both querying and summarizing chat conversations using large language models.

## Features

- Chat message summarization
- Query-based information extraction
- Semantic search
- Topic clustering
- Conversation analysis
- Custom query templates
- Batch processing
- Real-time analysis
- Multi-language support
- Context preservation

## Installation

```bash
npm install @mcpso/mcp-server-chatsum
```

## Usage

```javascript
{
  "mcpServers": {
    "chatsum": {
      "command": "npx",
      "args": ["@mcpso/mcp-server-chatsum"],
      "env": {
        "LLM_MODEL": "gpt-4",
        "MAX_TOKENS": "4096",
        "QUERY_TIMEOUT": "30000",
        "LANGUAGE": "en",
        "ENABLE_STREAMING": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- LLM API access
- Vector database
- NLP libraries
- Query processor
- Summarization engine

## Related Servers

- chatmcp/mcp-server-chatsum
- rebots-online-mcp-chat-analysis-server
- shin-t-o-mcp-access
