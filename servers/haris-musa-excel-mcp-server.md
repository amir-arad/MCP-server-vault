---
type: server
repo_url: https://github.com/haris-musa/excel-mcp-server
name: Excel MCP Server
owner: haris-musa
stars: 6
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/spreadsheet",
    "integration/excel",
    "purpose/workbook-creation",
    "purpose/data-manipulation",
    "purpose/formatting",
    "tech/python",
    "tech/openpyxl"
  ]
---

# Excel MCP Server

#status/active #category/spreadsheet #integration/excel #purpose/workbook-creation #purpose/data-manipulation #purpose/formatting #tech/python #tech/openpyxl

## Description

Provides Excel file manipulation capabilities without requiring Microsoft Excel installation. This server enables workbook creation, data manipulation, formatting, and advanced Excel features, leveraging OpenPyXL for seamless spreadsheet operations.

## Features

- Workbook creation
- Data manipulation
- Cell formatting
- Formula management
- Chart creation
- Pivot table support
- Template handling
- Style management
- Data validation
- Macro support
- OpenPyXL integration
- Comprehensive Excel support

## Installation

```bash
# Install dependencies
pip install openpyxl
```

## Usage

```javascript
{
  "mcpServers": {
    "excel": {
      "command": "uv",
      "args": ["excel-mcp-server"],
      "env": {
        "WORKBOOK_DIR": "./workbooks",
        "TEMPLATE_DIR": "./templates",
        "MACRO_ENABLED": "false",
        "DEFAULT_FORMAT": "xlsx"
      }
    }
  }
}
```

## Dependencies

- Python 3.10+
- OpenPyXL 3.1.2+
- File system access
- Memory management
- Formula parser
- MCP SDK

## Related Servers

- Lipdog/excel-master-mcp
- ArchimedesCrypto/excel-reader-mcp