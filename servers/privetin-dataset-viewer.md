---
type: server
repo_url: https://github.com/privetin/dataset-viewer
name: Hugging Face Dataset Viewer MCP Server
owner: privetin
stars: 3
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/ai",
    "integration/huggingface",
    "purpose/dataset-exploration",
    "purpose/analysis",
    "tech/api",
  ]
---

# Hugging Face Dataset Viewer MCP Server

#status/active #category/ai #integration/huggingface #purpose/dataset-exploration #purpose/analysis #tech/api

## Description

Integrates with the Hugging Face Dataset Viewer API to enable exploration, analysis, and content retrieval of datasets hosted on the Hugging Face Hub.

## Features

- Dataset exploration
- Content retrieval
- Data analysis
- Search functionality
- Metadata access
- Dataset statistics
- Sample viewing
- Format conversion
- Filter support
- Export capabilities

## Installation

```bash
npm install @privetin/dataset-viewer-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "dataset-viewer": {
      "command": "npx",
      "args": ["@privetin/dataset-viewer-mcp"],
      "env": {
        "HF_TOKEN": "your-huggingface-token",
        "CACHE_PATH": "./cache",
        "MAX_SAMPLES": "1000",
        "PREVIEW_SIZE": "10",
        "DOWNLOAD_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Hugging Face account
- API token
- Dataset loader
- Cache system
- Analysis tools

## Related Servers

- reading-plus-ai-mcp-server-data-exploration
- modelcontextprotocol-dataset-server
- modelcontextprotocol-huggingface-server
