---
type: server
repo_url: https://github.com/kazuph/mcp-fetch
name: Fetch MCP Server
owner: kazuph
stars: 6
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
    "purpose/image-processing",
    "tech/web-content",
    "category/media",
    "tech/javascript",
    "tech/sharp",
    "tech/mozjpeg",
    "platform/macos"
  ]
---

# Fetch MCP Server

#status/active #category/web #purpose/content-fetching #purpose/image-processing #tech/web-content #category/media #tech/javascript #tech/sharp #tech/mozjpeg #platform/macos

## Description

A JavaScript-based MCP server designed for macOS that provides web content fetching and image processing capabilities. The server enables automated extraction and optimization of web content and images, supporting features like article title extraction, image optimization, and pagination, specifically tailored for Claude Desktop integration.

## Features

- Web content extraction
- Article title parsing
- Image processing
- Content optimization
- Format conversion
- Resource handling
- Cache management
- Error handling
- Response formatting
- Image resizing
- Content validation
- JPEG optimization
- GIF frame extraction
- Pagination support
- Clipboard integration

## Installation

```bash
# Install global dependencies
npm install -g tsx

# Install server
npm install @kazuph/mcp-fetch

# Configure Claude Desktop
# Edit ~/Library/Application Support/Claude/claude_desktop_config.json:
{
  "tools": {
    "fetch": {
      "command": "npx",
      "args": ["-y", "@kazuph/mcp-fetch"]
    }
  }
}
```

## Usage

```javascript
// Configuration Parameters
url: "https://example.com",  // Required
maxLength: 20000,           // Max content length
startIndex: 0,              // Content start position
imageStartIndex: 0,         // Image collection start
raw: false,                 // Raw vs markdown content
imageMaxCount: 3,           // Max images per request
imageMaxHeight: 4000,       // Max merged image height
imageMaxWidth: 1000,        // Max image width
imageQuality: 80,           // JPEG quality (1-100)
disableImages: false,       // Skip image processing
ignoreRobotsTxt: false      // Ignore robots.txt

// Image Processing Specs
- JPEG format conversion
- Width limit: 1200px
- Height limit: 1600px
- Chroma subsampling (4:2:0)
- MozJPEG optimization
```

## Dependencies

- Node.js >= 18
- macOS system
- Claude Desktop
- Sharp library
- MozJPEG
- TSX runtime
- Image processors
- Web fetchers
- Cache system
- Clipboard manager

## Related Servers

- zcaceres/fetch-mcp
- thesethrose/fetch-browser
- exactdoug/mcp-fetch
- modelcontextprotocol/fetch-server