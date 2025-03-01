---
type: server
repo_url: https://github.com/crazyrabbitLTC/mcp-ethers-server
name: Ethers MCP Server
owner: crazyrabbitLTC
stars: 1
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/blockchain",
    "integration/ethereum",
    "tech/ethers-js",
    "purpose/wallet-operations",
    "purpose/smart-contracts",
  ]
---

# Ethers MCP Server

#status/active #category/blockchain #integration/ethereum #tech/ethers-js #purpose/wallet-operations #purpose/smart-contracts

## Description

Integrates with Ethereum networks and smart contracts using ethers.js to enable wallet operations, transaction management, and blockchain interactions.

## Features

- Wallet operations
- Transaction management
- Smart contract interaction
- Network integration
- Balance checking
- Gas estimation
- Event listening
- Contract deployment
- ABI handling
- Transaction signing

## Installation

```bash
npm install @crazyrabbitltc/mcp-ethers-server
```

## Usage

```javascript
{
  "mcpServers": {
    "ethers": {
      "command": "npx",
      "args": ["@crazyrabbitltc/mcp-ethers-server"],
      "env": {
        "ETHEREUM_NETWORK": "mainnet",
        "PROVIDER_URL": "your-provider-url",
        "PRIVATE_KEY": "your-private-key",
        "GAS_LIMIT": "2000000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- ethers.js
- Ethereum network access
- Web3 provider
- Network connectivity

## Related Servers

- None currently listed
