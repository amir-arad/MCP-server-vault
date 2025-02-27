---
type: server
repo_url: https://github.com/qdrant/mcp-server-qdrant/
name: Qdrant
owner: qdrant
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/database", "category/ai"]
---

#status/active #status/official #category/database #category/ai

# Qdrant

## Description

Implement semantic memory layer on top of the Qdrant vector search engine. This MCP server provides advanced vector similarity search capabilities for building semantic memory systems and AI applications.

## Features

- Vector similarity search
- Semantic memory storage
- High-dimensional indexing
- Real-time updates
- Filtering capabilities
- Payload storage
- Collection management
- Batch operations
- Query optimization
- Clustering support

## Installation

```bash
npm install @qdrant/mcp-server
```

## Usage

```javascript
import { QdrantServer } from '@qdrant/mcp-server';

const server = new QdrantServer({
  url: 'http://localhost:6333',
  apiKey: 'your-qdrant-api-key'
});

// Create a collection
await server.createCollection({
  name: 'semantic_memory',
  vectorSize: 768,
  distance: 'Cosine',
  config: {
    indexing: {
      type: 'hnsw',
      m: 16,
      efConstruction: 100
    }
  }
});

// Insert vectors with payload
await server.upsert({
  collection: 'semantic_memory',
  points: [
    {
      id: 1,
      vector: [0.1, 0.2, ...], // 768-dimensional vector
      payload: {
        text: 'Example memory content',
        timestamp: new Date().toISOString(),
        tags: ['important', 'context']
      }
    }
  ]
});

// Search similar vectors
const results = await server.search({
  collection: 'semantic_memory',
  vector: [0.15, 0.25, ...], // Query vector
  limit: 10,
  filter: {
    must: [
      {
        key: 'tags',
        match: {
          value: 'important'
        }
      }
    ]
  }
});

// Implement semantic memory operations
const memory = await server.semanticMemory({
  text: 'Remember this important information',
  embedding: {
    model: 'text-embedding-ada-002',
    options: {
      normalize: true
    }
  },
  metadata: {
    source: 'user-input',
    category: 'general'
  }
});
```

## Dependencies

- Node.js >= 14.x
- Qdrant instance
- Qdrant API key
- Vector embedding model (optional)

## Related Servers

- None currently listed
