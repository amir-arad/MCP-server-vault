---
type: server
repo_url: https://github.com/NewbieNL/enhanced-google-maps-mcp
name: Enhanced Google Maps MCP Server
owner: NewbieNL
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/maps",
    "integration/google-maps",
    "purpose/geocoding",
    "purpose/routing",
    "purpose/place-search",
  ]
---

# Enhanced Google Maps MCP Server

#status/active #category/maps #integration/google-maps #purpose/geocoding #purpose/routing #purpose/place-search

## Description

Integrates with Google Maps API to provide geocoding, place search, and routing capabilities for location-based applications and services.

## Features

- Geocoding services
- Place search
- Route calculation
- Distance matrix
- Place details
- Address validation
- Location autocomplete
- Map visualization
- Traffic data
- Transit information

## Installation

```bash
npm install @newbienl/enhanced-google-maps-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "google-maps": {
      "command": "npx",
      "args": ["@newbienl/enhanced-google-maps-mcp"],
      "env": {
        "GOOGLE_MAPS_API_KEY": "your-api-key",
        "DEFAULT_REGION": "US",
        "LANGUAGE": "en",
        "CACHE_DURATION": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Google Maps API key
- Google Cloud account
- Geocoding API access
- Places API access

## Related Servers

- None currently listed
