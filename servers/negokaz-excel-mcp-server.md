---
type: server
repo_url: https://github.com/negokaz/excel-mcp-server
name: Excel MCP Server
owner: negokaz
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/spreadsheet",
    "integration/microsoft-excel",
    "purpose/text-data",
    "purpose/file-io",
    "tech/xlsx",
    "tech/go",
    "tech/javascript"
  ]
---

# Excel MCP Server

#status/active #category/spreadsheet #integration/microsoft-excel #purpose/text-data #purpose/file-io #tech/xlsx #tech/go #tech/javascript

## Description

Integrates with Microsoft Excel to enable reading and writing of text data in xlsx files for spreadsheet manipulation and analysis tasks. It provides functionalities to read and write text data within Excel files, enabling seamless integration with spreadsheet applications.

## Features

- XLSX file handling
- Text data reading
- Text data writing
- Spreadsheet manipulation
- Data analysis
- Format preservation
- Cell management
- Sheet handling
- Error detection
- Data validation
- Multi-format support
- Smithery installation
- UV installation

## Installation

```bash
# Installing via NPM
npx -y @smithery/cli install @negokaz/excel-mcp-server --client claude

# Manual Installation
npm install @negokaz/excel-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "excel": {
      "command": "npx",
      "args": ["@negokaz/excel-mcp-server"],
      "env": {
        "FILE_DIR": "./excel-files",
        "ENCODING": "utf8",
        "MAX_FILE_SIZE": "10MB",
        "BACKUP_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 20
- Microsoft Excel
- XLSX libraries
- Text processing tools
- File system access
- Go runtime
- JavaScript modules

## Related Servers

- haris-musa/excel-mcp-server
- ArchimedesCrypto/excel-reader-mcp