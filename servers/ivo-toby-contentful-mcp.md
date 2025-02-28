---
type: server
repo_url: https://github.com/ivo-toby/contentful-mcp
name: Contentful Management MCP Server
owner: ivo-toby
stars: 6
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/cms",
    "integration/contentful",
    "purpose/content-management",
    "purpose/asset-management",
    "purpose/modeling",
    "tech/typescript",
    "tech/javascript",
    "integration/smithery"
  ]
---

# Contentful Management MCP Server

#status/active #category/cms #integration/contentful #purpose/content-management #purpose/asset-management #purpose/modeling #tech/typescript #tech/javascript #integration/smithery

## Description

A comprehensive MCP server implementation that integrates with Contentful's Content Management API, providing full CRUD operations for content, assets, spaces, and content models. Features smart pagination to prevent context window overflow and supports multiple deployment options including Smithery integration.

## Features

- Content Management (CRUD operations)
- Space and Environment Management
- Content Type Definition Control
- Asset Management and Processing
- Smart Pagination (3 items per request)
- Multi-locale Support
- Publishing Workflow Control
- Version Management
- App Identity Support
- Error Handling
- Real-time Development Tools

## Installation

```bash
# Via npm
npm install @ivo-toby/contentful-mcp

# Via Smithery (recommended for Claude Desktop)
npx -y @smithery/cli install @ivotoby/contentful-management-mcp-server --client claude
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
- TypeScript Runtime
- Contentful Management API
- Content Validator
- Asset Processor
- Model Manager
- Backup System
- MCP Inspector (for debugging)

## Related Servers

- mshaaban0/contentful-delivery-mcp
- modelcontextprotocol-cms-server
- akira-papa-akirapapa-mcp-notion-server