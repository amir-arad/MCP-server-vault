---
type: server
repo_url: https://github.com/Alihkhawaher/everything-search-server
name: Everything Search Server
owner: Alihkhawaher
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/search",
    "integration/everything",
    "purpose/file-search",
    "purpose/file-management",
    "tech/query-options",
    "tech/javascript",
    "tech/typescript"
  ]
---

# Everything Search Server

#status/active #category/search #integration/everything #purpose/file-search #purpose/file-management #tech/query-options #tech/javascript #tech/typescript

## Description

Integrates with the Everything Search Engine to enable file search and management across large file systems using advanced query options and customizable result formatting. It provides a powerful search interface for locating files and directories quickly and efficiently.

## Features

- Large-scale file search
- Advanced query options
- Result formatting
- File management
- Search customization
- Pattern matching
- Filter capabilities
- Sorting options
- Batch operations
- Search history
- Regex support
- Case-sensitive search
- Whole word search

## Installation

```bash
npm install @alihkhawaher/everything-search-server
```

## Usage

```javascript
{
  "mcpServers": {
    "everything-search": {
      "command": "npx",
      "args": ["@alihkhawaher/everything-search-server"],
      "env": {
        "SEARCH_ROOT": "C:\\",
        "RESULT_FORMAT": "json",
        "MAX_RESULTS": "500",
        "INCLUDE_HIDDEN": "false"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Everything Search Engine
- Windows OS
- File system access
- Query parser
- TypeScript runtime

## Related Servers

- mamertofabian/mcp-everything-search