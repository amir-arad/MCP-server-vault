---
type: server
repo_url: https://github.com/itay1542/brokers-mcp
name: Brokers MCP Server
owner: itay1542
stars: 54
last_updated: 2025-02-08
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/finance",
    "integration/interactive-brokers",
    "integration/tradestation",
    "purpose/trading",
  ]
---

# Brokers MCP Server

#status/active #category/finance #integration/interactive-brokers #integration/tradestation #purpose/trading

## Description

Integrates with brokers like Interactive Brokers and TradeStation to provide real-time market data, order execution, and portfolio analysis for quantitative trading and financial analysis.

## Features

- Real-time market data
- Order execution
- Portfolio analysis
- Quantitative trading
- Financial analysis
- Multi-broker support
- Risk management
- Performance tracking

## Installation

```bash
npm install @itay1542/brokers-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "brokers": {
      "command": "npx",
      "args": ["@itay1542/brokers-mcp"],
      "env": {
        "IB_ACCOUNT": "your-ib-account",
        "IB_PORT": "7496",
        "TS_CLIENT_ID": "your-ts-client-id",
        "TS_CLIENT_SECRET": "your-ts-client-secret"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Broker accounts
- API credentials
- TWS or IB Gateway

## Related Servers

- None currently listed
