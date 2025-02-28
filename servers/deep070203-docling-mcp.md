---
type: server
repo_url: https://github.com/Deep070203/docling-mcp
name: Docling MCP Server
owner: Deep070203
stars: 4
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_010.md"]
tags: ["status/active", "category/document-processing", "integration/ibm", "purpose/document-conversion", "tech/markdown", "purpose/parsing"]
---

# Docling MCP Server

#status/active #category/document-processing #integration/ibm #purpose/document-conversion #tech/markdown #purpose/parsing

## Description

Integrates IBM's Docling software to parse and convert various document formats into standardized Markdown, enabling efficient document processing and analysis workflows.

## Features

- Multi-format document parsing
- Markdown conversion
- Document standardization
- Format detection
- Metadata extraction
- Content structuring
- Batch processing
- Error handling
- Progress tracking
- Custom formatting rules

## Installation

```bash
npm install @deep070203/docling-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "docling": {
      "command": "npx",
      "args": ["@deep070203/docling-mcp"],
      "env": {
        "IBM_API_KEY": "your-ibm-api-key",
        "DOCLING_WORKSPACE": "./workspace",
        "OUTPUT_FORMAT": "markdown"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- IBM Docling SDK
- IBM Cloud account
- Document processing libraries
- Storage space for processing

## Related Servers

- None currently listed