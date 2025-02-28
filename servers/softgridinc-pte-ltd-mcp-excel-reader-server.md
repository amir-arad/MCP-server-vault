---
type: server
repo_url: https://github.com/softgridinc-pte-ltd/mcp-excel-reader-server
name: Excel Reader MCP Server
owner: softgridinc-pte-ltd
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/data-processing",
    "integration/excel",
    "purpose/data-extraction",
    "purpose/analysis",
    "purpose/reporting",
    "tech/python",
    "tech/openpyxl"
  ]
---

# Excel Reader MCP Server

#status/active #category/data-processing #integration/excel #purpose/data-extraction #purpose/analysis #purpose/reporting #tech/python #tech/openpyxl

## Description

Integrates with Excel files to extract and process data from sheets, enabling automated analysis and reporting tasks. It provides tools for reading data from Excel files and presenting it in a structured format for further processing.

## Features

- Data extraction
- Sheet processing
- Automated analysis
- Report generation
- Format handling
- Data validation
- Error checking
- Batch processing
- Formula evaluation
- Result formatting
- OpenPyXL integration
- Multi-format support

## Installation

```bash
# Install dependencies
pip install openpyxl
```

## Usage

```javascript
{
  "mcpServers": {
    "excel-reader": {
      "command": "uv",
      "args": ["excel-reader-server"],
      "env": {
        "INPUT_DIR": "./input",
        "OUTPUT_DIR": "./output",
        "DEFAULT_FORMAT": "json",
        "VALIDATE_DATA": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Excel processing libraries (OpenPyXL)
- File system access
- Data validation tools
- Report generation libraries
- Python runtime

## Related Servers

- ArchimedesCrypto/excel-reader-mcp
- Lipdog/excel-master-mcp