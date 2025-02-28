---
type: server
repo_url: https://github.com/shin-t-o/mcp-access
name: Access MCP Server
owner: shin-t-o
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/active",
    "category/content-processing",
    "category/automation",
    "purpose/data-extraction",
    "tech/nodejs",
  ]
---

# Access MCP Server

#status/active #category/content-processing #category/automation #purpose/data-extraction

## Description

Enables text extraction from web pages and PDFs, and execution of predefined commands, enhancing content processing and automation capabilities.

## Features

- Web page text extraction
- PDF content extraction
- Predefined command execution
- Content processing automation
- Structured data output

## Installation

```bash
npm install @shin-t-o/mcp-access
```

## Usage

```javascript
{
  "mcpServers": {
    "access": {
      "command": "npx",
      "args": ["@shin-t-o/mcp-access"],
      "env": {
        "ALLOWED_DOMAINS": "domain1.com,domain2.com",
        "MAX_FILE_SIZE": "10MB",
        "TIMEOUT": "30000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- PDF processing libraries
- Puppeteer (for web scraping)

## Related Servers

- None currently listed
