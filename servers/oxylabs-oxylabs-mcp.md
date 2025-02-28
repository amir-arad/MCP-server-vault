---
type: server
repo_url: https://github.com/oxylabs/oxylabs-mcp
name: Oxylabs
owner: oxylabs
stars: 2
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags: ["status/active", "status/official", "category/web-scraping"]
---

#status/active #status/official #category/web-scraping

# Oxylabs

## Description

Scrape websites with Oxylabs Web API, supporting dynamic rendering and parsing for structured data extraction. This MCP server provides enterprise-grade web scraping capabilities with advanced features for handling complex websites.

## Features

- Advanced web scraping
- Dynamic page rendering
- Structured data extraction
- Proxy management
- JavaScript execution
- Anti-bot bypass
- Rate limiting
- Geolocation targeting
- Custom headers support
- Data parsing and formatting

## Installation

```bash
npm install @oxylabs/mcp-server
```

## Usage

```javascript
import { OxylabsServer } from "@oxylabs/mcp-server";

const server = new OxylabsServer({
  apiKey: "your-oxylabs-api-key",
});

// Scrape a website with dynamic rendering
const data = await server.scrape({
  url: "https://example.com/products",
  options: {
    renderJs: true,
    waitFor: ".product-grid",
    geolocation: "United States",
    device: "desktop",
  },
});

// Extract structured data
const products = await server.extract({
  url: "https://example.com/products",
  selectors: {
    products: {
      selector: ".product-item",
      multiple: true,
      data: {
        name: ".product-name",
        price: {
          selector: ".price",
          transform: (text) => parseFloat(text.replace("$", "")),
        },
        description: ".description",
        image: {
          selector: "img",
          attr: "src",
        },
      },
    },
  },
});

// Handle pagination
const allProducts = await server.scrapeAll({
  url: "https://example.com/products",
  pagination: {
    type: "infinite-scroll",
    itemSelector: ".product-item",
    maxPages: 10,
  },
  parser: (html) => {
    // Custom parsing logic
    return extractProductData(html);
  },
});
```

## Dependencies

- Node.js >= 14.x
- Oxylabs account
- Oxylabs API key
- Active subscription plan

## Related Servers

- None currently listed
