---
type: server
repo_url: https://github.com/sirmews/apple-notes-mcp
name: Apple Notes MCP Server
owner: sirmews
stars: 40
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/productivity", "integration/apple", "purpose/note-management", "tech/macos", "tech/python"]
---

# Apple Notes MCP Server

#status/active #category/productivity #integration/apple #purpose/note-management #tech/macos #tech/python

## Description

A Model Context Protocol server that allows Claude to read from your local Apple Notes database on macOS. Provides tools to search, retrieve, and access your notes directly from the Claude interface.

## Features

- Get all notes from the database
- Read full content of specific notes
- Search through notes with query functionality
- Note metadata access
- Content parsing and formatting
- Folder organization support
- Local database access
- Database querying

## Installation

```bash
# Using uv (recommended)
uvx apple-notes-mcp

# Or with pip
uv pip install apple-notes-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "apple-notes": {
      "command": "uvx",
      "args": ["apple-notes-mcp"]
    }
  }
}
```

## Dependencies

- macOS (requires Full Disk Access permissions)
- Python 3.8+
- uv (recommended for installation)
- Apple Notes app
- SQLite3

## Related Servers

- Dhravya/apple-mcp - General Apple integration
- RafalWilinski/mcp-apple-notes - Alternative Apple Notes integration
- turlockmike/apple-notifier-mcp - Apple notifications
- joshrutkowski/applescript-mcp - AppleScript integration