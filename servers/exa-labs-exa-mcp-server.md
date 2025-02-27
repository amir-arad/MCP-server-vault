---
type: server
repo_url: https://github.com/exa-labs/exa-mcp-server
name: Exa
owner: exa-labs
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/search", "category/ai"]
---

#status/active #status/official #category/search #category/ai

# Exa

## Description

Search Engine made for AIs by [Exa](https://exa.ai). This MCP server provides AI-optimized search capabilities, designed specifically for AI agents to efficiently find and process information.

## Features

- AI-optimized search algorithms
- Semantic understanding of queries
- Context-aware search results
- Structured data extraction
- Real-time search capabilities
- Advanced filtering options
- Integration with Exa's AI search platform

## Installation

```bash
npm install @exa/mcp-server
```

## Usage

```javascript
import { ExaServer } from "@exa/mcp-server";

const server = new ExaServer({
  apiKey: "your-exa-api-key",
});

// Perform an AI-optimized search
const results = await server.search({
  query: "Latest developments in quantum computing",
  filters: {
    date: "past_year",
    type: "research_paper",
  },
  maxResults: 10,
});
```

## Dependencies

- Node.js >= 14.x
- Exa API key
- Active Exa account

## Related Servers

- None currently listed
