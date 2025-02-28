---
type: server
repo_url: https://github.com/mshaaban0/contentful-delivery-mcp
name: Contentful Delivery MCP Server
owner: mshaaban0
stars: 0
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
    "tech/typescript",
    "tech/javascript",
    "purpose/content-delivery",
    "purpose/notes",
    "integration/mastra-ai"
  ]
---

# Contentful Delivery MCP Server

#status/active #category/cms #integration/contentful #tech/typescript #tech/javascript #purpose/content-delivery #purpose/notes #integration/mastra-ai

## Description

A TypeScript-based MCP server that provides seamless access to Contentful's Delivery API through AI assistants. The server enables natural language querying and retrieval of content entries, assets, and content types from Contentful, with built-in support for Mastra AI integration.

## Features

- Natural language content querying
- Entry management and retrieval
- Asset handling and browsing
- Content type schema access
- Pagination support
- Rich text content handling
- Mastra AI integration
- Type-safe implementation
- Content modeling support
- Version control

## Installation

```bash
# Project installation
npm install @mshaaban0/contentful-delivery-mcp

# Global installation
npm install -g @mshaaban0/contentful-delivery-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "contentful-delivery": {
      "command": "npx",
      "args": ["@mshaaban0/contentful-delivery-mcp"],
      "env": {
        "CONTENTFUL_SPACE_ID": "your-space-id",
        "CONTENTFUL_ACCESS_TOKEN": "your-access-token",
        "ENVIRONMENT": "master",
        "LOCALE": "en-US",
        "CACHE_DURATION": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript runtime
- Contentful SDK
- Content processor
- Query engine
- Cache system
- Mastra AI SDK (optional)
- MCP Inspector (for debugging)

## Related Servers

- ivo-toby/contentful-mcp
- modelcontextprotocol-cms-server
- akira-papa-akirapapa-mcp-notion-server