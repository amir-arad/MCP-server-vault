---
type: server
repo_url: https://github.com/ben4mn/amadeus-mcp
name: Amadeus MCP Server
owner: ben4mn
stars: 1
last_updated: 2025-02-16
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/travel", "integration/amadeus", "purpose/flight-search"]
---

# Amadeus MCP Server

#status/active #category/travel #integration/amadeus #purpose/flight-search

## Description

Integrates with Amadeus API to provide flight search capabilities for travel planning and itinerary creation.

## Features

- Flight search functionality
- Travel planning tools
- Itinerary creation
- Real-time pricing
- Availability checking
- Booking management
- Schedule information
- Multi-city routing

## Installation

```bash
npm install @ben4mn/amadeus-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "amadeus": {
      "command": "npx",
      "args": ["@ben4mn/amadeus-mcp"],
      "env": {
        "AMADEUS_CLIENT_ID": "your-client-id",
        "AMADEUS_CLIENT_SECRET": "your-client-secret",
        "AMADEUS_ENV": "test",
        "CACHE_DURATION": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Amadeus API credentials
- Cache storage (optional)

## Related Servers

- None currently listed