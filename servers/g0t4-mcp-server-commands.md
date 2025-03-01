---
type: server
repo_url: https://github.com/g0t4/mcp-server-commands
name: Commands MCP Server
owner: g0t4
stars: 52
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/system",
    "purpose/command-execution",
    "purpose/automation",
    "tech/shell",
    "purpose/system-control",
    "tech/javascript",
  ]
---

# Commands MCP Server

#status/active #category/system #purpose/command-execution #purpose/automation #tech/shell #purpose/system-control

## Description

An MCP server to run commands. This server provides a streamlined interface for executing system commands with proper security controls and output handling.

## Features

- Command execution
- Output capture
- Error handling
- Security controls
- Process management
- Environment control
- Shell integration
- Command chaining
- Status monitoring
- Result formatting

## Installation

```bash
npm install @g0t4/mcp-server-commands
```

## Usage

```javascript
{
  "mcpServers": {
    "commands": {
      "command": "npx",
      "args": ["@g0t4/mcp-server-commands"],
      "env": {
        "SHELL_PATH": "/bin/bash",
        "WORKING_DIR": "./",
        "TIMEOUT": "30000",
        "MAX_BUFFER": "1048576",
        "ALLOW_SUDO": "false"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Shell environment
- Process manager
- Output handler
- Security module
- Environment manager

## Related Servers

- sunwood-ai-labs/command-executor-mcp-server
- andrew-beniash/mcp-command-server
- phialsbasement/cmd-mcp-server
