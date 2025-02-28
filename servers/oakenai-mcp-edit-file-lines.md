---
type: server
repo_url: https://github.com/oakenai/mcp-edit-file-lines
name: Edit File Lines MCP Server
owner: oakenai
stars: 16
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/development",
    "purpose/file-editing",
    "purpose/text-processing",
    "tech/line-editing",
    "purpose/safety",
  ]
---

# Edit File Lines MCP Server

#status/active #category/development #purpose/file-editing #purpose/text-processing #tech/line-editing #purpose/safety

## Description

Provides precise line-based editing tools for text files within allowed directories, enabling safe and controlled bulk modifications across multiple files.

## Features

- Line-based text editing
- Directory access control
- Bulk file modifications
- Safety checks
- Line number tracking
- Change validation
- Backup creation
- Undo capabilities
- Permission management
- Operation logging

## Installation

```bash
npm install @oakenai/mcp-edit-file-lines
```

## Usage

```javascript
{
  "mcpServers": {
    "edit-file-lines": {
      "command": "npx",
      "args": ["@oakenai/mcp-edit-file-lines"],
      "env": {
        "ALLOWED_DIRS": "./src,./config",
        "BACKUP_ENABLED": "true",
        "MAX_FILE_SIZE": "1048576"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- File system access
- Text processing libraries
- Diff utilities
- Backup storage

## Related Servers

- None currently listed
