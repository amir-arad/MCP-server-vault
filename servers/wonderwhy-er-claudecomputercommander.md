---
type: server
repo_url: https://github.com/wonderwhy-er/ClaudeComputerCommander
name: Claude Computer Commander MCP Server
owner: wonderwhy-er
stars: 32
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/system",
    "purpose/automation",
    "purpose/process-management",
    "tech/terminal",
    "tech/filesystem",
  ]
---

# Claude Computer Commander MCP Server

#status/active #category/system #purpose/automation #purpose/process-management #tech/terminal #tech/filesystem

## Description

Integrates terminal and filesystem capabilities for executing system commands, managing processes, and performing advanced file operations on the local system.

## Features

- System command execution
- Process management
- File operations
- Directory handling
- Permission management
- Environment control
- Job scheduling
- Output capture
- Error handling
- Resource monitoring

## Installation

```bash
npm install @wonderwhy-er/claude-computer-commander
```

## Usage

```javascript
{
  "mcpServers": {
    "computer-commander": {
      "command": "npx",
      "args": ["@wonderwhy-er/claude-computer-commander"],
      "env": {
        "ALLOWED_PATHS": "/home/user,/tmp",
        "MAX_PROCESSES": "10",
        "TIMEOUT": "30000",
        "LOG_LEVEL": "info",
        "SANDBOX_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Shell access
- Process manager
- File system API
- Permission handler
- Resource monitor

## Related Servers

- modelcontextprotocol-filesystem-server
- andre-jesus-claude-mcp
- shin-t-o-mcp-access
