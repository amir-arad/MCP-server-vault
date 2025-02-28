---
type: server
repo_url: https://github.com/lyuhau/claude-mcp-repl
name: Claude REPL MCP Server
owner: lyuhau
stars: 0
last_updated: 2025-01-03
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/development",
    "tech/python",
    "purpose/code-execution",
    "purpose/shell-commands",
    "tech/repl",
  ]
---

# Claude REPL MCP Server

#status/active #category/development #tech/python #purpose/code-execution #purpose/shell-commands #tech/repl

## Description

Provides a Python REPL server for executing code and shell commands, enabling complex data analysis and system administration tasks through an interactive Python environment.

## Features

- Python code execution
- Shell command integration
- Interactive REPL
- Variable persistence
- Module management
- Output capture
- Error handling
- History tracking
- Completion support
- Environment isolation

## Installation

```bash
npm install @lyuhau/claude-mcp-repl
```

## Usage

```javascript
{
  "mcpServers": {
    "claude-repl": {
      "command": "npx",
      "args": ["@lyuhau/claude-mcp-repl"],
      "env": {
        "PYTHON_PATH": "/usr/bin/python3",
        "VIRTUAL_ENV": "./venv",
        "MAX_EXECUTION_TIME": "30",
        "ALLOWED_MODULES": "*",
        "HISTORY_SIZE": "1000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Python >= 3.8
- Virtual environment
- Shell access
- History manager
- Code parser

## Related Servers

- modelcontextprotocol-python-server
- kivo360-anthropic-mcp-code-analyzer
- runekaagaard-mcp-alchemy
