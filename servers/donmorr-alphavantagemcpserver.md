--- 
type: server
repo_url: https://github.com/DonMorr/AlphavantageMCPServer
name: Alphavantage MCP Server
owner: DonMorr
stars: 0
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/active",
    "category/finance",
    "integration/alpha-vantage",
    "purpose/market-data",
    "tech/python",
  ]
---

# Alphavantage MCP Server

#status/active #category/finance #integration/alpha-vantage #purpose/market-data

## Description

Integrates with Alphavantage API to provide real-time and historical financial data for stock market analysis and trading strategies.

## Features

- Real-time financial data
- Historical data access
- Stock market analysis
- Trading strategy support
- Technical indicators
- Market data aggregation
- Custom data formatting
- API rate limiting

## Installation

```bash
npm install @donmorr/alphavantage-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "alphavantage": {
      "command": "npx",
      "args": ["@donmorr/alphavantage-mcp"],
      "env": {
        "ALPHAVANTAGE_API_KEY": "your-api-key",
        "RATE_LIMIT": "5",
        "CACHE_TTL": "300",
        "DATA_PRECISION": "4"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Alphavantage API key
- Redis (optional, for caching)