---
type: server
repo_url: https://github.com/lalanikarim/comfy-mcp-server
name: Comfy FastMCP Server
owner: lalanikarim
stars: 2
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/ai",
    "integration/comfy",
    "tech/fastmcp",
    "purpose/image-generation",
    "tech/remote",
  ]
---

# Comfy FastMCP Server

#status/active #category/ai #integration/comfy #tech/fastmcp #purpose/image-generation #tech/remote

## Description

The Comfy MCP Server uses the FastMCP framework to generate images from prompts by interacting with a remote Comfy server, allowing automated image creation based on workflow configurations.

## Features

- FastMCP integration
- Remote server interaction
- Image generation
- Prompt processing
- Workflow configuration
- Result handling
- Queue management
- Status tracking
- Error recovery
- Resource management

## Installation

```bash
npm install @lalanikarim/comfy-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "comfy-server": {
      "command": "npx",
      "args": ["@lalanikarim/comfy-mcp-server"],
      "env": {
        "COMFY_SERVER_URL": "http://remote-server:8188",
        "WORKFLOW_CONFIG": "./workflow.json",
        "MAX_CONCURRENT": "2",
        "TIMEOUT": "300",
        "RETRY_ATTEMPTS": "3"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- FastMCP framework
- Remote Comfy server
- Queue system
- Status tracker
- Result handler

## Related Servers

- lalanikarim/comfy-mcp-pipeline
- jonpojonpo/comfy-ui-mcp-server
- mikeyny-ai-image-gen-mcp
