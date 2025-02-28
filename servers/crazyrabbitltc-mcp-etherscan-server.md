---
type: server
repo_url: https://github.com/crazyrabbitLTC/mcp-etherscan-server
name: Etherscan MCP Server
owner: crazyrabbitLTC
stars: 6
last_updated: 2025-02-03
status: active
official: false
verified: false
sources: ["inbox/batch_011.md"]
tags: ["status/active", "category/blockchain", "integration/etherscan", "purpose/blockchain-data", "tech/ethereum", "purpose/real-time-data"]
---

# Etherscan MCP Server

#status/active #category/blockchain #integration/etherscan #purpose/blockchain-data #tech/ethereum #purpose/real-time-data

## Description

Facilitates interaction with Ethereum blockchain data via Etherscan's API, providing real-time access to balances, transactions, token transfers, contract ABIs, gas prices, and ENS name resolutions.

## Features

- Real-time blockchain data
- Balance monitoring
- Transaction tracking
- Token transfer tracking
- Contract ABI access
- Gas price monitoring
- ENS resolution
- Event log access
- Address analytics
- Multi-network support

## Installation

```bash
npm install @crazyrabbitltc/mcp-etherscan-server
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

- Node.js >= 14
- Etherscan API key
- Network connectivity
- Cache storage
- Rate limiting system

## Related Servers

- [Etherscan Server](https://github.com/5ajaki/mcp-etherscan-server) - Alternative Etherscan implementation