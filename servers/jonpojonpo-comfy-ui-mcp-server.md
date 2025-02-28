---
type: server
repo_url: https://github.com/jonpojonpo/comfy-ui-mcp-server
name: ComfyUI Node Workflow MCP Server
owner: jonpojonpo
stars: 1
last_updated: 2025-01-21
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/ai",
    "integration/comfyui",
    "purpose/image-generation",
    "tech/node-based",
    "tech/stable-diffusion",
  ]
---

# ComfyUI Node Workflow MCP Server

#status/active #category/ai #integration/comfyui #purpose/image-generation #tech/node-based #tech/stable-diffusion

## Description

Integrates ComfyUI's stable diffusion interface to enable programmatic image generation through customizable node-based workflows. This server provides a programmatic interface to ComfyUI's visual workflow system.

## Features

- Node-based workflows
- Programmatic control
- Image generation
- Workflow customization
- Node management
- Parameter control
- Visual interface
- Workflow export
- Result handling
- Error management

## Installation

```bash
npm install @jonpojonpo/comfy-ui-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "comfy-ui": {
      "command": "npx",
      "args": ["@jonpojonpo/comfy-ui-mcp"],
      "env": {
        "COMFY_UI_URL": "http://localhost:8188",
        "WORKFLOW_DIR": "./workflows",
        "OUTPUT_DIR": "./outputs",
        "DEFAULT_MODEL": "sd_xl_base_1.0",
        "AUTO_LOAD": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- ComfyUI installation
- Stable Diffusion models
- Node manager
- Workflow engine
- Result processor

## Related Servers

- lalanikarim/comfy-mcp-pipeline
- lalanikarim/comfy-mcp-server
- mikeyny-ai-image-gen-mcp
