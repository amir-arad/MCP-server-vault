---
type: server
repo_url: https://github.com/RonaldDegsa/server-everything
name: Everything Server
owner: RonaldDegsa
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/system",
    "purpose/file-handling",
    "purpose/information-retrieval",
    "purpose/http-requests",
    "purpose/command-execution",
    "tech/nodejs",
  ]
---

# Everything Server

#status/active #category/system #purpose/file-handling #purpose/information-retrieval #purpose/http-requests #purpose/command-execution

## Description

Provides system-level operations for file handling, information retrieval, HTTP requests, and command execution, enabling versatile system management and task automation.

## Features

- File handling operations
- Information retrieval
- HTTP request management
- Command execution
- System monitoring
- Task automation
- Resource management
- Process control
- Error handling
- Logging system

## Installation

```bash
npm install @ronalddegsa/server-everything
```

## Usage

```javascript
{
  "mcpServers": {
    "everything": {
      "command": "npx",
      "args": ["@ronalddegsa/server-everything"],
      "env": {
        "ALLOWED_PATHS": "./data,./logs",
        "MAX_PROCESSES": "10",
        "TIMEOUT": "30000",
        "LOG_LEVEL": "info"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- System access permissions
- HTTP client library
- File system access
- Process management tools

## Related Servers

- [Everything MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/everything) - Official Everything implementation
