---
type: server
repo_url: https://github.com/AdamikHQ/adamik-mcp-server
name: Adamik MCP Server
owner: AdamikHQ
stars: 0
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/blockchain", "integration/starknet", "purpose/blockchain-operations"]
---

# Adamik MCP Server

#status/active #category/blockchain #integration/starknet #purpose/blockchain-operations

## Description

Integrates with the Adamik API to enable blockchain operations and custom AI functionalities via Starknet, supporting secure API key management and efficient request handling.

## Features

- Starknet blockchain integration
- Secure API key management
- Efficient request handling
- Custom AI functionalities
- Blockchain operations support

## Installation

```bash
npm install @adamikhq/mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "adamik": {
      "command": "npx",
      "args": ["@adamikhq/mcp-server"],
      "env": {
        "ADAMIK_API_KEY": "your-api-key",
        "STARKNET_NETWORK": "mainnet",
        "REQUEST_TIMEOUT": "30000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Adamik API key
- Starknet provider

## Related Servers

- None currently listed