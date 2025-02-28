---
type: server
repo_url: https://github.com/ArchimedesCrypto/excel-reader-mcp
name: Excel Reader MCP Server
owner: ArchimedesCrypto
stars: 5
last_updated: 2025-02-19
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/data-processing",
    "integration/excel",
    "purpose/file-reading",
    "tech/chunking",
    "purpose/pagination",
  ]
---

# Excel Reader MCP Server

#status/active #category/data-processing #integration/excel #purpose/file-reading #tech/chunking #purpose/pagination

## Description

Provides efficient handling of large Excel files through automatic chunking and pagination, using MCP to enable seamless file reading and management features such as sheet selection and error handling.

## Features

- Large file handling
- Automatic chunking
- Pagination support
- Sheet selection
- Error handling
- Memory optimization
- Progress tracking
- Data validation
- Format detection
- Stream processing

## Installation

```bash
npm install @archimedescrypto/excel-reader-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "excel-reader": {
      "command": "npx",
      "args": ["@archimedescrypto/excel-reader-mcp"],
      "env": {
        "CHUNK_SIZE": "1000",
        "MAX_MEMORY": "512MB",
        "TEMP_DIR": "./temp",
        "CACHE_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Excel file support
- Streaming libraries
- Memory management
- Temporary storage

## Related Servers

- [Excel Server](https://github.com/haris-musa/excel-mcp-server) - Full Excel implementation
- [Excel Master MCP](https://github.com/Lipdog/excel-master-mcp) - Advanced Excel operations
