---
type: server
repo_url: https://github.com/raw391/coin_daemon_mcp
name: Cryptocurrency Daemon MCP Server
owner: raw391
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/cryptocurrency",
    "purpose/daemon-management",
    "purpose/wallet-operations",
    "tech/rpc",
    "category/blockchain",
    "tech/typescript",
  ]
---

# Cryptocurrency Daemon MCP Server

#status/active #category/cryptocurrency #purpose/daemon-management #purpose/wallet-operations #tech/rpc #category/blockchain

## Description

Enables secure interactions with cryptocurrency daemon RPC interfaces through AI assistants, supporting transaction management, wallet operations, and daemon monitoring for Bitcoin-derived cryptocurrencies.

## Features

- Daemon RPC interface
- Transaction management
- Wallet operations
- Daemon monitoring
- Security controls
- Balance checking
- Address validation
- Block exploration
- Network status
- Transaction history

## Installation

```bash
npm install @raw391/coin-daemon-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "coin-daemon": {
      "command": "npx",
      "args": ["@raw391/coin-daemon-mcp"],
      "env": {
        "RPC_HOST": "localhost",
        "RPC_PORT": "8332",
        "RPC_USER": "your-rpc-user",
        "RPC_PASSWORD": "your-rpc-password",
        "NETWORK": "mainnet"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Cryptocurrency daemon
- RPC client
- Security modules
- Transaction parser
- Network monitor

## Related Servers

- longmans/coin_api_mcp
- quantgeekdev/coincap-mcp
- crazyrabbitltc/mcp-coingecko-server
