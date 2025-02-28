---
type: server
repo_url: https://github.com/ngeojiajun/mcp-code-snippets
name: Code Snippets MCP Server
owner: ngeojiajun
stars: 4
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/development",
    "purpose/code-management",
    "purpose/snippets",
    "tech/multi-language",
    "purpose/storage",
  ]
---

# Code Snippets MCP Server

#status/active #category/development #purpose/code-management #purpose/snippets #tech/multi-language #purpose/storage

## Description

A MCP server for managing and storing code snippets in various programming languages, allowing users to create, list, and delete snippets via a standardized interface.

## Features

- Snippet management
- Multi-language support
- Storage system
- Search functionality
- Tag organization
- Version control
- Syntax highlighting
- Access control
- Import/Export
- Sharing capabilities

## Installation

```bash
npm install @ngeojiajun/mcp-code-snippets
```

## Usage

```javascript
{
  "mcpServers": {
    "code-snippets": {
      "command": "npx",
      "args": ["@ngeojiajun/mcp-code-snippets"],
      "env": {
        "STORAGE_PATH": "./snippets",
        "DEFAULT_LANGUAGE": "javascript",
        "MAX_SIZE": "1mb",
        "ENABLE_SHARING": "true",
        "BACKUP_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Storage backend
- Language parser
- Search indexer
- Version control
- Syntax highlighter

## Related Servers

- davidvc/code-knowledge-mcptool
- seanivore/mcp-code-analyzer
- modelcontextprotocol-git-server
