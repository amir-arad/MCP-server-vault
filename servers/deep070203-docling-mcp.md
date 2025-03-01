--- 
type: server
repo_url: https://github.com/Deep070203/docling-mcp
name: Docling MCP Server
owner: Deep070203
stars: 5
last_updated: 2025-03-01
status: active
official: false
verified: true
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

To use the published one, add the below code to Claude config file.

## Usage

```javascript
{
  "mcpServers": {
    "docling-mcp": {
      "command": "uvx",
      "args": ["docling-mcp"]
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