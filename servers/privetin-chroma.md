---
type: server
repo_url: https://github.com/privetin/chroma
name: ChromaDB MCP Server
owner: privetin
stars: 0
last_updated: 2025-02-28
status: inactive
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/inactive",
    "category/database",
    "integration/chromadb",
    "purpose/vector-search",
    "category/ai",
    "purpose/document-management",
  ]
---

# ChromaDB MCP Server

#status/inactive #category/database #integration/chromadb #purpose/vector-search #category/ai #purpose/document-management

## Description

Integrates ChromaDB vector database capabilities for efficient semantic document search, storage, and retrieval in natural language processing and information retrieval applications.

> **Note**: This server is currently inactive as the repository is no longer accessible.

## Features

- Vector database integration
- Semantic document search
- Document embedding storage
- Similarity matching
- Collection management
- Query optimization
- Metadata handling
- Batch operations
- Real-time indexing
- Multi-modal support

## Installation

```bash
npm install @privetin/chroma-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "chroma": {
      "command": "npx",
      "args": ["@privetin/chroma-mcp"],
      "env": {
        "CHROMA_HOST": "localhost",
        "CHROMA_PORT": "8000",
        "EMBEDDING_MODEL": "all-MiniLM-L6-v2",
        "MAX_BATCH_SIZE": "1000",
        "DISTANCE_METRIC": "cosine"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- ChromaDB instance
- Embedding model
- Vector operations library
- Document processor
- Storage backend

## Related Servers

- qdrant-mcp-server-qdrant
- modelcontextprotocol-memory-server
- needle-ai-needle-mcp