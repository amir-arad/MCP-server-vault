---
type: server
repo_url: https://github.com/QuantGeekDev/coincap-mcp
name: CoinCap MCP Server
owner: QuantGeekDev
stars: 16
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/finance",
    "integration/coincap",
    "purpose/market-data",
    "category/cryptocurrency",
    "purpose/real-time",
  ]
---

# CoinCap MCP Server

#status/active #category/finance #integration/coincap #purpose/market-data #category/cryptocurrency #purpose/real-time

## Description

Real-time cryptocurrency market data integration using CoinCap's public API, providing access to crypto prices and market information without API keys.

## Features

- Real-time price data
- Market information
- No API key required
- Asset listings
- Exchange rates
- Market metrics
- Historical data
- Price tracking
- Volume analysis
- Market updates

## Installation

```bash
npm install @quantgeekdev/coincap-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "coincap": {
      "command": "npx",
      "args": ["@quantgeekdev/coincap-mcp"],
      "env": {
        "UPDATE_INTERVAL": "5",
        "DEFAULT_CURRENCY": "USD",
        "MAX_ASSETS": "100",
        "WEBSOCKET_ENABLED": "true",
        "CACHE_DURATION": "60"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- WebSocket client
- HTTP client
- Cache system
- Data formatter
- Event emitter

## Related Servers

- longmans/coin_api_mcp
- crazyrabbitltc/mcp-coingecko-server
- anjor/coinmarket-mcp-server
