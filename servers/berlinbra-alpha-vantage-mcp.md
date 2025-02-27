---
type: server
repo_url: https://github.com/berlinbra/alpha-vantage-mcp
name: Alpha Vantage MCP Server
owner: berlinbra
stars: 8
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/finance", "integration/alpha-vantage", "purpose/market-data"]
---

# Alpha Vantage MCP Server

#status/active #category/finance #integration/alpha-vantage #purpose/market-data

## Description

A Model Context Protocol (MCP) server that provides real-time access to financial market data through the free Alpha Vantage API. This server implements a standardized interface for retrieving stock quotes and company information.

## Features

- Real-time market data access
- Stock quote retrieval
- Company information
- Financial data analysis
- Market indicators
- Historical data access
- API standardization
- Data caching

## Installation

```bash
npm install @berlinbra/alpha-vantage-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "alpha-vantage": {
      "command": "npx",
      "args": ["@berlinbra/alpha-vantage-mcp"],
      "env": {
        "ALPHA_VANTAGE_API_KEY": "your-api-key",
        "CACHE_DURATION": "300",
        "MAX_REQUESTS_PER_MINUTE": "5",
        "DEFAULT_MARKET": "US"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Alpha Vantage API key
- Cache storage (optional)

## Related Servers

- calvernaz/alphavantage
- DonMorr/AlphavantageMCPServer