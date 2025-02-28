---
type: server
repo_url: https://github.com/LucasHild/mcp-server-bigquery
name: BigQuery MCP Server
owner: LucasHild
stars: 12
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
  ]
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

### Tools

The server implements the following tools:

- `execute-query`: Executes a SQL query using BigQuery dialect
- `list-tables`: Lists all tables in the BigQuery database
- `describe-table`: Describes the schema of a specific table

## Installation

To install BigQuery Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/mcp-server-bigquery):

```bash
npx -y @smithery/cli install mcp-server-bigquery --client claude
```

### Claude Desktop

On MacOS: `~/Library/Application\ Support/Claude/claude_desktop_config.json` On Windows: `%APPDATA%/Claude/claude_desktop_config.json`

#### Development/Unpublished Servers Configuration

```json
"mcpServers": {
  "bigquery": {
    "command": "uv",
    "args": [
      "--directory",
      "{{PATH_TO_REPO}}",
      "run",
      "mcp-server-bigquery",
      "--project",
      "{{GCP_PROJECT_ID}}",
      "--location",
      "{{GCP_LOCATION}}"
    ]
  }
}
```

#### Published Servers Configuration

```json
"mcpServers": {
  "bigquery": {
    "command": "uvx",
    "args": [
      "mcp-server-bigquery",
      "--project",
      "{{GCP_PROJECT_ID}}",
      "--location",
      "{{GCP_LOCATION}}"
    ]
  }
}
```

Replace `{{PATH_TO_REPO}}`, `{{GCP_PROJECT_ID}}`, and `{{GCP_LOCATION}}` with the appropriate values.

## Dependencies

- Node.js >= 14
- Google Cloud account
- BigQuery access
- Service account
