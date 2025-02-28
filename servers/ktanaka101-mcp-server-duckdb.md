---
type: server
repo_url: https://github.com/ktanaka101/mcp-server-duckdb
name: DuckDB MCP Server
owner: ktanaka101
stars: 43
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/database",
    "integration/duckdb",
    "purpose/data-analysis",
    "tech/sql",
    "purpose/local-analysis",
  ]
---

# DuckDB MCP Server

#status/active #category/database #integration/duckdb #purpose/data-analysis #tech/sql #purpose/local-analysis

## Description

A Model Context Protocol (MCP) server implementation for DuckDB, providing database interaction capabilities through MCP tools. DuckDB is suitable for local analysis with its efficient columnar-based storage and processing.

## Features

- SQL query execution
- Data import/export
- Schema management
- Data analysis tools
- Query optimization
- Column-based storage
- Transaction support
- Data type handling
- Index management
- Performance monitoring

## Installation

To install DuckDB Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/mcp-server-duckdb):

```bash
npx -y @smithery/cli install mcp-server-duckdb --client claude
```

## Usage

Configure the MCP server in Claude Desktop's configuration file:

#### MacOS

Location: `~/Library/Application Support/Claude/claude_desktop_config.json`

#### Windows

Location: `%APPDATA%/Claude/claude_desktop_config.json`

```json
{
  "mcpServers": {
    "duckdb": {
      "command": "uvx",
      "args": [
        "mcp-server-duckdb",
        "--db-path",
        "~/mcp-server-duckdb/data/data.db"
      ]
    }
  }
}
```

- Note: `~/mcp-server-duckdb/data/data.db` should be replaced with the actual path to the DuckDB database file.

## Dependencies

- Rust >= 1.54
- DuckDB
- SQLite (for compatibility)
- File system access
- Memory for analysis
