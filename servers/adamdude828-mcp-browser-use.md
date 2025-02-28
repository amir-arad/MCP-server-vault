---
type: server
repo_url: https://github.com/adamdude828/mcp-browser-use
name: Browser Use MCP Server
owner: adamdude828
stars: 0
last_updated: 2025-02-05
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "purpose/note-taking",
    "purpose/summarization",
  ]
---

# Browser Use MCP Server

#status/active #category/productivity #purpose/note-taking #purpose/summarization

## Description

This server provides a note storage system with a custom URI scheme, allowing users to add and summarize notes, with adjustable summary detail levels.

## Features

- Note storage system
- Custom URI scheme
- Note summarization
- Detail level adjustment
- Content organization
- Search functionality
- Tag management
- Export capabilities

## Installation

```bash
npm install @adamdude828/mcp-browser-use
```

## Usage

```javascript
{
  "mcpServers": {
    "browser-use": {
      "command": "npx",
      "args": ["@adamdude828/mcp-browser-use"],
      "env": {
        "STORAGE_PATH": "./notes",
        "SUMMARY_LEVELS": "brief,detailed,full",
        "DEFAULT_LEVEL": "detailed",
        "MAX_NOTE_SIZE": "10MB"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Storage system
- URI handler
- Text processing tools

## Related Servers

- JovaniPink/mcp-browser-use
- Saik0s/mcp-browser-use
