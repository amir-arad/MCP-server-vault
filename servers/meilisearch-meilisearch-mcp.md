---
type: server
repo_url: https://github.com/meilisearch/meilisearch-mcp
name: Meilisearch
owner: meilisearch
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/search"]
---

#status/active #status/official #category/search

# Meilisearch

## Description

Interact & query with Meilisearch (Full-text & semantic search API). This MCP server provides integration with Meilisearch's powerful search engine, enabling fast and relevant search capabilities with typo tolerance and natural language understanding.

## Features

- Full-text search
- Semantic search capabilities
- Typo tolerance
- Custom ranking rules
- Faceted search
- Search-as-you-type
- Document indexing
- Custom synonyms
- Filtering capabilities
- Search result highlighting

## Installation

```bash
npm install @meilisearch/mcp-server
```

## Usage

```javascript
import { MeilisearchServer } from "@meilisearch/mcp-server";

const server = new MeilisearchServer({
  host: "http://localhost:7700",
  apiKey: "your-meilisearch-api-key",
});

// Index documents
await server.index({
  indexUid: "products",
  documents: [
    { id: 1, name: "iPhone 12", description: "Latest Apple smartphone" },
    { id: 2, name: "Samsung Galaxy", description: "Android flagship phone" },
  ],
});

// Perform a search
const results = await server.search({
  indexUid: "products",
  query: "smartphone",
  options: {
    limit: 20,
    offset: 0,
    filters: "price > 500",
    sort: ["price:desc"],
    facets: ["brand", "category"],
  },
});

// Update search settings
await server.updateSettings({
  indexUid: "products",
  settings: {
    rankingRules: [
      "words",
      "typo",
      "proximity",
      "attribute",
      "sort",
      "exactness",
    ],
    searchableAttributes: ["name", "description"],
  },
});
```

## Dependencies

- Node.js >= 14.x
- Meilisearch instance
- Meilisearch API key

## Related Servers

- None currently listed
