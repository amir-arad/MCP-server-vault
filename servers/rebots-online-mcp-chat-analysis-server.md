---
type: server
repo_url: https://github.com/rebots-online/mcp-chat-analysis-server
name: Chat Analysis MCP Server
owner: rebots-online
stars: 6
last_updated: 2025-01-24
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/ai",
    "category/analytics",
    "purpose/chat-analysis",
    "tech/vector-embeddings",
    "tech/knowledge-graphs",
  ]
---

# Chat Analysis MCP Server

#status/active #category/ai #category/analytics #purpose/chat-analysis #tech/vector-embeddings #tech/knowledge-graphs

## Description

Facilitates semantic analysis of chat conversations through vector embeddings and knowledge graphs, offering tools for semantic search, concept extraction, and conversation pattern analysis.

## Features

- Semantic chat analysis
- Vector embeddings generation
- Knowledge graph construction
- Pattern recognition
- Concept extraction
- Sentiment analysis
- Topic modeling
- Conversation clustering
- Semantic search
- Trend identification

## Installation

```bash
npm install @rebots-online/mcp-chat-analysis
```

## Usage

```javascript
{
  "mcpServers": {
    "chat-analysis": {
      "command": "npx",
      "args": ["@rebots-online/mcp-chat-analysis"],
      "env": {
        "EMBEDDING_MODEL": "all-MiniLM-L6-v2",
        "VECTOR_DB_URL": "your-vector-db-url",
        "GRAPH_DB_URL": "your-graph-db-url",
        "MAX_BATCH_SIZE": "1000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Vector database
- Graph database
- Embedding model
- NLP libraries
- Analysis tools

## Related Servers

- chatmcp/mcp-server-chatsum
- mcpso/mcp-server-chatsum
- shin-t-o-mcp-access
