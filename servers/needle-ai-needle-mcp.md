--- 
type: server
repo_url: https://github.com/needle-ai/needle-mcp
name: Needle
owner: needle-ai
stars: 20
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags:
  ["status/active", "status/official", "category/ai", "category/knowledge-base"]
---

#status/active #status/official #category/ai #category/knowledge-base

# Needle

## Description

Production-ready RAG (Retrieval-Augmented Generation) out of the box to search and retrieve data from your own documents. This MCP server provides advanced document processing and retrieval capabilities using AI technology.

## Features

- Document indexing and processing
- Semantic search capabilities
- RAG implementation
- Document embedding generation
- Context-aware retrieval
- Multi-format document support
- Automatic text chunking
- Vector similarity search
- Query optimization
- Real-time document updates

## Installation

```bash
npm install @needle-ai/mcp-server
```

## Usage

```javascript
import { NeedleServer } from "@needle-ai/mcp-server";

const server = new NeedleServer({
  apiKey: "your-needle-api-key",
  embeddingModel: "default",
});

// Index documents
await server.indexDocuments({
  documents: [
    {
      id: "doc1",
      content: "Technical documentation content...",
      metadata: {
        type: "technical",
        author: "John Doe",
      },
    },
  ],
  options: {
    chunkSize: 500,
    overlap: 50,
  },
});

// Perform semantic search
const results = await server.search({
  query: "How to implement authentication?",
  options: {
    maxResults: 5,
    minRelevance: 0.7,
    includeMetadata: true,
  },
});

// Generate RAG response
const response = await server.generateResponse({
  query: "Explain the deployment process",
  options: {
    maxTokens: 500,
    temperature: 0.7,
    contextWindow: 2000,
  },
});
```

## Dependencies

- Node.js >= 14.x
- Needle AI account
- Needle AI API key
- Vector database (optional)

## Related Servers

- None currently listed