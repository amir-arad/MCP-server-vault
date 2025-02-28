---
type: server
repo_url: https://github.com/longmans/coin_api_mcp
name: CoinMarketCap API MCP Server
owner: longmans
stars: 6
last_updated: 2025-02-14
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/finance",
    "integration/coinmarketcap",
    "purpose/market-data",
    "category/cryptocurrency",
    "purpose/analytics",
  ]
---

# CoinMarketCap API MCP Server

#status/active #category/finance #integration/coinmarketcap #purpose/market-data #category/cryptocurrency #purpose/analytics

## Description

Integrates with CoinMarketCap's API to fetch and analyze cryptocurrency market data, supporting customizable queries for real-time information.

## Features

- Market data retrieval
- Price tracking
- Custom queries
- Real-time updates
- Market analytics
- Historical data
- Currency conversion
- Portfolio tracking
- Market metrics
- Data visualization

## Installation

```bash
npm install @longmans/coin-api-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "coinmarketcap": {
      "command": "npx",
      "args": ["@longmans/coin-api-mcp"],
      "env": {
        "CMC_API_KEY": "your-api-key",
        "UPDATE_INTERVAL": "300",
        "DEFAULT_CURRENCY": "USD",
        "MAX_COINS": "100",
        "CACHE_TTL": "60"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- CoinMarketCap API key
- Cache system
- Data processor
- HTTP client
- Analytics engine

## Related Servers

- raw391/coin_daemon_mcp
- quantgeekdev/coincap-mcp
- crazyrabbitltc/mcp-coingecko-server
