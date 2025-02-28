---
type: server
repo_url: https://github.com/DMontgomery40/mcp-server-birdstats
name: BirdStats MCP Server
owner: DMontgomery40
stars: 1
last_updated: 2024-12-13
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/data-analysis",
    "integration/birdnet",
    "integration/ebird",
    "purpose/wildlife-monitoring",
  ]
---

# BirdStats MCP Server

#status/active #category/data-analysis #integration/birdnet #integration/ebird #purpose/wildlife-monitoring

## Description

Cross-reference your BirdNET-Pi data with eBird observations using natural language.

## Features

- BirdNET-Pi integration
- eBird data access
- Cross-referencing
- Natural language queries
- Bird observation analysis
- Data visualization
- Species tracking
- Location mapping

## Installation

```bash
npm install @dmontgomery40/mcp-server-birdstats
```

## Usage

```javascript
{
  "mcpServers": {
    "birdstats": {
      "command": "npx",
      "args": ["@dmontgomery40/mcp-server-birdstats"],
      "env": {
        "BIRDNET_PI_URL": "http://your-birdnet-pi:8080",
        "EBIRD_API_KEY": "your-ebird-key",
        "DEFAULT_LOCATION": "US-NY-109",
        "DATA_RETENTION": "30"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- BirdNET-Pi setup
- eBird API access
- Database storage

## Related Servers

- None currently listed
