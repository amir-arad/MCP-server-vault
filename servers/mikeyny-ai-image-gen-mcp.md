---
type: server
repo_url: https://github.com/mikeyny/ai-image-gen-mcp
name: AI Image Generation MCP Server
owner: mikeyny
stars: 28
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/ai", "category/image-generation", "integration/replicate", "purpose/content-creation"]
---

# AI Image Generation MCP Server

#status/active #category/ai #category/image-generation #integration/replicate #purpose/content-creation

## Description

Enables users to generate images from text prompts using Replicate's model, with configurable parameters and full MCP protocol compliance.

## Features

- Text-to-image generation
- Replicate model integration
- Configurable parameters
- MCP protocol compliance
- Image customization options
- Multiple model support
- Batch processing
- Result caching

## Installation

```bash
npm install @mikeyny/ai-image-gen-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "ai-image-gen": {
      "command": "npx",
      "args": ["@mikeyny/ai-image-gen-mcp"],
      "env": {
        "REPLICATE_API_TOKEN": "your-replicate-token",
        "DEFAULT_MODEL": "stability-ai/sdxl",
        "MAX_BATCH_SIZE": "4",
        "CACHE_DURATION": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Replicate API access
- Image processing libraries
- Cache storage (optional)

## Related Servers

- None currently listed