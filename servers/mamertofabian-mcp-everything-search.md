---
type: server
repo_url: https://github.com/mamertofabian/mcp-everything-search
name: Everything Search MCP Server
owner: mamertofabian
stars: 22
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/search",
    "tech/windows",
    "purpose/file-search",
    "tech/everything-sdk",
    "purpose/filesystem",
    "tech/python",
    "tech/mdfind",
    "tech/locate"
  ]
---

# Everything Search MCP Server

#status/active #category/search #tech/windows #purpose/file-search #tech/everything-sdk #purpose/filesystem #tech/python #tech/mdfind #tech/locate

## Description

This server provides fast file search capabilities across Windows, macOS, and Linux. On Windows, it uses the Everything SDK. On macOS, it uses the built-in `mdfind` command. On Linux, it uses the `locate`/`plocate` command.

## Features

- Fast file search
- Windows, macOS, and Linux support
- Everything SDK usage (Windows)
- mdfind usage (macOS)
- locate/plocate usage (Linux)
- Pattern matching
- Search filtering
- Result sorting
- Path exclusions
- Real-time indexing
- Advanced queries
- Search history
- Cross-platform support

## Installation

```bash
pip install mcp-server-everything-search
```

## Usage

```javascript
{
  "mcpServers": {
    "everything-search": {
      "command": "uvx",
      "args": ["mcp-server-everything-search"],
      "env": {
        "EVERYTHING_SDK_PATH": "path/to/Everything-SDK/dll/Everything64.dll"
      }
    }
  }
}
```

## Dependencies

- Python 3.7+
- Windows, macOS, or Linux
- Everything Search Engine (Windows)
- Everything SDK (Windows)
- mdfind (macOS)
- locate/plocate (Linux)

## Related Servers

- Alihkhawaher/everything-search-server