---
type: server
repo_url: https://github.com/lenwood/cfbd-mcp-server
name: College Football Data MCP Server
owner: lenwood
stars: 6
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/sports",
    "integration/cfbd",
    "purpose/statistics",
    "purpose/data-analysis",
    "tech/python",
  ]
---

# College Football Data MCP Server

#status/active #category/sports #integration/cfbd #purpose/statistics #purpose/data-analysis

## Description

An MCP server providing access to college football statistics sourced from the College Football Data API within Claude Desktop. This server enables comprehensive analysis and retrieval of college football data and statistics.

## Features

- Team statistics access
- Player performance data
- Game results and schedules
- Historical data retrieval
- Conference standings
- Player rankings
- Team rankings
- Game predictions
- Statistical analysis
- Real-time updates

## Installation

```bash
npm install @lenwood/cfbd-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "cfbd": {
      "command": "npx",
      "args": ["@lenwood/cfbd-mcp-server"],
      "env": {
        "CFBD_API_KEY": "your-api-key",
        "CACHE_DURATION": "3600",
        "MAX_REQUESTS": "100",
        "TIMEZONE": "America/New_York"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- CFBD API key
- Cache system
- Data processing library
- Statistics library

## Related Servers

- seansoreilly-abs
- dmontgomery40-mcp-server-birdstats
