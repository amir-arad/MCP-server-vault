---
type: server
repo_url: https://github.com/wpnbos/buienradar-mcp-server
name: Buienradar MCP Server
owner: wpnbos
stars: 0
last_updated: 2025-02-17
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/weather",
    "integration/buienradar",
    "purpose/weather-forecast",
    "integration/claude",
  ]
---

# Buienradar MCP Server

#status/active #category/weather #integration/buienradar #purpose/weather-forecast #integration/claude

## Description

Fetches precipitation forecasts for any location using Buienradar and integrates with Claude for Desktop to provide accurate two-hour weather predictions.

## Features

- Precipitation forecasts
- Location-based data
- Two-hour predictions
- Claude integration
- Real-time updates
- Location tracking
- Forecast accuracy
- Data visualization

## Installation

```bash
npm install @wpnbos/buienradar-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "buienradar": {
      "command": "npx",
      "args": ["@wpnbos/buienradar-mcp"],
      "env": {
        "DEFAULT_LOCATION": "52.379189,4.899431",
        "UPDATE_INTERVAL": "300",
        "FORECAST_HOURS": "2",
        "LANGUAGE": "en"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Claude Desktop
- Internet connection
- Location services

## Related Servers

- None currently listed
