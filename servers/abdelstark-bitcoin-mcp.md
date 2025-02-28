---
type: server
repo_url: https://github.com/AbdelStark/bitcoin-mcp
name: Bitcoin MCP Server
owner: AbdelStark
stars: 9
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/blockchain",
    "integration/bitcoin",
    "purpose/cryptocurrency",
  ]
---

# Bitcoin MCP Server

#status/active #category/blockchain #integration/bitcoin #purpose/cryptocurrency

## Description

Facilitates interaction with the Bitcoin network via the Model Context Protocol, enabling key generation, address validation, transaction decoding, and blockchain data retrieval.

## Features

- Key generation
- Address validation
- Transaction decoding
- Blockchain data retrieval
- Network interaction
- Wallet management
- Balance checking
- Transaction history

## Installation

```bash
npm install @abdelstark/bitcoin-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "bitcoin": {
      "command": "npx",
      "args": ["@abdelstark/bitcoin-mcp"],
      "env": {
        "BITCOIN_NODE_URL": "http://localhost:8332",
        "BITCOIN_RPC_USER": "your-rpc-user",
        "BITCOIN_RPC_PASSWORD": "your-rpc-password",
        "NETWORK": "mainnet"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Bitcoin Core node
- RPC access
- Network connectivity

## Related Servers

- None currently listed
