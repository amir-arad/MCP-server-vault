--- 
type: server
repo_url: https://github.com/baba786/angleone-mcp-server
name: AngleOne MCP Server
owner: baba786
stars: 0
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/finance", "integration/angleone", "purpose/trading"]
---

# AngleOne MCP Server

#status/active #category/finance #integration/angleone #purpose/trading

## Description

Integrates AngelOne India trading platform to provide real-time market data access, order management, and portfolio tracking for automated financial analysis and trading operations.

## Features

- Real-time market data
- Order management
- Portfolio tracking
- Financial analysis
- Trading operations
- Market monitoring
- Position management
- Risk assessment

## Installation

```bash
npm install @baba786/angleone-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "angleone": {
      "command": "npx",
      "args": ["@baba786/angleone-mcp"],
      "env": {
        "ANGLEONE_API_KEY": "your-api-key",
        "ANGLEONE_CLIENT_ID": "your-client-id",
        "ANGLEONE_PASSWORD": "your-password",
        "MARKET_TYPE": "CASH"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- AngelOne trading account
- API credentials
- Market data subscription

## Related Servers

- None currently listed