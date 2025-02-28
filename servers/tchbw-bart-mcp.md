---
type: server
repo_url: https://github.com/tchbw/bart-mcp
name: BART MCP Server
owner: tchbw
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/transportation", "integration/bart", "purpose/transit-info", "tech/typescript"]
---

# BART MCP Server

#status/active #category/transportation #integration/bart #purpose/transit-info #tech/typescript

## Description

A Model Context Protocol server that integrates with BART's API to provide real-time train departure information in San Francisco. The server allows Claude to access up-to-date BART transit data for improved trip planning and transit information retrieval.

## Features

- Real-time departures for all BART stations
- Station information retrieval
- Platform and train details
- Departure time estimates
- Train direction information
- Train length reporting
- Delay notifications
- Color-coded line identification

## Installation

```bash
# Clone the repository
git clone https://github.com/tchbw/bart-mcp.git
cd bart-mcp

# Install dependencies
npm install

# Build the server
npm run build
```

## Usage

```javascript
{
  "mcpServers": {
    "bart": {
      "command": "npx",
      "args": ["@tchbw/bart-mcp"],
      "env": {
        "BART_API_KEY": "your-api-key",
        "DEFAULT_STATION": "SFIA",
        "UPDATE_INTERVAL": "60",
        "MAX_DEPARTURES": "10"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- TypeScript
- @modelcontextprotocol/sdk
- BART API key
- Internet connection

## Related Servers

- None currently listed