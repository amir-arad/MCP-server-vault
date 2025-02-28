---
type: server
repo_url: https://github.com/crazyrabbitLTC/mcp-coingecko-server
name: CoinGecko Pro MCP Server
owner: crazyrabbitLTC
stars: 5
last_updated: 2025-02-13
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
[
"status/active",
"category/finance",
"integration/coingecko",
"purpose/market-data",
"category/cryptocurrency",
"tech/openai",
]

---

# CoinGecko Pro MCP Server

#status/active #category/finance #integration/coingecko #purpose/market-data #category/cryptocurrency #tech/openai

## Description

Enables interaction with the CoinGecko Pro API to access cryptocurrency data including price history and market metrics through both MCP and OpenAI function calling.

## Features

- Price history access
- Market metrics
- OpenAI integration
- Function calling
- Data aggregation
- Historical analysis
- Market indicators
- Token information
- Exchange data
- Trend analysis

## Installation

```bash
npm install @crazyrabbitltc/mcp-coingecko
```

## Usage

```javascript
{
  "mcpServers": {
    "coingecko": {
      "command": "npx",
      "args": ["@crazyrabbitltc/mcp-coingecko"],
      "env": {
        "COINGECKO_PRO_KEY": "your-api-key",
        "OPENAI_API_KEY": "your-openai-key",
        "UPDATE_INTERVAL": "300",
        "MAX_HISTORY": "365",
        "CACHE_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- CoinGecko Pro API key
- OpenAI API key
- Data processor
- Cache system
- Analytics engine

## Related Servers

- quantgeekdev/coincap-mcp
- longmans/coin_api_mcp
- anjor/coinmarket-mcp-server
