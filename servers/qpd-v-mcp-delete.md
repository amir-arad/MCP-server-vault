---
type: server
repo_url: https://github.com/qpd-v/mcp-delete
name: File Deletion MCP Server
owner: qpd-v
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_009.md"]
tags:
  [
    "status/active",
    "category/filesystem",
    "purpose/file-deletion",
    "purpose/cleanup",
    "tech/paths",
    "purpose/safety",
  ]
---

# File Deletion MCP Server

#status/active #category/filesystem #purpose/file-deletion #purpose/cleanup #tech/paths #purpose/safety

## Description

A Model Context Protocol (MCP) server that provides file deletion capabilities. This server allows AI assistants to safely delete files when needed, with support for both relative and absolute paths.

## Features

- File deletion
- Path validation
- Safety checks
- Permission handling
- Recursive deletion
- Confirmation system
- Error handling
- Path resolution
- Logging support
- Recovery options

## Installation

```bash
npm install @qpd-v/mcp-delete
```

## Usage

```javascript
{
  "mcpServers": {
    "file-delete": {
      "command": "npx",
      "args": ["@qpd-v/mcp-delete"],
      "env": {
        "ALLOWED_PATHS": "./,/tmp",
        "REQUIRE_CONFIRM": "true",
        "LOG_DELETIONS": "true",
        "BACKUP_ENABLED": "false",
        "SAFETY_LEVEL": "high"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- File system access
- Path resolver
- Permission checker
- Logger
- Backup system

## Related Servers

- modelcontextprotocol-filesystem-server
- pimpmynines-ai-mcp-server-filesystem
- modelcontextprotocol-cleanup-server
