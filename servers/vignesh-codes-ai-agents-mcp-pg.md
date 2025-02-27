---
type: server
repo_url: https://github.com/vignesh-codes/ai-agents-mcp-pg
name: AI Agents PostgreSQL MCP Server
owner: vignesh-codes
stars: 2
last_updated: 2025-01-22
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/database", "tech/postgresql", "purpose/data-access", "category/ai"]
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

```bash
npm install @vignesh-codes/ai-agents-mcp-pg
```

## Usage

```javascript
{
  "mcpServers": {
    "ai-pg": {
      "command": "npx",
      "args": ["@vignesh-codes/ai-agents-mcp-pg"],
      "env": {
        "PG_CONNECTION_STRING": "postgresql://user:pass@localhost:5432/db",
        "MAX_QUERY_TIMEOUT": "5000",
        "READ_ONLY": "true",
        "SCHEMA_CACHE_TTL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- PostgreSQL >= 10
- pg-promise library
- Database credentials

## Related Servers

- None currently listed