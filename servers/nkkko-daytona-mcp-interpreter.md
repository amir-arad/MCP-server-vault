---
type: server
repo_url: https://github.com/nkkko/daytona-mcp-interpreter
name: Daytona Python Interpreter MCP Server
owner: nkkko
stars: 0
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/development",
    "tech/python",
    "purpose/code-execution",
    "integration/daytona",
    "purpose/workspace",
  ]
---

# Daytona Python Interpreter MCP Server

#status/active #category/development #tech/python #purpose/code-execution #integration/daytona #purpose/workspace

## Description

A Model Context Protocol server that allows execution of Python code within Daytona workspaces, providing a secure and isolated environment for executing and managing Python scripts.

## Features

- Python code execution
- Workspace isolation
- Environment management
- Script handling
- Output capture
- Error handling
- Package management
- Security controls
- Resource limits
- Session persistence

## Installation

```bash
npm install @nkkko/daytona-mcp-interpreter
```

## Usage

```javascript
{
  "mcpServers": {
    "daytona-python": {
      "command": "npx",
      "args": ["@nkkko/daytona-mcp-interpreter"],
      "env": {
        "PYTHON_PATH": "/usr/bin/python3",
        "WORKSPACE_ROOT": "./workspaces",
        "MAX_EXECUTION_TIME": "30",
        "MEMORY_LIMIT": "512mb",
        "ALLOWED_PACKAGES": "*"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Python >= 3.8
- Daytona workspace
- Sandbox environment
- Package manager
- Resource monitor

## Related Servers

- lyuhau/claude-mcp-repl
- modelcontextprotocol-python-server
- modelcontextprotocol-workspace-server
