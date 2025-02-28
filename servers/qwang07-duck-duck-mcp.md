---
type: server
repo_url: https://github.com/qwang07/duck-duck-mcp
name: DuckDuckGo MCP Server
owner: qwang07
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/search",
    "integration/duckduckgo",
    "purpose/web-search",
    "purpose/metadata",
    "tech/content-classification",
  ]
---

# DuckDuckGo MCP Server

#status/active #category/search #integration/duckduckgo #purpose/web-search #purpose/metadata #tech/content-classification

## Description

This MCP server utilizes DuckDuckGo for web searches, providing structured search results with metadata and features like smart content classification and language detection, facilitating easy integration with AI clients supporting the MCP protocol.

## Features

- Web search capabilities
- Metadata extraction
- Content classification
- Language detection
- Structured results
- Search filtering
- Result ranking
- Safe search options
- Region-specific search
- Result caching

## Installation

```bash
npm install @qwang07/duck-duck-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "duckduckgo": {
      "command": "npx",
      "args": ["@qwang07/duck-duck-mcp"],
      "env": {
        "SAFE_SEARCH": "moderate",
        "REGION": "us-en",
        "CACHE_DURATION": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- DuckDuckGo API access
- Language detection libraries
- Content classification models
- Caching system

## Related Servers

- [DuckDuckGo Search](https://github.com/spences10/mcp-duckduckgo-search) - Alternative DuckDuckGo integration
