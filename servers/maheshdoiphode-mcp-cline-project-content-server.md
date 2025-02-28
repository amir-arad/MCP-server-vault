---
type: server
repo_url: https://github.com/MaheshDoiphode/mcp-cline-project-content-server
name: Cline Project Content MCP Server
owner: MaheshDoiphode
stars: 3
last_updated: 2025-01-22
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/development",
    "tech/cline",
    "purpose/file-access",
    "purpose/content-management",
    "tech/filesystem",
  ]
---

# Cline Project Content MCP Server

#status/active #category/development #tech/cline #purpose/file-access #purpose/content-management #tech/filesystem

## Description

An MCP server that provides access to project files and their contents, allowing users to retrieve file data from specified project directories with error handling and configuration options.

## Features

- File content access
- Directory navigation
- Error handling
- Content retrieval
- Path resolution
- File type detection
- Access control
- Content caching
- Search capabilities
- Change monitoring

## Installation

```bash
npm install @maheshdoiphode/mcp-cline-project-content
```

## Usage

```javascript
{
  "mcpServers": {
    "project-content": {
      "command": "npx",
      "args": ["@maheshdoiphode/mcp-cline-project-content"],
      "env": {
        "PROJECT_ROOT": "./",
        "ALLOWED_EXTENSIONS": "*",
        "CACHE_ENABLED": "true",
        "WATCH_CHANGES": "true",
        "MAX_FILE_SIZE": "10mb"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- File system access
- Content parser
- Cache system
- File watcher
- Path resolver

## Related Servers

- modelcontextprotocol-filesystem-server
- bradfair/mcp-cline-personas
- davidvc/code-knowledge-mcptool
