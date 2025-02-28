--- 
type: server
repo_url: https://github.com/ZeparHyfar/mcp-datetime
name: DateTime Formatting MCP Server
owner: ZeparHyfar
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/utility",
    "purpose/datetime",
    "purpose/formatting",
    "integration/claude",
    "tech/time",
  ]
---

# DateTime Formatting MCP Server

#status/active #category/utility #purpose/datetime #purpose/formatting #integration/claude #tech/time

## Description

A datetime formatting service implemented as an MCP server for the Claude Desktop Application. Supports generation of datetime strings in various formats.

## Features

- DateTime formatting
- Format customization
- Timezone support
- Locale handling
- Format validation
- String generation
- Pattern matching
- Error handling
- Format conversion
- Timezone conversion

## Installation

Before using mcp-datetime, ensure you have the following tools installed:

- Python 3.12 or later
- uv (Python package installer)
- uvx (Python package runner)

### About Installation

If you need to install the package directly (e.g., for development or source code inspection), you can use one of these methods:

- Install from PyPI

```bash
pip install mcp-datetime
```

- Install from GitHub Source

```bash
git clone https://github.com/ZeparHyfar/mcp-datetime.git
cd mcp-datetime
pip install -e .
```

- Example `claude_desktop_config.json` for manual installation

```json
{
 "mcpServers": {
 "mcp-datetime": {
 "command": "python",
 "args": ["-m", "mcp_datetime"],
 "env": {
 "PYTHON": "/path/to/your/python"
 }
 }
 }
}
```

Replace "/path/to/your/python" with your actual Python interpreter path

> e.g., "/usr/local/bin/python3" or "/Users/username/.pyenv/versions/3.12.0/bin/python3"

## Usage

### Basic Examples

- Command format

```
# Standard datetime format
call datetime-service.get_datetime {"format": "datetime"}
# Result: 2024-12-10 00:54:01

# Japanese format
call datetime-service.get_datetime {"format": "datetime_jp"}
# Result: 2024年12月10日 00時54分01秒

# Filename format
call datetime-service.get_datetime {"format": "filename_md"}
# Result: 20241210005401.md
```

- Claude Desktop App prompt examples

  - User

    ```
Please tell me the current time in date_slash format
    ```

  - Claude

    ```
I'll get the current date in date_slash format.

The current date is 2024/12/12
    ```

## Dependencies

- Node.js >= 16
- DateTime library
- Timezone database
- Locale data
- Format parser
- Validation engine

## Related Servers

- bossjones/datetime-mcp-server
- modelcontextprotocol-time-server
- modelcontextprotocol-utility-server