---
type: server
repo_url: https://github.com/afrise/academic-search-mcp-server
name: Academic Search MCP Server
owner: afrise
stars: 5
last_updated: 2025-02-12
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/search", "category/academic", "purpose/research"]
---

# Academic Search MCP Server

#status/active #category/search #category/academic #purpose/research

## Description

Enables real-time search and retrieval of academic paper information from multiple sources, providing access to paper metadata, abstracts, and full-text content when available, with structured data responses for integration with AI models.

## Features

- Multi-source academic paper search
- Metadata retrieval
- Abstract access
- Full-text content retrieval when available
- Structured data responses
- Integration with AI models

## Installation

```bash
npm install @afrise/academic-search-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "academic-search": {
      "command": "npx",
      "args": ["@afrise/academic-search-mcp"],
      "env": {
        "ACADEMIC_API_KEY": "your-api-key",
        "MAX_RESULTS": "100",
        "CACHE_DURATION": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Academic API access credentials
- Redis (optional, for caching)

## Related Servers

- None currently listed