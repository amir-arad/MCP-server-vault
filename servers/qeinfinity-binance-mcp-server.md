---
type: server
repo_url: https://github.com/qeinfinity/binance-mcp-server
name: Binance MCP Server
owner: qeinfinity
stars: 1
last_updated: 2025-01-08
status: active
official: false
verified: false
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/finance", "integration/binance", "purpose/trading", "purpose/market-data"]
---

# Binance MCP Server

#status/active #category/finance #integration/binance #purpose/trading #purpose/market-data

## Description

Integrates with Binance to provide real-time cryptocurrency market data streaming for spot and futures markets, enabling automated trading strategies and financial analysis.

## Features

- Real-time market data
- Spot market support
- Futures market support
- Trading automation
- Financial analysis
- Data streaming
- Strategy execution
- Portfolio tracking

## Installation

```bash
npm install @qeinfinity/binance-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "binance": {
      "command": "npx",
      "args": ["@qeinfinity/binance-mcp"],
      "env": {
        "BINANCE_API_KEY": "your-api-key",
        "BINANCE_SECRET_KEY": "your-secret-key",
        "DEFAULT_MARKET": "spot",
        "STREAM_BUFFER_SIZE": "1000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Binance account
- API credentials
- WebSocket support

## Related Servers

- None currently listed