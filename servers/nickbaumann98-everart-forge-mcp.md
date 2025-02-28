---
type: server
repo_url: https://github.com/nickbaumann98/everart-forge-mcp
name: Everart Forge MCP Server
owner: nickbaumann98
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/ai",
    "integration/everart",
    "purpose/image-generation",
    "tech/vector",
    "tech/raster",
    "tech/javascript"
  ]
---

# Everart Forge MCP Server

#status/active #category/ai #integration/everart #purpose/image-generation #tech/vector #tech/raster #tech/javascript

## Description

An advanced MCP server for Cline that leverages EverArt's AI models to generate vector and raster images, supporting flexible storage, multiple formats, and robust image generation capabilities. It provides powerful image generation capabilities with flexible storage options and format conversion, enabling AI-driven art creation.

## Features

- Vector image generation
- Raster image generation
- Flexible storage options
- Multiple format support (SVG, PNG, JPEG, WebP)
- AI model integration
- Format conversion
- Batch processing
- Quality control
- Style customization
- Output optimization
- Cline integration

## Installation

```bash
npm install @nickbaumann98/everart-forge-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "everart-forge": {
      "command": "npx",
      "args": ["@nickbaumann98/everart-forge-mcp"],
      "env": {
        "STORAGE_PATH": "./storage",
        "VECTOR_FORMATS": "svg,ai,eps",
        "RASTER_FORMATS": "png,jpg,webp",
        "MAX_BATCH_SIZE": "10",
        "EVERART_API_KEY": "your_api_key_here"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- EverArt AI models
- Vector graphics libraries
- Image processing tools
- Storage system
- TypeScript runtime

## Related Servers

- modelcontextprotocol/servers/tree/main/src/everart