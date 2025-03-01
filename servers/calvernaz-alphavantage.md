--- 
type: server
repo_url: https://github.com/calvernaz/alphavantage
name: Alphavantage MCP Server
owner: calvernaz
stars: 11
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/finance", "integration/alpha-vantage", "purpose/market-data"]
---

# Alphavantage MCP Server

#status/active #category/finance #integration/alpha-vantage #purpose/market-data

## Description

Integrates with the Alphavantage API to provide access to real-time stock market data and financial information.

## Features

- Real-time stock market data
- Financial information access
- Market data streaming
- Historical data retrieval
- Technical indicators
- Fundamental data
- Currency exchange rates
- Crypto market data

## Installation

```bash
npm install @calvernaz/alphavantage-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "alphavantage": {
      "command": "npx",
      "args": ["@calvernaz/alphavantage-mcp"],
      "env": {
        "ALPHAVANTAGE_API_KEY": "your-api-key",
        "UPDATE_INTERVAL": "60000",
        "DATA_FORMAT": "json",
        "ENABLE_STREAMING": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Alphavantage API key
- WebSocket support (for streaming)

## Related Servers

- berlinbra/alpha-vantage-mcp
- DonMorr/AlphavantageMCPServer