---
type: server
repo_url: https://github.com/zcaceres/fetch-mcp
name: Fetch MCP Server
owner: zcaceres
stars: 55
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/web",
    "purpose/content-fetching",
    "tech/multi-format",
    "purpose/data-retrieval",
    "tech/format-conversion",
    "tech/typescript",
    "tech/javascript",
    "tech/jsdom",
    "tech/turndown"
  ]
---

# Fetch MCP Server

#status/active #category/web #purpose/content-fetching #tech/multi-format #purpose/data-retrieval #tech/format-conversion #tech/typescript #tech/javascript #tech/jsdom #tech/turndown

## Description

A TypeScript-based MCP server that provides flexible HTTP fetching capabilities with multi-format support. The server enables fetching and transforming web content in various formats including HTML, JSON, plain text, and Markdown, using modern fetch API and specialized format converters.

## Features

- Multi-format content fetching
- HTML content retrieval
- JSON data parsing
- Plain text extraction
- Markdown conversion
- Format auto-detection
- Content validation
- Error handling
- Response formatting
- Cache management
- Custom headers support
- JSDOM integration
- TurndownService support
- TypeScript types
- Modern fetch API

## Installation

```bash
# Install dependencies
npm install

# Build the server
npm run build

# Start the server
npm start
```

## Usage

```javascript
{
  "mcpServers": {
    "fetch": {
      "command": "node",
      "args": ["{ABSOLUTE PATH}/dist/index.js"],
      "env": {
        "DEFAULT_FORMAT": "markdown",
        "CACHE_TTL": "3600",
        "TIMEOUT": "30000",
        "MAX_SIZE": "5242880"
      }
    }
  }
}

// Available Tools
fetch_html:
  - url: Website URL to fetch
  - headers: Optional custom headers

fetch_json:
  - url: JSON URL to fetch
  - headers: Optional custom headers

fetch_txt:
  - url: Website URL to fetch
  - headers: Optional custom headers

fetch_markdown:
  - url: Website URL to fetch
  - headers: Optional custom headers
```

## Dependencies

- Node.js >= 14
- TypeScript runtime
- JSDOM parser
- TurndownService
- Format converters
- Network client
- Cache system
- Content validators
- Error handlers
- Response formatters

## Related Servers

- modelcontextprotocol/fetch-server
- thesethrose/fetch-browser
- kazuph/mcp-fetch
- exactdoug/mcp-fetch