---
type: server
repo_url: https://github.com/LucasHild/mcp-server-bigquery
name: BigQuery MCP Server
owner: LucasHild
stars: 12
last_updated: 2025-02-16
status: active
official: false
verified: false
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/database", "integration/bigquery", "purpose/data-analysis", "integration/google"]
---

# BigQuery MCP Server

#status/active #category/database #integration/bigquery #purpose/data-analysis #integration/google

## Description

A Model Context Protocol server that provides access to BigQuery. This server enables LLMs to inspect database schemas and execute queries.

## Features

- BigQuery integration
- Schema inspection
- Query execution
- Data analysis
- Performance optimization
- Cost management
- Access control
- Result formatting

## Installation

```bash
npm install @lucashild/mcp-server-bigquery
```

## Usage

```javascript
{
  "mcpServers": {
    "bigquery": {
      "command": "npx",
      "args": ["@lucashild/mcp-server-bigquery"],
      "env": {
        "GOOGLE_APPLICATION_CREDENTIALS": "path/to/credentials.json",
        "PROJECT_ID": "your-project-id",
        "DATASET_ID": "your-dataset",
        "MAX_BYTES_BILLED": "1000000000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Google Cloud account
- BigQuery access
- Service account

## Related Servers

- ergut/mcp-bigquery-server
- monochromegane/mcp-bigquery-server