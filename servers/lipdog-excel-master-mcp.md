---
type: server
repo_url: https://github.com/Lipdog/excel-master-mcp
name: Excel Master MCP Server
owner: Lipdog
stars: 5
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/data-analysis",
    "integration/excel",
    "tech/xlwings",
    "purpose/automation",
    "purpose/reporting",
    "tech/python"
  ]
---

# Excel Master MCP Server

#status/active #category/data-analysis #integration/excel #tech/xlwings #purpose/automation #purpose/reporting #tech/python

## Description

Integrates with Excel using XLwings to enable automated data manipulation, analysis, and reporting for business workflows. It provides tools for automating Excel-based tasks, enabling data analysis and report generation with minimal manual intervention.

## Features

- Excel automation
- Data manipulation
- Analysis tools
- Report generation
- XLwings integration
- Workflow automation
- Template management
- Data validation
- Formula handling
- Batch processing
- Python scripting
- Windows support

## Installation

```bash
pip install xlwings
pip install excel-master-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "excel-master": {
      "command": "python",
      "args": ["-m", "excel_master_mcp"],
      "env": {
        "EXCEL_PATH": "C:\\Program Files\\Microsoft Office\\root\\Office16\\EXCEL.EXE",
        "TEMPLATE_DIR": "./templates",
        "OUTPUT_DIR": "./reports",
        "VISIBLE": "false"
      }
    }
  }
}
```

## Dependencies

- Python >= 3.7
- Microsoft Excel (Windows)
- XLwings
- Windows OS
- Office automation permissions

## Related Servers

- haris-musa/excel-mcp-server