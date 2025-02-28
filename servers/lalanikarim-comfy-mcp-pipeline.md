---
type: server
repo_url: https://github.com/lalanikarim/comfy-mcp-pipeline
name: ComfyUI Pipeline MCP Server
owner: lalanikarim
stars: 3
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/ai",
    "integration/comfyui",
    "purpose/image-generation",
    "tech/stable-diffusion",
    "purpose/workflow",
  ]
---

# ComfyUI Pipeline MCP Server

#status/active #category/ai #integration/comfyui #purpose/image-generation #tech/stable-diffusion #purpose/workflow

## Description

Integrates with ComfyUI to enable natural language-driven image generation using customizable Stable Diffusion workflows. This server provides a pipeline for creating images through natural language commands.

## Features

- Natural language control
- Image generation
- Workflow customization
- Pipeline management
- Stable Diffusion integration
- Parameter control
- Batch processing
- Result management
- Workflow templates
- Error handling

## Installation

```bash
npm install @lalanikarim/comfy-mcp-pipeline
```

## Usage

```javascript
{
  "mcpServers": {
    "comfy-pipeline": {
      "command": "npx",
      "args": ["@lalanikarim/comfy-mcp-pipeline"],
      "env": {
        "COMFY_API_URL": "http://localhost:8188",
        "DEFAULT_MODEL": "stable-diffusion-v1-5",
        "MAX_BATCH_SIZE": "4",
        "SAVE_PATH": "./outputs",
        "WORKFLOW_PATH": "./workflows"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- ComfyUI installation
- Stable Diffusion models
- GPU support
- Pipeline manager
- Image processor

## Related Servers

- lalanikarim/comfy-mcp-server
- jonpojonpo/comfy-ui-mcp-server
- mikeyny-ai-image-gen-mcp
