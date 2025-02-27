---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/src/google-maps
name: Google Maps
owner: modelcontextprotocol
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags:
  [
    "category/location",
    "status/official",
    "purpose/development",
    "tech/typescript",
    "integration/google",
  ]
---

#category/location #status/official #purpose/development #tech/typescript #integration/google

# Google Maps

## Description

A reference MCP server that provides location services, directions, and place details through Google Maps Platform integration. This server enables comprehensive access to mapping and location-based services.

## Features

- Geocoding and reverse geocoding
- Place search and details
- Route calculation and directions
- Distance matrix computation
- Map styling and customization
- Real-time traffic information
- Street View imagery access

## Installation

```bash
npm install @modelcontextprotocol/google-maps-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { GoogleMapsServer } from "@modelcontextprotocol/google-maps-server";

const server = new GoogleMapsServer({
  apiKey: process.env.GOOGLE_MAPS_API_KEY,
});
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- @googlemaps/google-maps-services-js
- TypeScript

## Related Servers

- Google Drive Server - For Google platform integration
- Memory Server - For caching location data
