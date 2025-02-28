---
type: server
repo_url: https://github.com/raju-deriv/mcp-deriv-api-server
name: Deriv API MCP Server
owner: raju-deriv
stars: 0
last_updated: 2025-01-07
status: active
official: false
verified: false
sources: ["inbox/batch_009.md"]
tags:
  [
    "status/active",
    "category/finance",
    "integration/deriv",
    "purpose/trading",
    "purpose/market-analysis",
    "tech/api",
  ]
---

# Deriv API MCP Server

#status/active #category/finance #integration/deriv #purpose/trading #purpose/market-analysis #tech/api

## Description

Integrates with Deriv API to enable trading operations like retrieving symbols and balances for automated trading systems and market analysis tools.

## Features

- Symbol retrieval
- Balance checking
- Trading operations
- Market analysis
- Account management
- Order handling
- Position tracking
- Price monitoring
- Portfolio management
- Risk assessment

## Installation

```bash
npm install @raju-deriv/deriv-api-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "deriv-api": {
      "command": "npx",
      "args": ["@raju-deriv/deriv-api-mcp"],
      "env": {
        "DERIV_API_TOKEN": "your-api-token",
        "ACCOUNT_ID": "your-account-id",
        "UPDATE_INTERVAL": "1000",
        "MAX_POSITIONS": "10",
        "RISK_LIMIT": "0.02"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Deriv API access
- WebSocket client
- Market data handler
- Order manager
- Risk calculator

## Related Servers

- qeinfinity-binance-mcp-server
- kydlikebtc-mcp-server-bn
- itay1542-brokers-mcp
