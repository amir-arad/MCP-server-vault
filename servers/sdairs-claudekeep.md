---
type: server
repo_url: https://github.com/sdairs/claudekeep
name: ClaudeKeep MCP Server
owner: sdairs
stars: 4
last_updated: 2025-01-14
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/knowledge-management",
    "purpose/note-taking",
    "purpose/organization",
    "tech/typescript",
    "category/productivity",
  ]
---

# ClaudeKeep MCP Server

#status/active #category/knowledge-management #purpose/note-taking #purpose/organization #tech/typescript #category/productivity

## Description

Integrates a personal knowledge management system for storing, retrieving, and organizing conversation notes locally. This MCP server provides a comprehensive solution for managing and organizing AI conversation history and insights.

## Features

- Note storage
- Content organization
- Search functionality
- Tag management
- Category system
- Version control
- Export options
- Import capabilities
- Backup management
- Cross-referencing

## Installation

```bash
npm install @sdairs/claudekeep
```

## Usage

```javascript
{
  "mcpServers": {
    "claudekeep": {
      "command": "npx",
      "args": ["@sdairs/claudekeep"],
      "env": {
        "STORAGE_PATH": "./notes",
        "INDEX_PATH": "./index",
        "BACKUP_INTERVAL": "86400",
        "MAX_VERSION_HISTORY": "10",
        "SEARCH_ALGORITHM": "fuzzy"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Local storage system
- Search engine
- Version control system
- Backup manager
- Markdown processor

## Related Servers

- davidteren-claude-server
- akira-papa-akirapapa-mcp-notion-server
- modelcontextprotocol-memory-server
