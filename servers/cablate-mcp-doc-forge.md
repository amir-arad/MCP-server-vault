---
type: server
repo_url: https://github.com/cablate/mcp-doc-forge
name: Doc Forge MCP Server
owner: cablate
stars: 0
last_updated: 2025-02-14
status: active
official: false
verified: false
sources: ["inbox/batch_010.md"]
tags: ["status/active", "category/document-processing", "purpose/file-conversion", "purpose/text-processing", "tech/html", "purpose/document-manipulation"]
---

# Doc Forge MCP Server

#status/active #category/document-processing #purpose/file-conversion #purpose/text-processing #tech/html #purpose/document-manipulation

## Description

Provides comprehensive document processing, including reading, converting, and manipulating various document formats with advanced text and HTML processing capabilities.

## Features

- Multi-format document reading
- Document format conversion
- Text processing and manipulation
- HTML processing
- Document metadata extraction
- Content formatting
- Template-based generation
- Batch processing
- Document merging
- Format validation

## Installation

```bash
npm install @cablate/mcp-doc-forge
```

## Usage

```javascript
{
  "mcpServers": {
    "doc-forge": {
      "command": "npx",
      "args": ["@cablate/mcp-doc-forge"],
      "env": {
        "DOC_FORGE_TEMP_DIR": "/tmp/doc-forge",
        "MAX_FILE_SIZE": "10485760",
        "SUPPORTED_FORMATS": "pdf,docx,html,md"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- LibreOffice (for document conversion)
- Pandoc
- ImageMagick (for image processing)
- PDF processing libraries

## Related Servers

- None currently listed