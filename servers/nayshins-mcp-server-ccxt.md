--- 
type: server
repo_url: https://github.com/Nayshins/mcp-server-ccxt
name: CCXT MCP Server
owner: Nayshins
stars: 13
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/finance",
    "category/cryptocurrency",
    "purpose/market-data",
    "tech/python",
    "integration/ccxt",
  ]
---

# CCXT MCP Server

#status/active #category/finance #category/cryptocurrency #purpose/market-data #tech/python #integration/ccxt

## Description

Provides real-time and historical cryptocurrency market data through integration with major exchanges. This server enables LLMs like Claude to fetch current prices, analyze market trends, and access detailed trading information.

## Features

- Real-time cryptocurrency price data
- Historical market data retrieval
- Multiple exchange support
- Trading pair information
- Order book data
- Market depth analysis
- Trading volume statistics
- Price chart data
- Exchange rate conversion
- Market trend indicators

## Installation

```bash
npm install @nayshins/mcp-server-ccxt
```

## Usage

```javascript
{
  "mcpServers": {
    "ccxt": {
      "command": "npx",
      "args": ["@nayshins/mcp-server-ccxt"],
      "env": {
        "EXCHANGE_ID": "binance",
        "API_KEY": "your-exchange-api-key",
        "API_SECRET": "your-exchange-api-secret",
        "TIMEOUT": "30000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- CCXT library
- Exchange API credentials
- WebSocket support (optional)
- Market data feed subscription

## Related Servers

- kydlikebtc/mcp-server-bn
- sammcj-bybit-mcp
- qeinfinity-binance-mcp-server