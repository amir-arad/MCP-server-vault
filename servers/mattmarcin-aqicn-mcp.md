---
type: server
repo_url: https://github.com/mattmarcin/aqicn-mcp
name: AQICN MCP Server
owner: mattmarcin
stars: 6
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags:
  [
    "status/active",
    "category/environmental",
    "integration/aqicn",
    "purpose/air-quality",
  ]
---

# AQICN MCP Server

#status/active #category/environmental #integration/aqicn #purpose/air-quality

## Description

Enables interaction with the World Air Quality Index to fetch real-time air quality data for cities and coordinates worldwide via Model Context Protocol (MCP).

## Features

- Real-time air quality data
- City-based queries
- Coordinate-based queries
- Pollutant breakdown
- Station information

### Available Tools

- `city_aqi` - Get air quality data for a specific city.

  - Input:
    - `city`: Name of the city to get air quality data for
  - Output: `AQIData` with:
    - `aqi`: Air Quality Index value
    - `station`: Station name
    - `dominant_pollutant`: Main pollutant (if available)
    - `time`: Timestamp of the measurement
    - `coordinates`: Latitude and longitude of the station

- `geo_aqi` - Get air quality data for a specific location using coordinates.

  - Input:
    - `latitude`: Latitude of the location
    - `longitude`: Longitude of the location
  - Output: Same as `city_aqi`

- `search_station` - Search for air quality monitoring stations by keyword.

  - Input:
    - `keyword`: Keyword to search for stations (city name, station name, etc.)
  - Output: List of `StationInfo` with:
    - `name`: Station name
    - `station_id`: Unique station identifier
    - `coordinates`: Latitude and longitude of the station

## Installation

### Installing via Smithery

To install AQICN MCP Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@mattmarcin/aqicn-mcp):

```bash
npx -y @smithery/cli install @mattmarcin/aqicn-mcp --client claude
```

### Installing via recommended uv (manual)

We recommend using [uv](https://docs.astral.sh/uv/) to manage your Python environment:

```bash
# Install the package and dependencies
uv pip install -e .
```

## Usage

Create a `.env` file in the project root (you can copy from `.env.example`):

```
# .env
AQICN_API_KEY=your_api_key_here
```

Alternatively, you can set the environment variable directly:

```bash
# Linux/macOS
export AQICN_API_KEY=your_api_key_here

# Windows
set AQICN_API_KEY=your_api_key_here
```

## Running the Server

### Development Mode

The fastest way to test and debug your server is with the MCP Inspector:

```bash
mcp dev aqicn_server.py
```

### Claude Desktop Integration

Once your server is ready, install it in Claude Desktop:

```bash
mcp install aqicn_server.py
```

### Direct Execution

For testing or custom deployments:

```bash
python aqicn_server.py
```

## Dependencies

- Node.js >= 14
- AQICN API key
- Internet connection
- Cache storage (optional)
