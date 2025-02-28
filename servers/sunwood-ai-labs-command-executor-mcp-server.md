---
type: server
repo_url: https://github.com/Sunwood-ai-labs/command-executor-mcp-server
name: Command Executor MCP Server
owner: Sunwood-ai-labs
stars: 13
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/automation",
    "purpose/command-execution",
    "purpose/system-management",
    "tech/security",
    "category/system",
  ]
---

# Command Executor MCP Server

#status/active #category/automation #purpose/command-execution #purpose/system-management #tech/security #category/system

## Description

Enables secure execution of pre-approved system commands for automation tasks, system management, and controlled access to host resources.

## Features

- Secure command execution
- Pre-approval system
- Automation support
- System management
- Access control
- Command validation
- Execution logging
- Resource monitoring
- Output handling
- Security policies

## Installation

```bash
npm install @sunwood-ai-labs/command-executor-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "command-executor": {
      "command": "npx",
      "args": ["@sunwood-ai-labs/command-executor-mcp"],
      "env": {
        "ALLOWED_COMMANDS": "ls,ps,df,top",
        "SECURITY_LEVEL": "high",
        "LOG_PATH": "./logs",
        "MAX_RUNTIME": "300",
        "SANDBOX_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Security module
- Command validator
- Logging system
- Resource monitor
- Access controller

## Related Servers

- andrew-beniash/mcp-command-server
- g0t4/mcp-server-commands
- phialsbasement/cmd-mcp-server
