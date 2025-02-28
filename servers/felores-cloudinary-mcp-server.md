---
type: server
repo_url: https://github.com/felores/cloudinary-mcp-server
name: Cloudinary MCP Server
owner: felores
stars: 4
last_updated: 2025-02-18
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/media",
    "integration/cloudinary",
    "purpose/media-management",
    "purpose/upload",
    "tech/cloud-storage",
  ]
---

# Cloudinary MCP Server

#status/active #category/media #integration/cloudinary #purpose/media-management #purpose/upload #tech/cloud-storage

## Description

This server provides tools for uploading images and videos directly to Cloudinary using Claude/Cline, facilitating resource management with customizable options like resource type and public ID.

## Features

- Image uploading
- Video uploading
- Resource management
- Custom public IDs
- Format conversion
- Transformation options
- Metadata handling
- Asset organization
- Upload monitoring
- Error handling

## Installation

```bash
npm install @felores/cloudinary-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "cloudinary": {
      "command": "npx",
      "args": ["@felores/cloudinary-mcp"],
      "env": {
        "CLOUDINARY_CLOUD_NAME": "your-cloud-name",
        "CLOUDINARY_API_KEY": "your-api-key",
        "CLOUDINARY_API_SECRET": "your-api-secret",
        "DEFAULT_FOLDER": "uploads",
        "MAX_FILE_SIZE": "10mb"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Cloudinary account
- API credentials
- Upload handler
- Media processor
- Resource manager

## Related Servers

- modelcontextprotocol-media-server
- mikeyny-ai-image-gen-mcp
- modelcontextprotocol-storage-server
