---
type: server
repo_url: https://github.com/Akira-Papa/akirapapa-mcp-notion-server
name: Akirapapa Notion Server
owner: Akira-Papa
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/notion",
    "purpose/knowledge-management",
  ]
---

# Akirapapa Notion Server

#status/active #category/productivity #integration/notion #purpose/knowledge-management

## Description

Integrates Notion workspaces, enabling seamless interaction with Notion's API for tasks like automated note-taking and knowledge base management.

## Features

- Notion workspace integration
- Automated note-taking
- Knowledge base management
- Page creation and editing
- Database operations
- Block manipulation
- Content organization
- Search capabilities

## Installation

```bash
npm install @akira-papa/mcp-notion-server
```

## Usage

```javascript
{
  "mcpServers": {
    "notion": {
      "command": "npx",
      "args": ["@akira-papa/mcp-notion-server"],
      "env": {
        "NOTION_API_KEY": "your-integration-token",
        "DEFAULT_PAGE_ID": "your-default-page",
        "CACHE_DURATION": "3600",
        "MAX_BLOCKS_PER_REQUEST": "100"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Notion account
- Notion integration token
- Workspace permissions

## Related Servers

- None currently listed
