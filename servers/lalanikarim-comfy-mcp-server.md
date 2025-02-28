---
type: server
repo_url: https://github.com/lalanikarim/comfy-mcp-server
name: Comfy FastMCP Server
owner: lalanikarim
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
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

You can install the required packages for local development:

```bash
uvx mcp[cli]
```

## Usage

Set the following environment variables:

- `COMFY_URL` to point to your Comfy server URL.
- `COMFY_WORKFLOW_JSON_FILE` to point to the absolute path of the API export json file for the comfyui workflow.
- `PROMPT_NODE_ID` to the id of the text prompt node.
- `OUTPUT_NODE_ID` to the id of the output node with the final image.
- `OUTPUT_MODE` to either `url` or `file` to select desired output.

Example:

```bash
export COMFY_URL=http://your-comfy-server-url:port
export COMFY_WORKFLOW_JSON_FILE=/path/to/the/comfyui_workflow_export.json
export PROMPT_NODE_ID=6 # use the correct node id here
export OUTPUT_NODE_ID=9 # use the correct node id here
export OUTPUT_MODE=file
```

Comfy MCP Server can be launched by the following command:

```bash
uvx comfy-mcp-server
```

### Example Claude Desktop Config

```json
{
  "mcpServers": {
    "Comfy MCP Server": {
      "command": "/path/to/uvx",
      "args": ["comfy-mcp-server"],
      "env": {
        "COMFY_URL": "http://your-comfy-server-url:port",
        "COMFY_WORKFLOW_JSON_FILE": "/path/to/the/comfyui_workflow_export.json",
        "PROMPT_NODE_ID": "6",
        "OUTPUT_NODE_ID": "9",
        "OUTPUT_MODE": "file"
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
