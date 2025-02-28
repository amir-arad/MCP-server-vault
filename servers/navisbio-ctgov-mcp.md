---
type: server
repo_url: https://github.com/navisbio/ctgov_MCP
name: Clinical Trials Database MCP Server
owner: navisbio
stars: 3
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/healthcare",
    "integration/aact",
    "purpose/clinical-trials",
    "purpose/research",
    "category/database",
  ]
---

# Clinical Trials Database MCP Server

#status/active #category/healthcare #integration/aact #purpose/clinical-trials #purpose/research #category/database

## Description

Integrates with the AACT clinical trials database, enabling querying and analysis of large-scale trial data for research and healthcare applications.

## Features

- Trial data querying
- Analysis capabilities
- Research support
- Data extraction
- Query optimization
- Result filtering
- Statistical analysis
- Data visualization
- Export functionality
- Search capabilities

## Installation

```bash
npm install @navisbio/ctgov-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "clinical-trials": {
      "command": "npx",
      "args": ["@navisbio/ctgov-mcp"],
      "env": {
        "AACT_HOST": "aact-db.ctti-clinicaltrials.org",
        "AACT_DATABASE": "aact",
        "AACT_USERNAME": "your-username",
        "AACT_PASSWORD": "your-password",
        "CACHE_TTL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- AACT database access
- PostgreSQL client
- Query builder
- Data analyzer
- Export handler

## Related Servers

- modelcontextprotocol-healthcare-server
- kartha-ai-agentcare-mcp
- modelcontextprotocol-research-server
