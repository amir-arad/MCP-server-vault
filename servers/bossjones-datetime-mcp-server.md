---
type: server
repo_url: https://github.com/bossjones/datetime-mcp-server
name: DateTime Notes MCP Server
owner: bossjones
stars: 0
last_updated: 2025-02-07
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "purpose/note-management",
    "tech/uri-scheme",
    "purpose/summarization",
    "purpose/organization",
  ]
---

# DateTime Notes MCP Server

#status/active #category/productivity #purpose/note-management #tech/uri-scheme #purpose/summarization #purpose/organization

## Description

This server enables users to store, manage, and summarize notes using a custom URI scheme, with functionality to add new notes and generate summaries with varying levels of detail.

## Features

- Note storage
- URI-based access
- Summary generation
- Note management
- Custom schemes
- Detail levels
- Search capability
- Organization tools
- Export options
- Version tracking

## Installation

```bash
npm install @bossjones/datetime-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "datetime-notes": {
      "command": "npx",
      "args": ["@bossjones/datetime-mcp"],
      "env": {
        "STORAGE_PATH": "./notes",
        "URI_PREFIX": "note://",
        "SUMMARY_LEVELS": "3",
        "MAX_NOTE_SIZE": "10mb",
        "BACKUP_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Storage system
- URI parser
- Summary generator
- Search engine
- Backup manager

## Related Servers

- zeparhyfar/mcp-datetime
- modelcontextprotocol-notes-server
- claudekeep/mcp-server
