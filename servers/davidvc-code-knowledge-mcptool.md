--- 
type: server
repo_url: https://github.com/davidvc/code-knowledge-mcptool
name: Code Knowledge MCP Server
owner: davidvc
stars: 8
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/knowledge-base",
    "purpose/code-understanding",
    "tech/rag",
    "category/ai",
    "purpose/documentation",
  ]
---

# Code Knowledge MCP Server

#status/active #category/knowledge-base #purpose/code-understanding #tech/rag #category/ai #purpose/documentation

## Description

Provides a project memory bank and RAG context provider for enhanced code understanding and management through vector embeddings, integrated with RooCode and Cline.

## Features

- Memory bank storage
- RAG context provision
- Vector embeddings
- Code understanding
- Knowledge retrieval
- Context management
- Integration support
- Search capabilities
- Version tracking
- Documentation linking

## Installation

```bash
npm install @davidvc/code-knowledge-mcptool
```

## Usage

```javascript
{
  "mcpServers": {
    "code-knowledge": {
      "command": "npx",
      "args": ["@davidvc/code-knowledge-mcptool"],
      "env": {
        "VECTOR_DB": "your-vector-db-url",
        "EMBEDDING_MODEL": "all-MiniLM-L6-v2",
        "PROJECT_ROOT": "./",
        "INDEX_INTERVAL": "3600",
        "CONTEXT_SIZE": "2048"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Vector database
- Embedding model
- RAG system
- Knowledge base
- Search engine

## Related Servers

- saiprashanths/code-analysis-mcp
- seanivore/mcp-code-analyzer
- modelcontextprotocol-memory-server