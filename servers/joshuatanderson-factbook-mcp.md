---
type: server
repo_url: https://github.com/Joshuatanderson/factbook-mcp
name: Factbook MCP Server
owner: Joshuatanderson
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/data",
    "integration/cia-factbook",
    "purpose/country-information",
    "purpose/data-retrieval",
    "category/reference",
    "tech/javascript",
    "tech/typescript"
  ]
---

# Factbook MCP Server

#status/active #category/data #integration/cia-factbook #purpose/country-information #purpose/data-retrieval #category/reference #tech/javascript #tech/typescript

## Description

Fetches information about a country from the CIA World Factbook, providing access to comprehensive country data and statistics. It allows retrieval of country-specific data and statistics from the CIA World Factbook, offering a structured and easily accessible source of reference information.

## Features

- Country information retrieval
- Statistical data access
- Geographic information
- Demographic data
- Economic statistics
- Political information
- Military data
- Infrastructure details
- Historical data
- Data formatting
- Comprehensive data access
- Structured output
- Easy integration

## Installation

```bash
# Install dependencies
npm install

# Build the project
npm run build
```

## Usage

```javascript
{
  "mcpServers": {
    "factbook": {
      "command": "npx",
      "args": ["@joshuatanderson/factbook-mcp"],
      "env": {
        "CACHE_DIR": "./cache",
        "CACHE_TTL": "86400",
        "OUTPUT_FORMAT": "json",
        "INCLUDE_HISTORY": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Internet connection
- Cache storage
- Data parser
- JSON processor
- TypeScript runtime
- Axios client

## Related Servers

- None currently listed