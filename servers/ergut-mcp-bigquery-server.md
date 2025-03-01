---
type: server
repo_url: https://github.com/ergut/mcp-bigquery-server
name: BigQuery MCP Server
owner: ergut
stars: 9
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "category/database",
    "integration/bigquery",
    "purpose/data-analysis",
    "integration/google",
    "tech/javascript",
  ]
---

# BigQuery MCP Server

#status/active #category/database #integration/bigquery #purpose/data-analysis #integration/google

## Description

This is a server that lets your LLMs (like Claude) talk directly to your BigQuery data! Think of it as a friendly translator that sits between your AI assistant and your database, making sure they can chat securely and efficiently.

## Features

- Direct BigQuery access
- Natural language queries
- Secure communication
- Efficient translation
- Query optimization
- Result formatting
- Schema management
- Access control

## Installation

```bash
npm install @ergut/mcp-bigquery
```

## Usage

```javascript
{
  "mcpServers": {
    "bigquery": {
      "command": "npx",
      "args": ["@ergut/mcp-bigquery"],
      "env": {
        "GOOGLE_CREDENTIALS": "path/to/credentials.json",
        "PROJECT_ID": "your-project-id",
        "DEFAULT_DATASET": "your-dataset",
        "QUERY_TIMEOUT": "30"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Google Cloud account
- BigQuery access
- Service credentials

## Related Servers

- LucasHild/mcp-server-bigquery
- monochromegane/mcp-bigquery-server
