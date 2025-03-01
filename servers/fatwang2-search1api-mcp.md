---
type: server
repo_url: https://github.com/fatwang2/search1api-mcp
name: Search1API
owner: fatwang2
stars: 85
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags:
  [
    "status/active",
    "status/official",
    "category/search",
    "category/web-scraping",
    "tech/javascript",
    "tech/typescript",
  ]
---

# Search1API

#status/active #status/official #category/search #category/web-scraping

## Description

One API for Search, Crawling, and Sitemaps. This MCP server provides a unified interface for web search, crawling, and sitemap management capabilities.

## Features

- Unified search interface
- Web crawling capabilities
- Sitemap generation
- Sitemap parsing
- Search result aggregation
- Custom crawling rules
- Rate limiting control
- Data extraction
- Search filtering
- Multi-source search

## Installation

```bash
npm install @search1api/mcp-server
```

## Usage

```javascript
import { Search1APIServer } from "@search1api/mcp-server";

const server = new Search1APIServer({
  apiKey: "your-search1api-key",
});

// Perform a search
const searchResults = await server.search({
  query: "artificial intelligence trends",
  options: {
    sources: ["web", "news", "academic"],
    limit: 20,
    language: "en",
    timeRange: "past_month",
  },
});

// Crawl a website
const crawlResult = await server.crawl({
  url: "https://example.com",
  options: {
    depth: 3,
    followLinks: true,
    respectRobotsTxt: true,
    customRules: {
      include: ["/blog/*", "/docs/*"],
      exclude: ["/private/*"],
    },
  },
});

// Generate sitemap
const sitemap = await server.generateSitemap({
  domain: "example.com",
  options: {
    includeImages: true,
    changefreq: "weekly",
    priority: 0.8,
    lastmod: true,
  },
});

// Parse existing sitemap
const parsedSitemap = await server.parseSitemap({
  url: "https://example.com/sitemap.xml",
  options: {
    validateUrls: true,
    extractMetadata: true,
  },
});
```

## Dependencies

- Node.js >= 14.x
- Search1API account
- Search1API API key

## Related Servers

- None currently listed
