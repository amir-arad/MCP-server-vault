---
type: server
repo_url: https://github.com/Funmula-Corp/BigGo-MCP-Server
name: BigGo MCP Server
owner: Funmula-Corp
stars: 3
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "category/e-commerce",
    "purpose/product-search",
    "purpose/price-tracking",
  ]
---

# BigGo MCP Server

#status/active #category/e-commerce #purpose/product-search #purpose/price-tracking

## Description

A Model Context Protocol server enabling product searches across e-commerce platforms, price history tracking, and product specification-based searches using natural language prompts.

## Features

- Cross-platform product search
- Price history tracking
- Specification-based search
- Natural language processing
- Product comparison
- Price alerts
- Trend analysis
- Market insights

## Installation

```bash
npm install @funmula-corp/biggo-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "biggo": {
      "command": "npx",
      "args": ["@funmula-corp/biggo-mcp"],
      "env": {
        "API_KEY": "your-api-key",
        "SEARCH_LIMIT": "100",
        "PRICE_HISTORY_DAYS": "90",
        "UPDATE_INTERVAL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- API access
- Database storage
- Price tracking system

## Related Servers

- None currently listed
