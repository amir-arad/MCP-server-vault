---
type: server
repo_url: https://github.com/kagisearch/kagimcp
name: Kagi Search
owner: kagisearch
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/search"]
---

#status/active #status/official #category/search

# Kagi Search

## Description

Search the web using Kagi's search API. This MCP server provides access to Kagi's powerful search capabilities, offering high-quality, privacy-focused web search results.

## Features

- Advanced web search capabilities
- Privacy-focused search results
- Customizable search parameters
- Rich search result metadata
- Fast response times
- Content filtering options
- Domain-specific searches
- Result ranking optimization

## Installation

```bash
npm install @kagi/mcp-server
```

## Usage

```javascript
import { KagiServer } from "@kagi/mcp-server";

const server = new KagiServer({
  apiKey: "your-kagi-api-key",
});

// Perform a web search
const results = await server.search({
  query: "latest developments in quantum computing",
  options: {
    language: "en",
    region: "us",
    timeRange: "past_year",
    safeSearch: true,
  },
});

// Get enriched results with metadata
const enrichedResults = await server.enrichedSearch({
  query: "machine learning frameworks",
  include: ["summary", "keywords", "readingTime"],
});

// Domain-specific search
const academicResults = await server.search({
  query: "neural networks research",
  filter: {
    domains: [".edu", ".ac.uk"],
    documentTypes: ["pdf", "research_paper"],
  },
});
```

## Dependencies

- Node.js >= 14.x
- Kagi API key
- Active Kagi subscription

## Related Servers

- None currently listed
