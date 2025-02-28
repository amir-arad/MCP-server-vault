---
type: server
repo_url: https://github.com/zereight/confluence-mcp
name: Confluence & Jira MCP Server
owner: zereight
stars: 1
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/confluence",
    "integration/jira",
    "purpose/wiki",
    "purpose/project-management",
  ]
---

# Confluence & Jira MCP Server

#status/active #category/productivity #integration/confluence #integration/jira #purpose/wiki #purpose/project-management

## Description

An MCP server that integrates with both Confluence wiki and Jira project management systems, providing unified access to documentation and issue tracking capabilities.

## Features

- Wiki management
- Issue tracking
- Content creation
- Project management
- Search functionality
- Permission handling
- Version control
- Comment management
- Attachment support
- Cross-linking

## Installation

```bash
npm install @zereight/confluence-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "confluence-jira": {
      "command": "npx",
      "args": ["@zereight/confluence-mcp"],
      "env": {
        "ATLASSIAN_URL": "your-instance.atlassian.net",
        "API_TOKEN": "your-api-token",
        "DEFAULT_PROJECT": "your-project",
        "WIKI_SPACE": "your-space",
        "SYNC_INTERVAL": "300"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Atlassian Cloud account
- API token
- Content processor
- Issue tracker
- Permission manager

## Related Servers

- mouhamadalmounayar/mcp-confluence
- aaronsb/confluence-cloud-mcp
- ks-gen-ai/confluence-mcp-server
