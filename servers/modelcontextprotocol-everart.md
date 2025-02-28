---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/tree/main/src/everart
name: Everart MCP Server
owner: modelcontextprotocol
stars: 9794
last_updated: 2025-02-21
status: active
official: true
verified: true
sources: ["inbox/batch_011.md"]
tags: ["status/active", "status/official", "status/verified", "category/ai", "purpose/image-generation", "tech/multi-model"]
---

# Everart MCP Server

#status/active #status/official #status/verified #category/ai #purpose/image-generation #tech/multi-model

## Description

AI image generation using various models, providing a unified interface for creating AI-generated images across different model architectures and styles.

## Features

- Multi-model support
- Image generation
- Style customization
- Model selection
- Parameter tuning
- Batch processing
- Format conversion
- Resolution control
- Progress tracking
- Result optimization

## Installation

```bash
npm install @modelcontextprotocol/everart
```

## Usage

```javascript
{
  "mcpServers": {
    "everart": {
      "command": "npx",
      "args": ["@modelcontextprotocol/everart"],
      "env": {
        "DEFAULT_MODEL": "stable-diffusion",
        "OUTPUT_DIR": "./generated",
        "MAX_RESOLUTION": "1024x1024",
        "BATCH_SIZE": "4"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- GPU support
- Image processing libraries
- Storage space
- Model weights

## Related Servers

- None currently listed