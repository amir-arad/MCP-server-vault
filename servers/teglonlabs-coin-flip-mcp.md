---
type: server
repo_url: https://github.com/TeglonLabs/coin-flip-mcp
name: Coin Flip MCP Server
owner: TeglonLabs
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/utility",
    "integration/random-org",
    "purpose/randomization",
    "tech/api",
    "purpose/demonstration",
  ]
---

# Coin Flip MCP Server

#status/active #category/utility #integration/random-org #purpose/randomization #tech/api #purpose/demonstration

## Description

Enables interaction with a tool for generating true random coin flips via random.org's API, supporting multiple custom side configurations and illustrating the Model Context Protocol.

## Features

- True random generation
- Custom side configuration
- API integration
- Result verification
- Statistics tracking
- Multiple flip support
- Custom probability
- History logging
- Quota management
- Error handling

## Installation

```bash
npm install @teglonlabs/coin-flip-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "coin-flip": {
      "command": "npx",
      "args": ["@teglonlabs/coin-flip-mcp"],
      "env": {
        "RANDOM_ORG_KEY": "your-api-key",
        "DEFAULT_SIDES": "heads,tails",
        "BATCH_SIZE": "100",
        "LOG_RESULTS": "true",
        "VERIFY_RANDOMNESS": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Random.org API key
- Result validator
- Statistics tracker
- History logger
- Quota monitor

## Related Servers

- modelcontextprotocol-random-server
- modelcontextprotocol-utility-server
- modelcontextprotocol-demo-server
