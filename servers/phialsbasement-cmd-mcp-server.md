---
type: server
repo_url: https://github.com/PhialsBasement/CMD-MCP-Server
name: CMD MCP Server
owner: PhialsBasement
stars: 7
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/system",
    "tech/cmd",
    "purpose/command-execution",
    "tech/windows",
    "purpose/system-control",
  ]
---

# CMD MCP Server

#status/active #category/system #tech/cmd #purpose/command-execution #tech/windows #purpose/system-control

## Description

MCP server allowing any and all command execution over CMD. This server provides a direct interface to the Windows Command Prompt for executing system commands and scripts.

## Features

- Command execution
- Output capture
- Error handling
- Environment control
- Process management
- Path resolution
- Variable handling
- Batch processing
- Script execution
- Session management

## Installation

```bash
npm install @phialsbasement/cmd-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "cmd": {
      "command": "npx",
      "args": ["@phialsbasement/cmd-mcp"],
      "env": {
        "CMD_PATH": "C:\\Windows\\System32\\cmd.exe",
        "WORKING_DIR": "C:\\",
        "MAX_BUFFER": "1048576",
        "TIMEOUT": "30000",
        "ENCODING": "utf8"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Windows OS
- CMD.exe
- Process manager
- Output handler
- Error handler

## Related Servers

- modelcontextprotocol-terminal-server
- wonderwhy-er-claudecomputercommander
- andre-jesus-claude-mcp
