---
type: server
repo_url: https://github.com/aaronsb/confluence-cloud-mcp
name: Confluence Cloud MCP Server
owner: aaronsb
stars: 5
last_updated: 2025-02-06
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/confluence",
    "tech/cloud",
    "purpose/content-management",
    "purpose/space-management",
  ]
---

# Confluence Cloud MCP Server

#status/active #category/productivity #integration/confluence #tech/cloud #purpose/content-management #purpose/space-management

## Description

Enables AI assistants to interact with Confluence Cloud for managing spaces, pages, and content via the Model Context Protocol (MCP).

## Features

- Space management
- Page management
- Content editing
- Permission control
- Version tracking
- Search functionality
- Template support
- Attachment handling
- Comment management
- Analytics access

## Installation

```bash
npm install @aaronsb/confluence-cloud-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "confluence-cloud": {
      "command": "npx",
      "args": ["@aaronsb/confluence-cloud-mcp"],
      "env": {
        "CONFLUENCE_CLOUD_URL": "your-instance.atlassian.net",
        "API_TOKEN": "your-api-token",
        "DEFAULT_SPACE": "your-space-key",
        "BATCH_SIZE": "50",
        "RETRY_ATTEMPTS": "3"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Confluence Cloud account
- API token
- Content processor
- Permission manager
- Version controller

## Related Servers

- mouhamadalmounayar/mcp-confluence
- zereight/confluence-mcp
- ks-gen-ai/confluence-mcp-server
