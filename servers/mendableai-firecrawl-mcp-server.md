---
type: server
repo_url: https://github.com/mendableai/firecrawl-mcp-server
name: Firecrawl
owner: mendableai
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/web-scraping"]
---

#status/active #status/official #category/web-scraping

# Firecrawl

## Description

Extract web data with [Firecrawl](https://firecrawl.dev). This MCP server provides powerful web scraping and data extraction capabilities, allowing you to efficiently collect and process web content.

## Features

- Advanced web scraping capabilities
- Automated data extraction
- Support for dynamic websites
- Rate limiting and proxy management
- Custom extraction rules
- Structured data output
- Browser-based rendering support

## Installation

```bash
npm install @firecrawl/mcp-server
```

## Usage

```javascript
import { FirecrawlServer } from "@firecrawl/mcp-server";

const server = new FirecrawlServer({
  apiKey: "your-firecrawl-api-key",
});

// Extract data from a webpage
const data = await server.extract({
  url: "https://example.com/products",
  selectors: {
    title: ".product-title",
    price: ".product-price",
    description: ".product-description",
  },
  pagination: {
    enabled: true,
    maxPages: 5,
  },
});
```

## Dependencies

- Node.js >= 14.x
- Firecrawl API key
- Active Firecrawl account

## Related Servers

- None currently listed
