---
type: server
repo_url: https://github.com/ivo-toby/contentful-mcp
name: Contentful Management MCP Server
owner: ivo-toby
stars: 6
last_updated: 2025-02-14
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/cms",
    "integration/contentful",
    "purpose/content-management",
    "purpose/asset-management",
    "purpose/modeling",
  ]
---

# Contentful Management MCP Server

#status/active #category/cms #integration/contentful #purpose/content-management #purpose/asset-management #purpose/modeling

## Description

Update, create, delete content, content-models and assets in your Contentful Space. This server provides comprehensive management capabilities for Contentful content management system.

## Features

- Content management
- Model creation
- Asset handling
- Content updates
- Content deletion
- Model validation
- Asset processing
- Version control
- Space management
- Localization support

## Installation

```bash
npm install @ivo-toby/contentful-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "contentful-management": {
      "command": "npx",
      "args": ["@ivo-toby/contentful-mcp"],
      "env": {
        "CONTENTFUL_SPACE_ID": "your-space-id",
        "CONTENTFUL_MANAGEMENT_TOKEN": "your-token",
        "DEFAULT_LOCALE": "en-US",
        "ENVIRONMENT": "master",
        "BACKUP_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Contentful Management API
- Content validator
- Asset processor
- Model manager
- Backup system

## Related Servers

- mshaaban0/contentful-delivery-mcp
- modelcontextprotocol-cms-server
- akira-papa-akirapapa-mcp-notion-server
