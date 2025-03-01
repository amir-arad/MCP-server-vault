---
type: server
repo_url: https://github.com/flexpa/mcp-fhir
name: FHIR MCP Server
owner: flexpa
stars: 17
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_012.md"]
tags:
  [
    "status/active",
    "category/healthcare",
    "integration/fhir",
    "purpose/data-access",
    "purpose/search",
    "purpose/analysis",
    "tech/typescript",
  ]
---

# FHIR MCP Server

#status/active #category/healthcare #integration/fhir #purpose/data-access #purpose/search #purpose/analysis

## Description

Integrates FHIR data into workflows, enabling seamless access and search of healthcare resources for dynamic querying and analysis.

## Features

- FHIR data integration
- Healthcare resource access
- Resource searching
- Dynamic querying
- Data analysis
- FHIR compliance
- Resource validation
- Security controls
- Query optimization
- Response formatting

## Installation

```bash
npm install @flexpa/mcp-fhir
```

## Usage

```javascript
{
  "mcpServers": {
    "fhir": {
      "command": "npx",
      "args": ["@flexpa/mcp-fhir"],
      "env": {
        "FHIR_BASE_URL": "https://api.example.com/fhir",
        "AUTH_TOKEN": "your-auth-token",
        "MAX_RESULTS": "100",
        "CACHE_TTL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- FHIR client library
- Authentication system
- Cache system
- Network connectivity

## Related Servers

- None currently listed
