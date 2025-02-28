---
type: server
repo_url: https://github.com/seanivore/bing-searches-mcp
name: Bing Searches MCP Server
owner: seanivore
stars: 2
last_updated: 2025-02-12
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags: ["status/active", "category/search", "integration/bing", "purpose/data-analysis"]
---

# Bing Searches MCP Server

#status/active #category/search #integration/bing #purpose/data-analysis

## Description

Integrates with Bing Search API to collect, parse, and analyze search data.

## Features

- Bing API integration
- Search data collection
- Data parsing
- Result analysis
- Query optimization
- Data aggregation
- Search analytics
- Result filtering

## Installation

```bash
npm install @seanivore/bing-searches-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "bing-searches": {
      "command": "npx",
      "args": ["@seanivore/bing-searches-mcp"],
      "env": {
        "BING_API_KEY": "your-api-key",
        "MAX_RESULTS": "50",
        "MARKET": "en-US",
        "SAFE_SEARCH": "moderate"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Bing API subscription
- API credentials
- Data storage

## Related Servers

- None currently listed