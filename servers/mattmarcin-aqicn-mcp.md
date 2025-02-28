---
type: server
repo_url: https://github.com/mattmarcin/aqicn-mcp
name: AQICN MCP Server
owner: mattmarcin
stars: 0
last_updated: 2025-02-04
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/environmental", "integration/aqicn", "purpose/air-quality"]
---

# AQICN MCP Server

#status/active #category/environmental #integration/aqicn #purpose/air-quality

## Description

Enables interaction with the World Air Quality Index to fetch real-time air quality data for cities and coordinates worldwide via Model Context Protocol (MCP).

## Features

- Real-time air quality data
- City-based queries
- Coordinate-based queries
- Historical data access
- Pollutant breakdown
- Station information
- Data visualization
- Alert thresholds

## Installation

```bash
npm install @mattmarcin/aqicn-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "aqicn": {
      "command": "npx",
      "args": ["@mattmarcin/aqicn-mcp"],
      "env": {
        "AQICN_API_KEY": "your-api-key",
        "DEFAULT_CITY": "beijing",
        "UPDATE_INTERVAL": "900",
        "CACHE_DURATION": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- AQICN API key
- Internet connection
- Cache storage (optional)

## Related Servers

- None currently listed