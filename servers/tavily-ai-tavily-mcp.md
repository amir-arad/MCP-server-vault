---
type: server
repo_url: https://github.com/tavily-ai/tavily-mcp
name: Tavily
owner: tavily-ai
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/search", "category/ai"]
---

#status/active #status/official #category/search #category/ai

# Tavily

## Description

Search engine for AI agents (search + extract) powered by [Tavily](https://tavily.com/). This MCP server provides AI-optimized search capabilities specifically designed for AI agents to efficiently find and extract information.

## Features

- AI-optimized search
- Content extraction
- Semantic understanding
- Context-aware results
- Structured data extraction
- Real-time search
- Topic classification
- Entity recognition
- Relevance ranking
- Multi-format support

## Installation

```bash
npm install @tavily/mcp-server
```

## Usage

```javascript
import { TavilyServer } from "@tavily/mcp-server";

const server = new TavilyServer({
  apiKey: "your-tavily-api-key",
});

// Perform AI-optimized search
const searchResults = await server.search({
  query: "Latest developments in quantum computing",
  options: {
    searchDepth: "comprehensive",
    includeImages: true,
    includeDomains: ["arxiv.org", "nature.com"],
    excludeDomains: ["wikipedia.org"],
    publishedTime: "past_year",
  },
});

// Extract specific information
const extraction = await server.extract({
  url: "https://example.com/article",
  extractionRules: {
    title: true,
    author: true,
    publishDate: true,
    mainContent: true,
    citations: true,
  },
});

// Analyze topic relevance
const topicAnalysis = await server.analyzeTopic({
  query: "artificial intelligence ethics",
  content: "Article content here...",
  aspects: [
    "technical_accuracy",
    "ethical_considerations",
    "practical_applications",
  ],
});

// Get structured data
const structuredData = await server.getStructuredData({
  query: "machine learning frameworks comparison",
  format: "comparison_table",
  attributes: [
    "name",
    "language",
    "learning_curve",
    "community_size",
    "performance",
  ],
});
```

## Dependencies

- Node.js >= 14.x
- Tavily account
- Tavily API key

## Related Servers

- None currently listed
