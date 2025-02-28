---
type: server
repo_url: https://github.com/kydlikebtc/mcp-server-bn
name: Binance Spot Trading MCP Server
owner: kydlikebtc
stars: 2
last_updated: 2025-02-08
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/finance",
    "integration/binance",
    "purpose/trading",
    "category/cryptocurrency",
  ]
---

# Binance Spot Trading MCP Server

#status/active #category/finance #integration/binance #purpose/trading #category/cryptocurrency

## Description

This server provides a robust interface for Binance spot trading operations, including secure management of API credentials, execution and management of spot orders, and monitoring of account balances and open orders.

## Features

- Spot trading operations
- API credential management
- Order execution
- Balance monitoring
- Order tracking
- Account management
- Market data access
- Security handling

## Installation

```bash
npm install @kydlikebtc/mcp-server-bn
```

## Usage

```javascript
{
  "mcpServers": {
    "binance-spot": {
      "command": "npx",
      "args": ["@kydlikebtc/mcp-server-bn"],
      "env": {
        "BINANCE_API_KEY": "your-api-key",
        "BINANCE_SECRET_KEY": "your-secret-key",
        "TRADE_PAIRS": "BTC/USDT,ETH/USDT",
        "ORDER_TIMEOUT": "30"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Binance account
- API credentials
- Trading permissions

## Related Servers

- qeinfinity/binance-mcp-server
