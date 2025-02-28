---
type: server
repo_url: https://github.com/monochromegane/mcp-bigquery-server
name: BigQuery MCP Server
owner: monochromegane
stars: 0
last_updated: 2025-02-09
status: active
official: false
verified: false
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/database", "integration/bigquery", "purpose/data-analysis", "integration/google"]
---

# BigQuery MCP Server

#status/active #category/database #integration/bigquery #purpose/data-analysis #integration/google

## Description

Integrates with BigQuery to enable querying and retrieving table schemas from specified datasets for data analysis and reporting.

## Features

- BigQuery integration
- Table schema retrieval
- Query execution
- Dataset management
- Schema analysis
- Data reporting
- Access control
- Performance monitoring

## Installation

```bash
npm install @monochromegane/mcp-bigquery
```

## Usage

```javascript
{
  "mcpServers": {
    "bigquery": {
      "command": "npx",
      "args": ["@monochromegane/mcp-bigquery"],
      "env": {
        "GOOGLE_CREDENTIALS_FILE": "path/to/credentials.json",
        "PROJECT_ID": "your-project-id",
        "DATASET_ID": "your-dataset",
        "LOCATION": "US"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Google Cloud account
- BigQuery access
- Service account key

## Related Servers

- LucasHild/mcp-server-bigquery
- ergut/mcp-bigquery-server