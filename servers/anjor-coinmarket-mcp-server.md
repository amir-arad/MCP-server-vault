---
type: server
repo_url: https://github.com/anjor/coinmarket-mcp-server
name: CoinMarket MCP Server
owner: anjor
stars: 18
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/finance",
    "integration/coinmarket",
    "purpose/market-data",
    "category/cryptocurrency",
    "purpose/quotes",
  ]
---

# CoinMarket MCP Server

#status/active #category/finance #integration/coinmarket #purpose/market-data #category/cryptocurrency #purpose/quotes

## Description

Coinmarket API integration to fetch cryptocurrency listings and quotes. This MCP server provides comprehensive access to cryptocurrency market data and pricing information.

## Features

- Cryptocurrency listings
- Price quotes
- Market data
- Real-time updates
- Currency conversion
- Market rankings
- Price alerts
- Volume tracking
- Market cap data
- Trend analysis

## Installation

```bash
npm install @anjor/coinmarket-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "coinmarket": {
      "command": "npx",
      "args": ["@anjor/coinmarket-mcp"],
      "env": {
        "COINMARKET_API_KEY": "your-api-key",
        "UPDATE_FREQUENCY": "300",
        "BASE_CURRENCY": "USD",
        "MAX_LISTINGS": "5000",
        "CACHE_TTL": "60"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Coinmarket API key
- HTTP client
- Cache system
- Data processor
- Event emitter

## Related Servers

- longmans/coin_api_mcp
- quantgeekdev/coincap-mcp
- crazyrabbitltc/mcp-coingecko-server
