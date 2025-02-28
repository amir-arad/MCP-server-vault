---
type: server
repo_url: https://github.com/chromindscan/chromia-mcp
name: Chromia Wallet MCP Server
owner: chromindscan
stars: 1
last_updated: 2024-12-23
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/blockchain",
    "integration/chromia",
    "purpose/transactions",
    "category/cryptocurrency",
    "tech/wallet",
  ]
---

# Chromia Wallet MCP Server

#status/active #category/blockchain #integration/chromia #purpose/transactions #category/cryptocurrency #tech/wallet

## Description

Enables AI to interact with Chromia Wallet for sending $CHR transactions. This MCP server provides a secure interface for automated cryptocurrency transactions on the Chromia blockchain.

## Features

- Wallet integration
- Transaction signing
- Balance checking
- Address validation
- Transaction history
- Fee estimation
- Network status
- Token transfers
- Security controls
- Error handling

## Installation

```bash
npm install @chromindscan/chromia-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "chromia": {
      "command": "npx",
      "args": ["@chromindscan/chromia-mcp"],
      "env": {
        "CHROMIA_NETWORK": "mainnet",
        "WALLET_PATH": "path/to/wallet.json",
        "MAX_GAS": "1000000",
        "MIN_BALANCE": "1",
        "TIMEOUT": "30000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Chromia Wallet
- Chromia SDK
- Crypto libraries
- Network client
- Security modules

## Related Servers

- abdelstark-bitcoin-mcp
- kydlikebtc-mcp-server-bn
- sammcj-bybit-mcp
