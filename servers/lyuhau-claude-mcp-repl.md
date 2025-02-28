---
type: server
repo_url: https://github.com/lyuhau/claude-mcp-repl
name: Claude REPL MCP Server
owner: lyuhau
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
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

A Python-based REPL server that enhances Claude with Python execution, shell commands, and file manipulation capabilities.

## Features

### Python Tools

- **One-off Python (`python`)**: Run code in fresh environments

  - Great for quick calculations and tests
  - Pandas and PyArrow support available
  - Clean environment each time

- **Session-based Python (`python_session`)**: Run code with persistent state

  - Keep variables between executions
  - Perfect for data analysis workflows
  - Sessions remain active for 5 minutes

### Shell Tools

- **Command execution (`shell`)**: Run shell commands

  - Quick commands return immediately
  - Long-running commands switch to async mode
  - Returns task ID for tracking

- **Task status (`shell_status`)**: Monitor long-running commands

  - Check progress of async commands
  - Get outputs when completed
  - View execution time and results

### File Tools

- **File modification (`perl`)**: Safe text processing
  - Pattern-based search and replace
  - Multi-line transformations
  - UTF-8 support built-in
  - Preserves file structure

## Installation

1.  Clone the repository
2.  Install dependencies:

    ```bash
    poetry install
    ```

    or

    ```bash
    uv pip install -r pyproject.toml
    ```

## Usage

Add to your Claude Desktop config file:

```json
{
  "mcpServers": {
    "repl": {
      "command": "/path/to/python/env/bin/python",
      "args": ["-m", "repl"]
    }
  }
}
```

Config locations:

- Windows: `%APPDATA%/Roaming/Claude/claude_desktop_config.json`
- macOS: (TBD)
- Linux: (TBD)

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
