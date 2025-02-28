---
type: server
repo_url: https://github.com/llmian-space/devdocs-mcp
name: DevDocs MCP Server
owner: llmian-space
stars: 0
last_updated: 2025-01-20
status: active
official: false
verified: false
sources: ["inbox/batch_009.md"]
tags:
  [
    "status/active",
    "category/documentation",
    "purpose/indexing",
    "purpose/retrieval",
    "purpose/code-assistance",
    "purpose/api-docs",
  ]
---

# DevDocs MCP Server

#status/active #category/documentation #purpose/indexing #purpose/retrieval #purpose/code-assistance #purpose/api-docs

## Description

Integrates with software documentation sources to process, index, and retrieve technical content for enhanced code assistance and API exploration.

## Features

- Documentation indexing
- Content retrieval
- API documentation
- Search functionality
- Content processing
- Version tracking
- Language support
- Code examples
- Quick reference
- Context awareness

## Installation

```bash
npm install @llmian-space/devdocs-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "devdocs": {
      "command": "npx",
      "args": ["@llmian-space/devdocs-mcp"],
      "env": {
        "DOCS_PATH": "./documentation",
        "INDEX_INTERVAL": "3600",
        "LANGUAGES": "javascript,python,ruby",
        "CACHE_TTL": "86400",
        "SEARCH_DEPTH": "3"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Documentation parser
- Search indexer
- Content processor
- Cache system
- Version tracker

## Related Servers

- modelcontextprotocol-docs-server
- nahmanmate/code-research-mcp-server
- daipendency/daipendency-mcp
