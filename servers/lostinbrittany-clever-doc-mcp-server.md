---
type: server
repo_url: https://github.com/LostInBrittany/clever-doc-mcp-server
name: Clever Cloud Documentation MCP Server
owner: LostInBrittany
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/documentation",
    "integration/clever-cloud",
    "purpose/knowledge-base",
    "purpose/query",
    "tech/typescript",
  ]
---

# Clever Cloud Documentation MCP Server

#status/active #category/documentation #integration/clever-cloud #purpose/knowledge-base #purpose/query #tech/typescript

## Description

This MCP demo Server based on [FastMCP](https://github.com/punkpeye/fastmcp), exposes [Clever Cloud](https://clever-cloud.com)'s documentation, allowing users to query and interact with it through Model Context Protocol clients like Claude Desktop.

## Features

- Documentation access
- Content querying
- Search functionality
- Version tracking
- Topic navigation
- Example code retrieval
- API documentation
- Tutorial access
- Content indexing
- Update notifications

## Usage

To use this server in an MCP client such as Claude Desktop:

```json
{
  "mcpServers": {
    "mcp-clever-demo": {
      "command": "npx",
      "args": ["-y", "mcp-clever-demo"]
    }
  }
}
```

## Development

### Test with `mcp-cli`

The fastest way to test and debug your server is with fastmcp dev:

```bash
npx fastmcp dev src/index.ts
```

This will run your server with [`mcp-cli`](https://github.com/wong2/mcp-cli) for testing and debugging your MCP server in the terminal.

### Inspect with MCP Inspector

Another way is to use the official [MCP Inspector](https://modelcontextprotocol.io/docs/tools/inspector) to inspect your server with a Web UI:

```bash
npx fastmcp inspect src/index.ts
```

## Dependencies

- Node.js >= 16
- Documentation indexer
- Search engine
- Cache system
- Content parser
- Version tracker

## Related Servers

- davlgd-mcp-clever-demo
- modelcontextprotocol-docs-server
- mendableai-firecrawl-mcp-server
