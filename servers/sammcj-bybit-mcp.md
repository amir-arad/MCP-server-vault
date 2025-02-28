---
type: server
repo_url: https://github.com/sammcj/bybit-mcp
name: Bybit MCP Server
owner: sammcj
stars: 5
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/finance",
    "integration/bybit",
    "purpose/market-data",
    "category/cryptocurrency",
    "tech/nodejs",
  ]
---

# Bybit MCP Server

#status/active #category/finance #integration/bybit #purpose/market-data #category/cryptocurrency

## Description

Provides read-only access to Bybit's cryptocurrency exchange API for retrieving real-time market data, order book information, and account details.

## Features

- Real-time market data
- Order book access
- Account information
- Read-only operations
- Market monitoring
- Price tracking
- Volume analysis
- Trading pairs support

## Installation

```bash
npm install @sammcj/bybit-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "bybit": {
      "command": "npx",
      "args": ["@sammcj/bybit-mcp"],
      "env": {
        "BYBIT_API_KEY": "your-api-key",
        "BYBIT_API_SECRET": "your-api-secret",
        "DEFAULT_PAIRS": "BTCUSD,ETHUSD",
        "UPDATE_INTERVAL": "1000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Bybit account
- API credentials
- WebSocket support

## Related Servers

- None currently listed
