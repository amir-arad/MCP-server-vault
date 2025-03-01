---
type: server
repo_url: https://github.com/crazyrabbitLTC/mcp-etherscan-server
name: Etherscan MCP Server
owner: crazyrabbitLTC
stars: 8
last_updated: 2025-03-01
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
    "tech/ethereum",
    "purpose/real-time-data",
  ]
---

# Etherscan MCP Server

#status/active #category/blockchain #integration/etherscan #purpose/blockchain-data #tech/ethereum #purpose/real-time-data

## Description

Facilitates interaction with Ethereum blockchain data via Etherscan's API, providing real-time access to balances, transactions, token transfers, contract ABIs, gas prices, and ENS name resolutions.

## Features

- Balance Checking: Get ETH balance for any Ethereum address
- Transaction History: View recent transactions with detailed information
- Token Transfers: Track ERC20 token transfers with token details
- Contract ABI: Fetch smart contract ABIs for development
- Gas Prices: Monitor current gas prices (Safe Low, Standard, Fast)
- ENS Resolution: Resolve Ethereum addresses to ENS names

## Installation

```bash
npm install
```

## Usage

```javascript
{
  "mcpServers": {
    "etherscan": {
      "command": "npx",
      "args": ["@crazyrabbitltc/mcp-etherscan-server"],
      "env": {
        "ETHERSCAN_API_KEY": "your-api-key",
        "DEFAULT_NETWORK": "mainnet",
        "RATE_LIMIT": "5",
        "CACHE_TTL": "300"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 18
- Etherscan API key

## Related Servers

- [Etherscan Server](https://github.com/5ajaki/mcp-etherscan-server) - Alternative Etherscan implementation
