---
type: server
repo_url: https://github.com/PimpMyNines/ai-mcp-server-filesystem
name: AI Filesystem MCP Server
owner: PimpMyNines
stars: 1
last_updated: 2025-02-18
status: inactive
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/inactive",
    "category/filesystem",
    "purpose/file-management",
    "category/ai",
  ]
---

# AI Filesystem MCP Server

#status/inactive #category/filesystem #purpose/file-management #category/ai

## Description

Provides a secure and scalable filesystem service for reading, writing, and searching files within a specified workspace, enabling structured file access and content manipulation tasks.

## Features

- Secure file operations
- Workspace management
- File reading and writing
- Content search capabilities
- Structured file access
- Content manipulation
- Directory traversal
- File metadata handling

## Installation

```bash
npm install @pimpmynines/ai-mcp-server-filesystem
```

## Usage

```javascript
{
  "mcpServers": {
    "ai-filesystem": {
      "command": "npx",
      "args": ["@pimpmynines/ai-mcp-server-filesystem"],
      "env": {
        "WORKSPACE_ROOT": "./workspace",
        "MAX_FILE_SIZE": "10MB",
        "ALLOWED_EXTENSIONS": ".txt,.md,.json,.yml",
        "SEARCH_DEPTH": "5"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- File system permissions
- Search indexing library

## Related Servers

- None currently listed
