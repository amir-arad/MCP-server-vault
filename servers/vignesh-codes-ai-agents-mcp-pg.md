---
type: server
repo_url: https://github.com/vignesh-codes/ai-agents-mcp-pg
name: AI Agents PostgreSQL MCP Server
owner: vignesh-codes
stars: 4
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/active",
    "category/database",
    "tech/postgresql",
    "purpose/data-access",
    "category/ai",
  ]
---

# AI Agents PostgreSQL MCP Server

#status/active #category/database #tech/postgresql #purpose/data-access #category/ai

## Description

A Model Context Protocol server providing LLMs read-only access to PostgreSQL databases for inspecting schemas and executing queries.

## Features

- PostgreSQL database integration
- Schema inspection capabilities
- Read-only query execution
- AI-safe database access
- Query validation and sanitization
- Performance optimization

## Installation

First, ensure you've installed Docker and Claude Desktop

To install the PostgreSQL MCP Server, follow these steps:

1.  Clone the repository: `git clone https://github.com/vignesh-codes/ai-agents-mcp-pg.git`
2.  Run PG Docker container `docker run --name postgres-container -e POSTGRES_USER=admin -e POSTGRES_PASSWORD=admin_password -e POSTGRES_DB=mydatabase -p 5432:5432 -d postgres:latest`
3.  Build the mcp server: `docker build -t mcp/postgres -f src/Dockerfile .`
4.  Open Claude Desktop and connect to the MCP server by updating the `mcpServers` field in `claude_desktop_config.json`:

## Usage

To use this server with the Claude Desktop app, add the following configuration to the "mcpServers" section of your `claude_desktop_config.json`:

### Docker

- When running Docker on macOS, use `host.docker.internal` if the server is running on the host network (e.g., localhost).
- Username/password can be added to the PostgreSQL URL with `postgresql://user:password@host:port/db-name`.

```json
{
  "mcpServers": {
    "postgres": {
      "command": "docker",
      "args": [
        "run",
        "-i",
        "--rm",
        "mcp/postgres",
        "postgresql://username:password@host.docker.internal:5432/mydatabase"
      ]
    }
  }
}
```

```

## Dependencies

- Node.js >= 14
- PostgreSQL >= 10
- pg-promise library
- Database credentials

## Related Servers

- None currently listed
```
