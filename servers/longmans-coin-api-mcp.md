---
type: server
repo_url: https://github.com/longmans/coin_api_mcp
name: CoinMarketCap API MCP Server
owner: longmans
stars: 6
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/finance",
    "integration/coinmarketcap",
    "purpose/market-data",
    "category/cryptocurrency",
    "purpose/analytics",
  ]
---

# CoinMarketCap API MCP Server

#status/active #category/finance #integration/coinmarketcap #purpose/market-data #category/cryptocurrency #purpose/analytics

## Description

Integrates with CoinMarketCap's API to fetch and analyze cryptocurrency market data, supporting customizable queries for real-time information.

## Features

- Market data retrieval
- Price tracking
- Custom queries
- Real-time updates
- Market analytics
- Historical data
- Currency conversion
- Portfolio tracking
- Market metrics
- Data visualization

### Available Tools

- `listing-coins` - Fetches a paginated list of all active cryptocurrencies with the latest market data.

  - `start` (integer, optional): Offset the start (1-based index) of the paginated list of items to return.
  - `limit` (integer, optional): Number of results to return (default: 10, max: 5000).
  - `price_min` (number, optional): Minimum USD price to filter results.
  - `price_max` (number, optional): Maximum USD price to filter results.
  - `market_cap_min` (number, optional): Minimum market cap to filter results.
  - `market_cap_max` (number, optional): Maximum market cap to filter results.
  - `convert` (string, optional): Calculate market quotes in multiple currencies.
  - `sort` (string, optional): Field to sort the list of cryptocurrencies by.
  - `sort_dir` (string, optional): Direction to order cryptocurrencies (asc or desc).

- `get-coin-info` - Retrieves detailed information about a specific cryptocurrency.

  - `id` (string, optional): One or more comma-separated CoinMarketCap cryptocurrency IDs.
  - `slug` (string, optional): A comma-separated list of cryptocurrency slugs.
  - `symbol` (string, optional): One or more comma-separated cryptocurrency symbols.

- `get-coin-quotes` - Fetches the latest market quotes for one or more cryptocurrencies.

  - `id` (string, optional): One or more comma-separated cryptocurrency CoinMarketCap IDs.
  - `slug` (string, optional): A comma-separated list of cryptocurrency slugs.
  - `symbol` (string, optional): One or more comma-separated cryptocurrency symbols.

## Installation

To install Cryptocurrency Data for Claude Desktop automatically via [Smithery](https://smithery.ai/server/coin-api-mcp):

```bash
npx -y @smithery/cli install coin-api-mcp --client claude
```

### Build the Server

Clone this repository and build and install the program with your default Python interpreter (recommended).

```bash
git clone https://github.com/longmans/coin_api_mcp.git
cd coin_api_mcp
uv build
uv pip install .
```

After installation, you can run it as a script using:

```bash
python -m coin_api_mcp
```

## Usage

### API Key

The server requires a CoinMarketCap API key to function. You can obtain one from [CoinMarketCap's website](https://coinmarketcap.com/api/). The API key can be provided in two ways:

1.  As an environment variable:

```bash
export COINMARKETCAP_API_KEY=your_api_key_here
```

2.  As a command-line argument:

```bash
python -m coin_api_mcp --api-key=your_api_key_here
```

### Configure for Claude.app

Add to your Claude settings:

Using pip installation

```json
"mcpServers": {
  "coin_api": {
    "command": "python",
    "args": ["-m", "coin_api_mcp"]
  },
  "env": {
        "COINMARKETCAP_API_KEY": "your_api_key_here"
  }
}
```

If you see any issue, you may want to use the full path for the Python interpreter you are using. You can do a `which python` to find out the exact path if needed.

Remember to set the COINMARKETCAP_API_KEY environment variable or provide it via the --api-key argument.

## Debugging

You can use the MCP inspector to debug the server

## Dependencies

- Node.js >= 16
- CoinMarketCap API key
- Cache system
- Data processor
- HTTP client
- Analytics engine
