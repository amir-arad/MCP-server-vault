---
type: server
repo_url: https://github.com/5ajaki/mcp-etherscan-server
name: Etherscan MCP Server
owner: 5ajaki
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/blockchain",
    "integration/etherscan",
    "purpose/blockchain-data",
    "purpose/transaction-tracking",
    "tech/ethereum",
  ]
---

# Etherscan MCP Server

#status/active #category/blockchain #integration/etherscan #purpose/blockchain-data #purpose/transaction-tracking #tech/ethereum

## Description

Integrates with Etherscan's API to provide Ethereum blockchain data tools for balance checking, transaction tracking, and smart contract interactions.

## Features

- Balance checking
- Transaction tracking
- Smart contract interaction
- ABI retrieval
- Token transfers
- Gas price monitoring
- Block exploration
- Address analytics
- Contract verification
- Event logs access

## Installation

```bash
npm install @5ajaki/mcp-etherscan-server
```

## Usage

```javascript
{
  "mcpServers": {
    "etherscan": {
      "command": "npx",
      "args": ["@5ajaki/mcp-etherscan-server"],
      "env": {
        "ETHERSCAN_API_KEY": "your-api-key",
        "NETWORK": "mainnet",
        "CACHE_DURATION": "300",
        "RATE_LIMIT": "5"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Etherscan API key
- Network connectivity
- Cache storage
- Rate limiting system

## Related Servers

- [Etherscan Server](https://github.com/crazyrabbitLTC/mcp-etherscan-server) - Alternative Etherscan implementation
