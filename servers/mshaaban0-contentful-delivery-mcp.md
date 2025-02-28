---
type: server
repo_url: https://github.com/mshaaban0/contentful-delivery-mcp
name: Contentful Delivery MCP Server
owner: mshaaban0
stars: 0
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/cms",
    "integration/contentful",
    "tech/typescript",
    "purpose/content-delivery",
    "purpose/notes",
  ]
---

# Contentful Delivery MCP Server

#status/active #category/cms #integration/contentful #tech/typescript #purpose/content-delivery #purpose/notes

## Description

A TypeScript-based MCP server that interacts with Contentful's Delivery API, enabling users to create, query, and summarize text notes through natural language.

## Features

- Content delivery
- Note creation
- Query capabilities
- Text summarization
- Content management
- Natural language interface
- Type safety
- Content modeling
- Asset handling
- Version control

## Installation

```bash
npm install @mshaaban0/contentful-delivery-mcp
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
- TypeScript
- Contentful SDK
- Content processor
- Query engine
- Cache system

## Related Servers

- ivo-toby/contentful-mcp
- modelcontextprotocol-cms-server
- akira-papa-akirapapa-mcp-notion-server
